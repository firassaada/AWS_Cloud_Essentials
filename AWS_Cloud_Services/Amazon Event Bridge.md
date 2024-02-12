Amazon EventBridge is a serverless event bus service provided by Amazon Web Services (AWS).
It enables easy and seamless integration of various applications, services, and event sources in an event-driven architecture.
EventBridge simplifies the development of event-driven applications by allowing different components to communicate with each other through events.

The following list describes some core concepts and components of EventBridge:

    Event source: 
    An event source is where the events originate. These sources can be AWS services, such as when a new file is uploaded to Amazon Simple Storage Service (Amazon S3).
    Sources can also include custom applications that send events to EventBridge for processing.

    Event bus:
    An event bus is a central hub where events are collected and delivered to their target. You can think of it as a communication channel that holds and routes events 
    to different parts of the application.EventBridge supports both default event buses and custom event buses.

    Event rules: 
    Event rules define the conditions that determine when an event should be sent from the event bus to a target. You can use event rules to specify filtering criteria 
    for events so that only the relevant events initiate actions.

    Targets:
    Targets are the AWS resources or custom applications that react to events. When the event bus receives an event that matches the conditions defined in an event rule,
    EventBridge forwards that event to the associated target for processing.

    Event patterns:
    Event patterns are used within event rules to filter events based on specific attributes or values. These patterns help you define the criteria for which events are
    triggers for the rule.

    Event archive:
    EventBridge can store a copy of every event that passes through the event bus if you need event copies for auditing, compliance, and analysis.
    You can configure this feature to archive events for a certain period.

    Event replay:
    With event replay, you can replay past events from your archive into an event bus. This feature is useful for testing and debugging. It’s also useful for scenarios
    where you need to re-create the state of your system at a specific time.

    The following diagram shows a basic outline for EventBridge. It includes event sources, which create events and post them to an event bus. After an event enters the
    event bus, it’s evaluated to see if it matches any rules. If a rule is met, the corresponding targets receive a copy of the message to process.

![image](https://github.com/firassaada/AWS_Cloud_Essentials/assets/94303698/bac5f071-cb53-4ab4-98fc-f7dd2f4e37c1)



