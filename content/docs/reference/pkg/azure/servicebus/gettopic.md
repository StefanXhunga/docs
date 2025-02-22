
---
title: "getTopic"
title_tag: "azure.servicebus.getTopic"
meta_desc: "Documentation for the azure.servicebus.getTopic function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Use this data source to access information about an existing Service Bus Topic.


{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using Azure = Pulumi.Azure;

class MyStack : Stack
{
    public MyStack()
    {
        var example = Output.Create(Azure.ServiceBus.GetTopic.InvokeAsync(new Azure.ServiceBus.GetTopicArgs
        {
            Name = "existing",
            ResourceGroupName = "existing",
            NamespaceName = "existing",
        }));
        this.Id = example.Apply(example => example.Id);
    }

    [Output("id")]
    public Output<string> Id { get; set; }
}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-azure/sdk/v3/go/azure/servicebus"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		example, err := servicebus.LookupTopic(ctx, &servicebus.LookupTopicArgs{
			Name:              "existing",
			ResourceGroupName: "existing",
			NamespaceName:     "existing",
		}, nil)
		if err != nil {
			return err
		}
		ctx.Export("id", example.Id)
		return nil
	})
}
```


{{< /example >}}


{{< example python >}}

```python
import pulumi
import pulumi_azure as azure

example = azure.servicebus.get_topic(name="existing",
    resource_group_name="existing",
    namespace_name="existing")
pulumi.export("id", example.id)
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure from "@pulumi/azure";

const example = azure.servicebus.getTopic({
    name: "existing",
    resourceGroupName: "existing",
    namespaceName: "existing",
});
export const id = example.then(example => example.id);
```


{{< /example >}}





{{% /examples %}}




## Using getTopic {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getTopic<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetTopicArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetTopicResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_topic(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">namespace_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetTopicResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupTopic<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupTopicArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupTopicResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupTopic` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetTopic </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetTopicResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetTopicArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of this Service Bus Topic.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="namespacename_csharp">
<a href="#namespacename_csharp" style="color: inherit; text-decoration: inherit;">Namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Service Bus Namespace.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Resource Group where the Service Bus Topic exists.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of this Service Bus Topic.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="namespacename_go">
<a href="#namespacename_go" style="color: inherit; text-decoration: inherit;">Namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Service Bus Namespace.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Resource Group where the Service Bus Topic exists.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of this Service Bus Topic.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="namespacename_nodejs">
<a href="#namespacename_nodejs" style="color: inherit; text-decoration: inherit;">namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Service Bus Namespace.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Resource Group where the Service Bus Topic exists.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of this Service Bus Topic.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="namespace_name_python">
<a href="#namespace_name_python" style="color: inherit; text-decoration: inherit;">namespace_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Service Bus Namespace.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Resource Group where the Service Bus Topic exists.
{{% /md %}}</dd></dl>
{{% /choosable %}}




## getTopic Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="autodeleteonidle_csharp">
<a href="#autodeleteonidle_csharp" style="color: inherit; text-decoration: inherit;">Auto<wbr>Delete<wbr>On<wbr>Idle</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of the idle interval after which the Topic is automatically deleted, minimum of 5 minutes.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="defaultmessagettl_csharp">
<a href="#defaultmessagettl_csharp" style="color: inherit; text-decoration: inherit;">Default<wbr>Message<wbr>Ttl</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of TTL of messages sent to this topic if no TTL value is set on the message itself.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="duplicatedetectionhistorytimewindow_csharp">
<a href="#duplicatedetectionhistorytimewindow_csharp" style="color: inherit; text-decoration: inherit;">Duplicate<wbr>Detection<wbr>History<wbr>Time<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration during which duplicates can be detected.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enablebatchedoperations_csharp">
<a href="#enablebatchedoperations_csharp" style="color: inherit; text-decoration: inherit;">Enable<wbr>Batched<wbr>Operations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls if server-side batched operations are enabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enableexpress_csharp">
<a href="#enableexpress_csharp" style="color: inherit; text-decoration: inherit;">Enable<wbr>Express</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether Express Entities are enabled. An express topic holds a message in memory temporarily before writing it to persistent storage.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enablepartitioning_csharp">
<a href="#enablepartitioning_csharp" style="color: inherit; text-decoration: inherit;">Enable<wbr>Partitioning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether to enable the topic to be partitioned across multiple message brokers.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="maxsizeinmegabytes_csharp">
<a href="#maxsizeinmegabytes_csharp" style="color: inherit; text-decoration: inherit;">Max<wbr>Size<wbr>In<wbr>Megabytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Integer value which controls the size of memory allocated for the topic. For supported values see the "Queue/topic size" section of [this document](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-quotas).
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="namespacename_csharp">
<a href="#namespacename_csharp" style="color: inherit; text-decoration: inherit;">Namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="requiresduplicatedetection_csharp">
<a href="#requiresduplicatedetection_csharp" style="color: inherit; text-decoration: inherit;">Requires<wbr>Duplicate<wbr>Detection</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic requires duplicate detection.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="status_csharp">
<a href="#status_csharp" style="color: inherit; text-decoration: inherit;">Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Status of the Service Bus Topic. Acceptable values are Active or Disabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="supportordering_csharp">
<a href="#supportordering_csharp" style="color: inherit; text-decoration: inherit;">Support<wbr>Ordering</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic supports ordering.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="autodeleteonidle_go">
<a href="#autodeleteonidle_go" style="color: inherit; text-decoration: inherit;">Auto<wbr>Delete<wbr>On<wbr>Idle</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of the idle interval after which the Topic is automatically deleted, minimum of 5 minutes.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="defaultmessagettl_go">
<a href="#defaultmessagettl_go" style="color: inherit; text-decoration: inherit;">Default<wbr>Message<wbr>Ttl</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of TTL of messages sent to this topic if no TTL value is set on the message itself.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="duplicatedetectionhistorytimewindow_go">
<a href="#duplicatedetectionhistorytimewindow_go" style="color: inherit; text-decoration: inherit;">Duplicate<wbr>Detection<wbr>History<wbr>Time<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration during which duplicates can be detected.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enablebatchedoperations_go">
<a href="#enablebatchedoperations_go" style="color: inherit; text-decoration: inherit;">Enable<wbr>Batched<wbr>Operations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls if server-side batched operations are enabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enableexpress_go">
<a href="#enableexpress_go" style="color: inherit; text-decoration: inherit;">Enable<wbr>Express</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether Express Entities are enabled. An express topic holds a message in memory temporarily before writing it to persistent storage.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enablepartitioning_go">
<a href="#enablepartitioning_go" style="color: inherit; text-decoration: inherit;">Enable<wbr>Partitioning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether to enable the topic to be partitioned across multiple message brokers.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="maxsizeinmegabytes_go">
<a href="#maxsizeinmegabytes_go" style="color: inherit; text-decoration: inherit;">Max<wbr>Size<wbr>In<wbr>Megabytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Integer value which controls the size of memory allocated for the topic. For supported values see the "Queue/topic size" section of [this document](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-quotas).
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="namespacename_go">
<a href="#namespacename_go" style="color: inherit; text-decoration: inherit;">Namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="requiresduplicatedetection_go">
<a href="#requiresduplicatedetection_go" style="color: inherit; text-decoration: inherit;">Requires<wbr>Duplicate<wbr>Detection</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic requires duplicate detection.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="status_go">
<a href="#status_go" style="color: inherit; text-decoration: inherit;">Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Status of the Service Bus Topic. Acceptable values are Active or Disabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="supportordering_go">
<a href="#supportordering_go" style="color: inherit; text-decoration: inherit;">Support<wbr>Ordering</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic supports ordering.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="autodeleteonidle_nodejs">
<a href="#autodeleteonidle_nodejs" style="color: inherit; text-decoration: inherit;">auto<wbr>Delete<wbr>On<wbr>Idle</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of the idle interval after which the Topic is automatically deleted, minimum of 5 minutes.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="defaultmessagettl_nodejs">
<a href="#defaultmessagettl_nodejs" style="color: inherit; text-decoration: inherit;">default<wbr>Message<wbr>Ttl</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of TTL of messages sent to this topic if no TTL value is set on the message itself.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="duplicatedetectionhistorytimewindow_nodejs">
<a href="#duplicatedetectionhistorytimewindow_nodejs" style="color: inherit; text-decoration: inherit;">duplicate<wbr>Detection<wbr>History<wbr>Time<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration during which duplicates can be detected.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enablebatchedoperations_nodejs">
<a href="#enablebatchedoperations_nodejs" style="color: inherit; text-decoration: inherit;">enable<wbr>Batched<wbr>Operations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls if server-side batched operations are enabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enableexpress_nodejs">
<a href="#enableexpress_nodejs" style="color: inherit; text-decoration: inherit;">enable<wbr>Express</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether Express Entities are enabled. An express topic holds a message in memory temporarily before writing it to persistent storage.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enablepartitioning_nodejs">
<a href="#enablepartitioning_nodejs" style="color: inherit; text-decoration: inherit;">enable<wbr>Partitioning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether to enable the topic to be partitioned across multiple message brokers.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="maxsizeinmegabytes_nodejs">
<a href="#maxsizeinmegabytes_nodejs" style="color: inherit; text-decoration: inherit;">max<wbr>Size<wbr>In<wbr>Megabytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Integer value which controls the size of memory allocated for the topic. For supported values see the "Queue/topic size" section of [this document](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-quotas).
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="namespacename_nodejs">
<a href="#namespacename_nodejs" style="color: inherit; text-decoration: inherit;">namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="requiresduplicatedetection_nodejs">
<a href="#requiresduplicatedetection_nodejs" style="color: inherit; text-decoration: inherit;">requires<wbr>Duplicate<wbr>Detection</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic requires duplicate detection.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="status_nodejs">
<a href="#status_nodejs" style="color: inherit; text-decoration: inherit;">status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Status of the Service Bus Topic. Acceptable values are Active or Disabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="supportordering_nodejs">
<a href="#supportordering_nodejs" style="color: inherit; text-decoration: inherit;">support<wbr>Ordering</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic supports ordering.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="auto_delete_on_idle_python">
<a href="#auto_delete_on_idle_python" style="color: inherit; text-decoration: inherit;">auto_<wbr>delete_<wbr>on_<wbr>idle</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of the idle interval after which the Topic is automatically deleted, minimum of 5 minutes.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="default_message_ttl_python">
<a href="#default_message_ttl_python" style="color: inherit; text-decoration: inherit;">default_<wbr>message_<wbr>ttl</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration of TTL of messages sent to this topic if no TTL value is set on the message itself.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="duplicate_detection_history_time_window_python">
<a href="#duplicate_detection_history_time_window_python" style="color: inherit; text-decoration: inherit;">duplicate_<wbr>detection_<wbr>history_<wbr>time_<wbr>window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ISO 8601 timespan duration during which duplicates can be detected.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enable_batched_operations_python">
<a href="#enable_batched_operations_python" style="color: inherit; text-decoration: inherit;">enable_<wbr>batched_<wbr>operations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls if server-side batched operations are enabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enable_express_python">
<a href="#enable_express_python" style="color: inherit; text-decoration: inherit;">enable_<wbr>express</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether Express Entities are enabled. An express topic holds a message in memory temporarily before writing it to persistent storage.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enable_partitioning_python">
<a href="#enable_partitioning_python" style="color: inherit; text-decoration: inherit;">enable_<wbr>partitioning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether to enable the topic to be partitioned across multiple message brokers.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="max_size_in_megabytes_python">
<a href="#max_size_in_megabytes_python" style="color: inherit; text-decoration: inherit;">max_<wbr>size_<wbr>in_<wbr>megabytes</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Integer value which controls the size of memory allocated for the topic. For supported values see the "Queue/topic size" section of [this document](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-quotas).
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="namespace_name_python">
<a href="#namespace_name_python" style="color: inherit; text-decoration: inherit;">namespace_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="requires_duplicate_detection_python">
<a href="#requires_duplicate_detection_python" style="color: inherit; text-decoration: inherit;">requires_<wbr>duplicate_<wbr>detection</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic requires duplicate detection.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="status_python">
<a href="#status_python" style="color: inherit; text-decoration: inherit;">status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Status of the Service Bus Topic. Acceptable values are Active or Disabled.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="support_ordering_python">
<a href="#support_ordering_python" style="color: inherit; text-decoration: inherit;">support_<wbr>ordering</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean flag which controls whether the Topic supports ordering.
{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure">https://github.com/pulumi/pulumi-azure</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`azurerm` Terraform Provider](https://github.com/terraform-providers/terraform-provider-azurerm).{{% /md %}}</dd>
</dl>

