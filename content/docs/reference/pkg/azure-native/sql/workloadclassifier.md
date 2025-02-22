
---
title: "WorkloadClassifier"
title_tag: "azure-native.sql.WorkloadClassifier"
meta_desc: "Documentation for the azure-native.sql.WorkloadClassifier resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Workload classifier operations for a data warehouse
API Version: 2020-11-01-preview.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}


### Create a workload group with all properties specified.


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var workloadClassifier = new AzureNative.Sql.WorkloadClassifier("workloadClassifier", new AzureNative.Sql.WorkloadClassifierArgs
        {
            Context = "test_context",
            DatabaseName = "testdb",
            EndTime = "14:00",
            Importance = "high",
            Label = "test_label",
            MemberName = "dbo",
            ResourceGroupName = "Default-SQL-SouthEastAsia",
            ServerName = "testsvr",
            StartTime = "12:00",
            WorkloadClassifierName = "wlm_workloadclassifier",
            WorkloadGroupName = "wlm_workloadgroup",
        });
    }

}

```


{{< /example >}}


{{< example go >}}


```go
package main

import (
	sql "github.com/pulumi/pulumi-azure-native/sdk/go/azure/sql"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := sql.NewWorkloadClassifier(ctx, "workloadClassifier", &sql.WorkloadClassifierArgs{
			Context:                pulumi.String("test_context"),
			DatabaseName:           pulumi.String("testdb"),
			EndTime:                pulumi.String("14:00"),
			Importance:             pulumi.String("high"),
			Label:                  pulumi.String("test_label"),
			MemberName:             pulumi.String("dbo"),
			ResourceGroupName:      pulumi.String("Default-SQL-SouthEastAsia"),
			ServerName:             pulumi.String("testsvr"),
			StartTime:              pulumi.String("12:00"),
			WorkloadClassifierName: pulumi.String("wlm_workloadclassifier"),
			WorkloadGroupName:      pulumi.String("wlm_workloadgroup"),
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

workload_classifier = azure_native.sql.WorkloadClassifier("workloadClassifier",
    context="test_context",
    database_name="testdb",
    end_time="14:00",
    importance="high",
    label="test_label",
    member_name="dbo",
    resource_group_name="Default-SQL-SouthEastAsia",
    server_name="testsvr",
    start_time="12:00",
    workload_classifier_name="wlm_workloadclassifier",
    workload_group_name="wlm_workloadgroup")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const workloadClassifier = new azure_native.sql.WorkloadClassifier("workloadClassifier", {
    context: "test_context",
    databaseName: "testdb",
    endTime: "14:00",
    importance: "high",
    label: "test_label",
    memberName: "dbo",
    resourceGroupName: "Default-SQL-SouthEastAsia",
    serverName: "testsvr",
    startTime: "12:00",
    workloadClassifierName: "wlm_workloadclassifier",
    workloadGroupName: "wlm_workloadgroup",
});

```


{{< /example >}}




### Create a workload group with the required properties specified.


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var workloadClassifier = new AzureNative.Sql.WorkloadClassifier("workloadClassifier", new AzureNative.Sql.WorkloadClassifierArgs
        {
            DatabaseName = "testdb",
            MemberName = "dbo",
            ResourceGroupName = "Default-SQL-SouthEastAsia",
            ServerName = "testsvr",
            WorkloadClassifierName = "wlm_workloadclassifier",
            WorkloadGroupName = "wlm_workloadgroup",
        });
    }

}

```


{{< /example >}}


{{< example go >}}


```go
package main

import (
	sql "github.com/pulumi/pulumi-azure-native/sdk/go/azure/sql"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := sql.NewWorkloadClassifier(ctx, "workloadClassifier", &sql.WorkloadClassifierArgs{
			DatabaseName:           pulumi.String("testdb"),
			MemberName:             pulumi.String("dbo"),
			ResourceGroupName:      pulumi.String("Default-SQL-SouthEastAsia"),
			ServerName:             pulumi.String("testsvr"),
			WorkloadClassifierName: pulumi.String("wlm_workloadclassifier"),
			WorkloadGroupName:      pulumi.String("wlm_workloadgroup"),
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

workload_classifier = azure_native.sql.WorkloadClassifier("workloadClassifier",
    database_name="testdb",
    member_name="dbo",
    resource_group_name="Default-SQL-SouthEastAsia",
    server_name="testsvr",
    workload_classifier_name="wlm_workloadclassifier",
    workload_group_name="wlm_workloadgroup")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const workloadClassifier = new azure_native.sql.WorkloadClassifier("workloadClassifier", {
    databaseName: "testdb",
    memberName: "dbo",
    resourceGroupName: "Default-SQL-SouthEastAsia",
    serverName: "testsvr",
    workloadClassifierName: "wlm_workloadclassifier",
    workloadGroupName: "wlm_workloadgroup",
});

```


{{< /example >}}





{{% /examples %}}




## Create a WorkloadClassifier Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">WorkloadClassifier</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">WorkloadClassifierArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">WorkloadClassifier</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">context</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">database_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">end_time</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">importance</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">label</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">member_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">server_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">start_time</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">workload_classifier_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">workload_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewWorkloadClassifier</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">WorkloadClassifierArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">WorkloadClassifier</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">WorkloadClassifier</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">WorkloadClassifierArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span class="property-type"><a href="#inputs">WorkloadClassifierArgs</a></span>
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
        <span class="property-type"><a href="#inputs">WorkloadClassifierArgs</a></span>
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
        <span class="property-type"><a href="#inputs">WorkloadClassifierArgs</a></span>
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

## WorkloadClassifier Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The WorkloadClassifier resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="databasename_csharp">
<a href="#databasename_csharp" style="color: inherit; text-decoration: inherit;">Database<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the database.{{% /md %}}</dd><dt class="property-required"
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
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="servername_csharp">
<a href="#servername_csharp" style="color: inherit; text-decoration: inherit;">Server<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the server.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workloadgroupname_csharp">
<a href="#workloadgroupname_csharp" style="color: inherit; text-decoration: inherit;">Workload<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload group from which to receive the classifier from.{{% /md %}}</dd><dt class="property-optional"
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
    <dd>{{% md %}}The name of the workload classifier to create/update.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="databasename_go">
<a href="#databasename_go" style="color: inherit; text-decoration: inherit;">Database<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the database.{{% /md %}}</dd><dt class="property-required"
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
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="servername_go">
<a href="#servername_go" style="color: inherit; text-decoration: inherit;">Server<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the server.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workloadgroupname_go">
<a href="#workloadgroupname_go" style="color: inherit; text-decoration: inherit;">Workload<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload group from which to receive the classifier from.{{% /md %}}</dd><dt class="property-optional"
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
    <dd>{{% md %}}The name of the workload classifier to create/update.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="databasename_nodejs">
<a href="#databasename_nodejs" style="color: inherit; text-decoration: inherit;">database<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the database.{{% /md %}}</dd><dt class="property-required"
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
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="servername_nodejs">
<a href="#servername_nodejs" style="color: inherit; text-decoration: inherit;">server<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the server.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workloadgroupname_nodejs">
<a href="#workloadgroupname_nodejs" style="color: inherit; text-decoration: inherit;">workload<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the workload group from which to receive the classifier from.{{% /md %}}</dd><dt class="property-optional"
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
    <dd>{{% md %}}The name of the workload classifier to create/update.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="database_name_python">
<a href="#database_name_python" style="color: inherit; text-decoration: inherit;">database_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the database.{{% /md %}}</dd><dt class="property-required"
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
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="server_name_python">
<a href="#server_name_python" style="color: inherit; text-decoration: inherit;">server_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the server.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="workload_group_name_python">
<a href="#workload_group_name_python" style="color: inherit; text-decoration: inherit;">workload_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the workload group from which to receive the classifier from.{{% /md %}}</dd><dt class="property-optional"
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
    <dd>{{% md %}}The name of the workload classifier to create/update.{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the WorkloadClassifier resource produces the following output properties:



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
    <dd>{{% md %}}Resource name.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}Resource name.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}Resource name.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}Resource name.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd></dl>
{{% /choosable %}}






## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:sql:WorkloadClassifier wlm_workloadclassifier /subscriptions/00000000-1111-2222-3333-444444444444/resourceGroups/Default-SQL-SouthEastAsia/providers/Microsoft.Sql/servers/testsvr/databases/testdb/workloadGroups/wlm_workloadgroup/workloadClassifiers/wlm_workloadclassifier 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

