
---
title: "Secret"
title_tag: "azure-native.devtestlab.Secret"
meta_desc: "Documentation for the azure-native.devtestlab.Secret resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

A secret.
API Version: 2018-09-15.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}


### Secrets_CreateOrUpdate


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var secret = new AzureNative.DevTestLab.Secret("secret", new AzureNative.DevTestLab.SecretArgs
        {
            LabName = "{labName}",
            Name = "{secretName}",
            ResourceGroupName = "resourceGroupName",
            UserName = "{userName}",
            Value = "{secret}",
        });
    }

}

```


{{< /example >}}


{{< example go >}}


```go
package main

import (
	devtestlab "github.com/pulumi/pulumi-azure-native/sdk/go/azure/devtestlab"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := devtestlab.NewSecret(ctx, "secret", &devtestlab.SecretArgs{
			LabName:           pulumi.String("{labName}"),
			Name:              pulumi.String("{secretName}"),
			ResourceGroupName: pulumi.String("resourceGroupName"),
			UserName:          pulumi.String("{userName}"),
			Value:             pulumi.String("{secret}"),
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

secret = azure_native.devtestlab.Secret("secret",
    lab_name="{labName}",
    name="{secretName}",
    resource_group_name="resourceGroupName",
    user_name="{userName}",
    value="{secret}")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const secret = new azure_native.devtestlab.Secret("secret", {
    labName: "{labName}",
    name: "{secretName}",
    resourceGroupName: "resourceGroupName",
    userName: "{userName}",
    value: "{secret}",
});

```


{{< /example >}}





{{% /examples %}}




## Create a Secret Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">Secret</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">SecretArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">Secret</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">lab_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">location</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">tags</span><span class="p">:</span> <span class="nx">Optional[Mapping[str, str]]</span> = None<span class="p">, </span><span class="nx">user_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">value</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewSecret</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">SecretArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">Secret</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">Secret</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">SecretArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span class="property-type"><a href="#inputs">SecretArgs</a></span>
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
        <span class="property-type"><a href="#inputs">SecretArgs</a></span>
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
        <span class="property-type"><a href="#inputs">SecretArgs</a></span>
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

## Secret Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The Secret resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="labname_csharp">
<a href="#labname_csharp" style="color: inherit; text-decoration: inherit;">Lab<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the lab.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="username_csharp">
<a href="#username_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the user profile.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="location_csharp">
<a href="#location_csharp" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The location of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the secret.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_csharp">
<a href="#tags_csharp" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}The tags of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="value_csharp">
<a href="#value_csharp" style="color: inherit; text-decoration: inherit;">Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The value of the secret for secret creation.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="labname_go">
<a href="#labname_go" style="color: inherit; text-decoration: inherit;">Lab<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the lab.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="username_go">
<a href="#username_go" style="color: inherit; text-decoration: inherit;">User<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the user profile.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="location_go">
<a href="#location_go" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The location of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the secret.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_go">
<a href="#tags_go" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}The tags of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="value_go">
<a href="#value_go" style="color: inherit; text-decoration: inherit;">Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The value of the secret for secret creation.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="labname_nodejs">
<a href="#labname_nodejs" style="color: inherit; text-decoration: inherit;">lab<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the lab.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="username_nodejs">
<a href="#username_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the user profile.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="location_nodejs">
<a href="#location_nodejs" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The location of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the secret.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_nodejs">
<a href="#tags_nodejs" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}The tags of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="value_nodejs">
<a href="#value_nodejs" style="color: inherit; text-decoration: inherit;">value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The value of the secret for secret creation.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="lab_name_python">
<a href="#lab_name_python" style="color: inherit; text-decoration: inherit;">lab_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the lab.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="user_name_python">
<a href="#user_name_python" style="color: inherit; text-decoration: inherit;">user_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the user profile.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="location_python">
<a href="#location_python" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The location of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the secret.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_python">
<a href="#tags_python" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}The tags of the resource.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="value_python">
<a href="#value_python" style="color: inherit; text-decoration: inherit;">value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The value of the secret for secret creation.{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the Secret resource produces the following output properties:



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
        <span id="provisioningstate_csharp">
<a href="#provisioningstate_csharp" style="color: inherit; text-decoration: inherit;">Provisioning<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provisioning status of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="uniqueidentifier_csharp">
<a href="#uniqueidentifier_csharp" style="color: inherit; text-decoration: inherit;">Unique<wbr>Identifier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The unique immutable identifier of a resource (Guid).{{% /md %}}</dd></dl>
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
        <span id="provisioningstate_go">
<a href="#provisioningstate_go" style="color: inherit; text-decoration: inherit;">Provisioning<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provisioning status of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="uniqueidentifier_go">
<a href="#uniqueidentifier_go" style="color: inherit; text-decoration: inherit;">Unique<wbr>Identifier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The unique immutable identifier of a resource (Guid).{{% /md %}}</dd></dl>
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
        <span id="provisioningstate_nodejs">
<a href="#provisioningstate_nodejs" style="color: inherit; text-decoration: inherit;">provisioning<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provisioning status of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="uniqueidentifier_nodejs">
<a href="#uniqueidentifier_nodejs" style="color: inherit; text-decoration: inherit;">unique<wbr>Identifier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The unique immutable identifier of a resource (Guid).{{% /md %}}</dd></dl>
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
        <span id="provisioning_state_python">
<a href="#provisioning_state_python" style="color: inherit; text-decoration: inherit;">provisioning_<wbr>state</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provisioning status of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="unique_identifier_python">
<a href="#unique_identifier_python" style="color: inherit; text-decoration: inherit;">unique_<wbr>identifier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The unique immutable identifier of a resource (Guid).{{% /md %}}</dd></dl>
{{% /choosable %}}






## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:devtestlab:Secret {secretName} /subscriptions/{subscriptionId}/resourcegroups/resourceGroupName/providers/microsoft.devtestlab/labs/{labName}/users/{userName}/secrets/{secretName} 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

