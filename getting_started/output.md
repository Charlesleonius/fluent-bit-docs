# Output

The output interface allows us to define destinations for the data. Common destinations are remote services, the local file system or a standard interface with others. Outputs are implemented as plugins and there are many available.

![](../.gitbook/assets/logging_pipeline_output.png)

When an output plugin is loaded, an internal _instance_ is created. Every instance has its own independent configuration. Configuration keys are often called **properties**.

Every output plugin has its own documentation section describing how to use it and what properties are available.

For more detail, please refer to the [Output Plugins](../output/) section.

