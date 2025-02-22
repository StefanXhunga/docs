
---
title: "getSlotType"
title_tag: "aws.lex.getSlotType"
meta_desc: "Documentation for the aws.lex.getSlotType function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Provides details about a specific Amazon Lex Slot Type.


{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using Aws = Pulumi.Aws;

class MyStack : Stack
{
    public MyStack()
    {
        var flowerTypes = Output.Create(Aws.Lex.GetSlotType.InvokeAsync(new Aws.Lex.GetSlotTypeArgs
        {
            Name = "FlowerTypes",
            Version = "1",
        }));
    }

}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-aws/sdk/v3/go/aws/lex"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		opt0 := "1"
		_, err := lex.LookupSlotType(ctx, &lex.LookupSlotTypeArgs{
			Name:    "FlowerTypes",
			Version: &opt0,
		}, nil)
		if err != nil {
			return err
		}
		return nil
	})
}
```


{{< /example >}}


{{< example python >}}

```python
import pulumi
import pulumi_aws as aws

flower_types = aws.lex.get_slot_type(name="FlowerTypes",
    version="1")
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const flowerTypes = pulumi.output(aws.lex.getSlotType({
    name: "FlowerTypes",
    version: "1",
}, { async: true }));
```


{{< /example >}}





{{% /examples %}}




## Using getSlotType {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getSlotType<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetSlotTypeArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetSlotTypeResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_slot_type(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">version</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetSlotTypeResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupSlotType<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupSlotTypeArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupSlotTypeResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupSlotType` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetSlotType </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetSlotTypeResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetSlotTypeArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
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
    <dd>{{% md %}}The name of the slot type. The name is case sensitive.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="version_csharp">
<a href="#version_csharp" style="color: inherit; text-decoration: inherit;">Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
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
    <dd>{{% md %}}The name of the slot type. The name is case sensitive.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="version_go">
<a href="#version_go" style="color: inherit; text-decoration: inherit;">Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
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
    <dd>{{% md %}}The name of the slot type. The name is case sensitive.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="version_nodejs">
<a href="#version_nodejs" style="color: inherit; text-decoration: inherit;">version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
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
    <dd>{{% md %}}The name of the slot type. The name is case sensitive.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="version_python">
<a href="#version_python" style="color: inherit; text-decoration: inherit;">version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
{{% /md %}}</dd></dl>
{{% /choosable %}}




## getSlotType Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="checksum_csharp">
<a href="#checksum_csharp" style="color: inherit; text-decoration: inherit;">Checksum</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Checksum identifying the version of the slot type that was created. The checksum is
not included as an argument because the resource will add it automatically when updating the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="createddate_csharp">
<a href="#createddate_csharp" style="color: inherit; text-decoration: inherit;">Created<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The date when the slot type version was created.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_csharp">
<a href="#description_csharp" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A description of the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enumerationvalues_csharp">
<a href="#enumerationvalues_csharp" style="color: inherit; text-decoration: inherit;">Enumeration<wbr>Values</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getslottypeenumerationvalue">List&lt;Get<wbr>Slot<wbr>Type<wbr>Enumeration<wbr>Value&gt;</a></span>
    </dt>
    <dd>{{% md %}}A set of EnumerationValue objects that defines the values that
the slot type can take. Each value can have a set of synonyms, which are additional values that help
train the machine learning model about the values that it resolves for a slot.
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
        <span id="lastupdateddate_csharp">
<a href="#lastupdateddate_csharp" style="color: inherit; text-decoration: inherit;">Last<wbr>Updated<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The date when the $LATEST version of this slot type was updated.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the slot type. The name is not case sensitive.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="valueselectionstrategy_csharp">
<a href="#valueselectionstrategy_csharp" style="color: inherit; text-decoration: inherit;">Value<wbr>Selection<wbr>Strategy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Determines the slot resolution strategy that Amazon Lex
uses to return slot type values. `ORIGINAL_VALUE` returns the value entered by the user if the user
value is similar to the slot value. `TOP_RESOLUTION` returns the first value in the resolution list
if there is a resolution list for the slot, otherwise null is returned.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="version_csharp">
<a href="#version_csharp" style="color: inherit; text-decoration: inherit;">Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="checksum_go">
<a href="#checksum_go" style="color: inherit; text-decoration: inherit;">Checksum</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Checksum identifying the version of the slot type that was created. The checksum is
not included as an argument because the resource will add it automatically when updating the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="createddate_go">
<a href="#createddate_go" style="color: inherit; text-decoration: inherit;">Created<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The date when the slot type version was created.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_go">
<a href="#description_go" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A description of the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enumerationvalues_go">
<a href="#enumerationvalues_go" style="color: inherit; text-decoration: inherit;">Enumeration<wbr>Values</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getslottypeenumerationvalue">[]Get<wbr>Slot<wbr>Type<wbr>Enumeration<wbr>Value</a></span>
    </dt>
    <dd>{{% md %}}A set of EnumerationValue objects that defines the values that
the slot type can take. Each value can have a set of synonyms, which are additional values that help
train the machine learning model about the values that it resolves for a slot.
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
        <span id="lastupdateddate_go">
<a href="#lastupdateddate_go" style="color: inherit; text-decoration: inherit;">Last<wbr>Updated<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The date when the $LATEST version of this slot type was updated.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the slot type. The name is not case sensitive.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="valueselectionstrategy_go">
<a href="#valueselectionstrategy_go" style="color: inherit; text-decoration: inherit;">Value<wbr>Selection<wbr>Strategy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Determines the slot resolution strategy that Amazon Lex
uses to return slot type values. `ORIGINAL_VALUE` returns the value entered by the user if the user
value is similar to the slot value. `TOP_RESOLUTION` returns the first value in the resolution list
if there is a resolution list for the slot, otherwise null is returned.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="version_go">
<a href="#version_go" style="color: inherit; text-decoration: inherit;">Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="checksum_nodejs">
<a href="#checksum_nodejs" style="color: inherit; text-decoration: inherit;">checksum</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Checksum identifying the version of the slot type that was created. The checksum is
not included as an argument because the resource will add it automatically when updating the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="createddate_nodejs">
<a href="#createddate_nodejs" style="color: inherit; text-decoration: inherit;">created<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The date when the slot type version was created.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_nodejs">
<a href="#description_nodejs" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A description of the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enumerationvalues_nodejs">
<a href="#enumerationvalues_nodejs" style="color: inherit; text-decoration: inherit;">enumeration<wbr>Values</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getslottypeenumerationvalue">Get<wbr>Slot<wbr>Type<wbr>Enumeration<wbr>Value[]</a></span>
    </dt>
    <dd>{{% md %}}A set of EnumerationValue objects that defines the values that
the slot type can take. Each value can have a set of synonyms, which are additional values that help
train the machine learning model about the values that it resolves for a slot.
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
        <span id="lastupdateddate_nodejs">
<a href="#lastupdateddate_nodejs" style="color: inherit; text-decoration: inherit;">last<wbr>Updated<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The date when the $LATEST version of this slot type was updated.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the slot type. The name is not case sensitive.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="valueselectionstrategy_nodejs">
<a href="#valueselectionstrategy_nodejs" style="color: inherit; text-decoration: inherit;">value<wbr>Selection<wbr>Strategy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Determines the slot resolution strategy that Amazon Lex
uses to return slot type values. `ORIGINAL_VALUE` returns the value entered by the user if the user
value is similar to the slot value. `TOP_RESOLUTION` returns the first value in the resolution list
if there is a resolution list for the slot, otherwise null is returned.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="version_nodejs">
<a href="#version_nodejs" style="color: inherit; text-decoration: inherit;">version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="checksum_python">
<a href="#checksum_python" style="color: inherit; text-decoration: inherit;">checksum</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Checksum identifying the version of the slot type that was created. The checksum is
not included as an argument because the resource will add it automatically when updating the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="created_date_python">
<a href="#created_date_python" style="color: inherit; text-decoration: inherit;">created_<wbr>date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The date when the slot type version was created.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_python">
<a href="#description_python" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A description of the slot type.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enumeration_values_python">
<a href="#enumeration_values_python" style="color: inherit; text-decoration: inherit;">enumeration_<wbr>values</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getslottypeenumerationvalue">Sequence[Get<wbr>Slot<wbr>Type<wbr>Enumeration<wbr>Value]</a></span>
    </dt>
    <dd>{{% md %}}A set of EnumerationValue objects that defines the values that
the slot type can take. Each value can have a set of synonyms, which are additional values that help
train the machine learning model about the values that it resolves for a slot.
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
        <span id="last_updated_date_python">
<a href="#last_updated_date_python" style="color: inherit; text-decoration: inherit;">last_<wbr>updated_<wbr>date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The date when the $LATEST version of this slot type was updated.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the slot type. The name is not case sensitive.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="value_selection_strategy_python">
<a href="#value_selection_strategy_python" style="color: inherit; text-decoration: inherit;">value_<wbr>selection_<wbr>strategy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Determines the slot resolution strategy that Amazon Lex
uses to return slot type values. `ORIGINAL_VALUE` returns the value entered by the user if the user
value is similar to the slot value. `TOP_RESOLUTION` returns the first value in the resolution list
if there is a resolution list for the slot, otherwise null is returned.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="version_python">
<a href="#version_python" style="color: inherit; text-decoration: inherit;">version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The version of the slot type.
{{% /md %}}</dd></dl>
{{% /choosable %}}




## Supporting Types


<h4 id="getslottypeenumerationvalue">Get<wbr>Slot<wbr>Type<wbr>Enumeration<wbr>Value</h4>



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="synonyms_csharp">
<a href="#synonyms_csharp" style="color: inherit; text-decoration: inherit;">Synonyms</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="value_csharp">
<a href="#value_csharp" style="color: inherit; text-decoration: inherit;">Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="synonyms_go">
<a href="#synonyms_go" style="color: inherit; text-decoration: inherit;">Synonyms</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="value_go">
<a href="#value_go" style="color: inherit; text-decoration: inherit;">Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="synonyms_nodejs">
<a href="#synonyms_nodejs" style="color: inherit; text-decoration: inherit;">synonyms</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="value_nodejs">
<a href="#value_nodejs" style="color: inherit; text-decoration: inherit;">value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="synonyms_python">
<a href="#synonyms_python" style="color: inherit; text-decoration: inherit;">synonyms</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Sequence[str]</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="value_python">
<a href="#value_python" style="color: inherit; text-decoration: inherit;">value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-aws">https://github.com/pulumi/pulumi-aws</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`aws` Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws).{{% /md %}}</dd>
</dl>

