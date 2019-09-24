# Getting Started

[Fluent Bit](http://fluentbit.io) is easy to get started with once you understand its basic workflow. Consider the following diagram as a big picture view:

![Fluent Bit Workflow](../.gitbook/assets/logging_pipeline.png)

| Interface | Description |
| :--- | :--- |
| [Input](input.md) | Entry point of data. Implemented through _Input Plugins_, this interface allows you to gather or receive data. E.g: log file content, data over TCP, built-in metrics, etc. |
| [Parser](parser.md) | Parsers allow you to convert unstructured data gathered from the Input interface into structured data. Parsers are optional and depend on the Input plugins. |
| [Filter](filter.md) | The filtering mechanism allows you to _alter_ the data ingested by the Input plugins. Filters are implemented as plugins. |
| [Buffer](buffer.md) | By default, the data ingested by the Input plugins resides in memory until is routed and delivered to an Output interface. |
| [Routing](routing.md) | Data ingested by an Input interface is _tagged_, that means that a Tag is assigned and this one is used to determine where the data should be routed based on a _match_ rule. |
| [Output](output.md) | An output defines a destination for the data. Destinations are handled by output plugins. Note that thanks to the Routing interface, the data can be delivered to multiple destinations. |

