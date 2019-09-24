# Input

[Fluent Bit](http://fluentbit.io) uses _Input Plugins_ to gather information from different sources. Some just collect data from log files while others can gather metrics information from the operating system. There are many plugins for different needs.

![](../.gitbook/assets/logging_pipeline_input.png)

When an input plugin is loaded, an internal _instance_ is created. Every instance has its own and independent configuration. Configuration keys are often called **properties**.

Every input plugin has its own documentation section describing how to use it and what properties are available.

For more detail, please refer to the [Input Plugins](../input/) section.

