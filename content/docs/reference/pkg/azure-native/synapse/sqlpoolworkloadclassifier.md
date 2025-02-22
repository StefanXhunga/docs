
---
title: "SqlPoolWorkloadClassifier"
title_tag: "azure-native.synapse.SqlPoolWorkloadClassifier"
meta_desc: "Documentation for the azure-native.synapse.SqlPoolWorkloadClassifier resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Workload classifier operations for a data warehouse
API Version: 2021-03-01.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}


### Create a workload classifier with all properties specified.


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var sqlPoolWorkloadClassifier = new AzureNative.Synapse.SqlPoolWorkloadClassifier("sqlPoolWorkloadClassifier", new AzureNative.Synapse.SqlPoolWorkloadClassifierArgs
        {
            Context = "test_context",
            EndTime = "14:00",
            Importance = "high",
            Label = "test_label",
            MemberName = "dbo",
            ResourceGroupName = "sqlcrudtest-6852",
            SqlPoolName = "sqlcrudtest-9187",
            StartTime = "12:00",
            WorkloadClassifierName = "wlm_workloadclassifier",
            WorkloadGroupName = "wlm_workloadgroup",
            WorkspaceName = "sqlcrudtest-2080",
        });
    }

}

```


{{< /example >}}


{{< example go >}}


```go
package main

import (
	synapse "github.com/pulumi/pulumi-azure-native/sdk/go/azure/synapse"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := synapse.NewSqlPoolWorkloadClassifier(ctx, "sqlPoolWorkloadClassifier", &synapse.SqlPoolWorkloadClassifierArgs{
			Context:                pulumi.String("test_context"),
			EndTime:                pulumi.String("14:00"),
			Importance:             pulumi.String("high"),
			Label:                  pulumi.String("test_label"),
			MemberName:             pulumi.String("dbo"),
			ResourceGroupName:      pulumi.String("sqlcrudtest-6852"),
			SqlPoolName:            pulumi.String("sqlcrudtest-9187"),
			StartTime:              pulumi.String("12:00"),
			WorkloadClassifierName: pulumi.String("wlm_workloadclassifier"),
			WorkloadGroupName:      pulumi.String("wlm_workloadgroup"),
			WorkspaceName:          pulumi.String("sqlcrudtest-2080"),
		})
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
import pulumi_azure_native as azure_native

sql_pool_workload_classifier = azure_native.synapse.SqlPoolWorkloadClassifier("sqlPoolWorkloadClassifier",
    context="test_context",
    end_time="14:00",
    importance="high",
    label="test_label",
    member_name="dbo",
    resource_group_name="sqlcrudtest-6852",
    sql_pool_name="sqlcrudtest-9187",
    start_time="12:00",
    workload_classifier_name="wlm_workloadclassifier",
    workload_group_name="wlm_workloadgroup",
    workspace_name="sqlcrudtest-2080")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const sqlPoolWorkloadClassifier = new azure_native.synapse.SqlPoolWorkloadClassifier("sqlPoolWorkloadClassifier", {
    context: "test_context",
    endTime: "14:00",
    importance: "high",
    label: "test_label",
    memberName: "dbo",
    resourceGroupName: "sqlcrudtest-6852",
    sqlPoolName: "sqlcrudtest-9187",
    startTime: "12:00",
    workloadClassifierName: "wlm_workloadclassifier",
    workloadGroupName: "wlm_workloadgroup",
    workspaceName: "sqlcrudtest-2080",
});

```


{{< /example >}}




### Create a workload classifier with the required properties specified.


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var sqlPoolWorkloadClassifier = new AzureNative.Synapse.SqlPoolWorkloadClassifier("sqlPoolWorkloadClassifier", new AzureNative.Synapse.SqlPoolWorkloadClassifierArgs
        {
            MemberName = "dbo",
            ResourceGroupName = "sqlcrudtest-6852",
            SqlPoolName = "sqlcrudtest-9187",
            WorkloadClassifierName = "wlm_workloadclassifier",
            WorkloadGroupName = "wlm_workloadgroup",
            WorkspaceName = "sqlcrudtest-2080",
        });
    }

}

```


{{< /example >}}


{{< example go >}}


```go
package main

import (
	synapse "github.com/pulumi/pulumi-azure-native/sdk/go/azure/synapse"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := synapse.NewSqlPoolWorkloadClassifier(ctx, "sqlPoolWorkloadClassifier", &synapse.SqlPoolWorkloadClassifierArgs{
			MemberName:             pulumi.String("dbo"),
			ResourceGroupName:      pulumi.String("sqlcrudtest-6852"),
			SqlPoolName:            pulumi.String("sqlcrudtest-9187"),
			WorkloadClassifierName: pulumi.String("wlm_workloadclassifier"),
			WorkloadGroupName:      pulumi.String("wlm_workloadgroup"),
			WorkspaceName:          pulumi.String("sqlcrudtest-2080"),
		})
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
import pulumi_azure_native as azure_native

sql_pool_workload_classifier = azure_native.synapse.SqlPoolWorkloadClassifier("sqlPoolWorkloadClassifier",
    member_name="dbo",
    resource_group_name="sqlcrudtest-6852",
    sql_pool_name="sqlcrudtest-9187",
    workload_classifier_name="wlm_workloadclassifier",
    workload_group_name="wlm_workloadgroup",
    workspace_name="sqlcrudtest-2080")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const sqlPoolWorkloadClassifier = new azure_native.synapse.SqlPoolWorkloadClassifier("sqlPoolWorkloadClassifier", {
    memberName: "dbo",
    resourceGroupName: "sqlcrudtest-6852",
    sqlPoolName: "sqlcrudtest-9187",
    workloadClassifierName: "wlm_workloadclassifier",
    workloadGroupName: "wlm_workloadgroup",
    workspaceName: "sqlcrudtest-2080",
});

```


{{< /example >}}





{{% /examples %}}




## Create a SqlPoolWorkloadClassifier Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">SqlPoolWorkloadClassifier</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">SqlPoolWorkloadClassifierArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">SqlPoolWorkloadClassifier</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">context</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">end_time</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">importance</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">label</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">member_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">sql_pool_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">start_time</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">workload_classifier_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">workload_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">workspace_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewSqlPoolWorkloadClassifier</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">SqlPoolWorkloadClassifierArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">SqlPoolWorkloadClassifier</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">SqlPoolWorkloadClassifier</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">SqlPoolWorkloadClassifierArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">SqlPoolWorkloadClassifierArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd></dl>

{{% /choosable %}}

{{% choosable language python %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type">
            <a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a>
        </span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties"><dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>
      Context object for the current deployment.
    </dd><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">SqlPoolWorkloadClassifierArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd></dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">SqlPoolWorkloadClassifierArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd></dl>

{{% /choosable %}}

## SqlPoolWorkloadClassifier Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The SqlPoolWorkloadClassifier resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="membername_csharp">
<a href="#membername_csharp" style="color: inherit; text-decoration: inherit;">Member<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier member name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sqlpoolname_csharp">
<a href="#sqlpoolname_csharp" style="color: inherit; text-decoration: inherit;">Sql<wbr>Pool<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}SQL pool name{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workloadgroupname_csharp">
<a href="#workloadgroupname_csharp" style="color: inherit; text-decoration: inherit;">Workload<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workspacename_csharp">
<a href="#workspacename_csharp" style="color: inherit; text-decoration: inherit;">Workspace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workspace{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="context_csharp">
<a href="#context_csharp" style="color: inherit; text-decoration: inherit;">Context</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier context.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="endtime_csharp">
<a href="#endtime_csharp" style="color: inherit; text-decoration: inherit;">End<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier end time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="importance_csharp">
<a href="#importance_csharp" style="color: inherit; text-decoration: inherit;">Importance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier importance.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="label_csharp">
<a href="#label_csharp" style="color: inherit; text-decoration: inherit;">Label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier label.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="starttime_csharp">
<a href="#starttime_csharp" style="color: inherit; text-decoration: inherit;">Start<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier start time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="workloadclassifiername_csharp">
<a href="#workloadclassifiername_csharp" style="color: inherit; text-decoration: inherit;">Workload<wbr>Classifier<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload classifier.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="membername_go">
<a href="#membername_go" style="color: inherit; text-decoration: inherit;">Member<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier member name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sqlpoolname_go">
<a href="#sqlpoolname_go" style="color: inherit; text-decoration: inherit;">Sql<wbr>Pool<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}SQL pool name{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workloadgroupname_go">
<a href="#workloadgroupname_go" style="color: inherit; text-decoration: inherit;">Workload<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workspacename_go">
<a href="#workspacename_go" style="color: inherit; text-decoration: inherit;">Workspace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workspace{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="context_go">
<a href="#context_go" style="color: inherit; text-decoration: inherit;">Context</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier context.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="endtime_go">
<a href="#endtime_go" style="color: inherit; text-decoration: inherit;">End<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier end time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="importance_go">
<a href="#importance_go" style="color: inherit; text-decoration: inherit;">Importance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier importance.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="label_go">
<a href="#label_go" style="color: inherit; text-decoration: inherit;">Label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier label.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="starttime_go">
<a href="#starttime_go" style="color: inherit; text-decoration: inherit;">Start<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier start time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="workloadclassifiername_go">
<a href="#workloadclassifiername_go" style="color: inherit; text-decoration: inherit;">Workload<wbr>Classifier<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload classifier.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="membername_nodejs">
<a href="#membername_nodejs" style="color: inherit; text-decoration: inherit;">member<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier member name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sqlpoolname_nodejs">
<a href="#sqlpoolname_nodejs" style="color: inherit; text-decoration: inherit;">sql<wbr>Pool<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}SQL pool name{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workloadgroupname_nodejs">
<a href="#workloadgroupname_nodejs" style="color: inherit; text-decoration: inherit;">workload<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workspacename_nodejs">
<a href="#workspacename_nodejs" style="color: inherit; text-decoration: inherit;">workspace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workspace{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="context_nodejs">
<a href="#context_nodejs" style="color: inherit; text-decoration: inherit;">context</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier context.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="endtime_nodejs">
<a href="#endtime_nodejs" style="color: inherit; text-decoration: inherit;">end<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier end time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="importance_nodejs">
<a href="#importance_nodejs" style="color: inherit; text-decoration: inherit;">importance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier importance.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="label_nodejs">
<a href="#label_nodejs" style="color: inherit; text-decoration: inherit;">label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier label.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="starttime_nodejs">
<a href="#starttime_nodejs" style="color: inherit; text-decoration: inherit;">start<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The workload classifier start time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="workloadclassifiername_nodejs">
<a href="#workloadclassifiername_nodejs" style="color: inherit; text-decoration: inherit;">workload<wbr>Classifier<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload classifier.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="member_name_python">
<a href="#member_name_python" style="color: inherit; text-decoration: inherit;">member_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The workload classifier member name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sql_pool_name_python">
<a href="#sql_pool_name_python" style="color: inherit; text-decoration: inherit;">sql_<wbr>pool_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SQL pool name{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workload_group_name_python">
<a href="#workload_group_name_python" style="color: inherit; text-decoration: inherit;">workload_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the workload group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workspace_name_python">
<a href="#workspace_name_python" style="color: inherit; text-decoration: inherit;">workspace_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the workspace{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="context_python">
<a href="#context_python" style="color: inherit; text-decoration: inherit;">context</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The workload classifier context.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="end_time_python">
<a href="#end_time_python" style="color: inherit; text-decoration: inherit;">end_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The workload classifier end time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="importance_python">
<a href="#importance_python" style="color: inherit; text-decoration: inherit;">importance</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The workload classifier importance.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="label_python">
<a href="#label_python" style="color: inherit; text-decoration: inherit;">label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The workload classifier label.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="start_time_python">
<a href="#start_time_python" style="color: inherit; text-decoration: inherit;">start_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The workload classifier start time for classification.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="workload_classifier_name_python">
<a href="#workload_classifier_name_python" style="color: inherit; text-decoration: inherit;">workload_<wbr>classifier_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the workload classifier.{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the SqlPoolWorkloadClassifier resource produces the following output properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or "Microsoft.Storage/storageAccounts"{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or "Microsoft.Storage/storageAccounts"{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or "Microsoft.Storage/storageAccounts"{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or "Microsoft.Storage/storageAccounts"{{% /md %}}</dd></dl>
{{% /choosable %}}






## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:synapse:SqlPoolWorkloadClassifier wlm_workloadclassifier /subscriptions/00000000-1111-2222-3333-444444444444/resourceGroups/sqlcrudtest-6852/providers/Microsoft.Synapse/workspaces/sqlcrudtest-2080/sqlPools/sqlcrudtest-9187/workloadGroups/wlm_workloadgroup/workloadClassifiers/wlm_workloadclassifier 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

