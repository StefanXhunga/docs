
---
title: "ReplicationStorageClassificationMapping"
title_tag: "azure-native.recoveryservices.ReplicationStorageClassificationMapping"
meta_desc: "Documentation for the azure-native.recoveryservices.ReplicationStorageClassificationMapping resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Storage mapping object.
API Version: 2018-07-10.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}


### Create storage classification mapping.


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var replicationStorageClassificationMapping = new AzureNative.RecoveryServices.ReplicationStorageClassificationMapping("replicationStorageClassificationMapping", new AzureNative.RecoveryServices.ReplicationStorageClassificationMappingArgs
        {
            FabricName = "2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0",
            Properties = new AzureNative.RecoveryServices.Inputs.StorageMappingInputPropertiesArgs
            {
                TargetStorageClassificationId = "/Subscriptions/9112a37f-0f3e-46ec-9c00-060c6edca071/resourceGroups/resourceGroupPS1/providers/Microsoft.RecoveryServices/vaults/vault1/replicationFabrics/2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0/replicationStorageClassifications/8891569e-aaef-4a46-a4a0-78c14f2d7b09",
            },
            ResourceGroupName = "resourceGroupPS1",
            ResourceName = "vault1",
            StorageClassificationMappingName = "testStorageMapping",
            StorageClassificationName = "8891569e-aaef-4a46-a4a0-78c14f2d7b09",
        });
    }

}

```


{{< /example >}}


{{< example go >}}


```go
package main

import (
	recoveryservices "github.com/pulumi/pulumi-azure-native/sdk/go/azure/recoveryservices"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := recoveryservices.NewReplicationStorageClassificationMapping(ctx, "replicationStorageClassificationMapping", &recoveryservices.ReplicationStorageClassificationMappingArgs{
			FabricName: pulumi.String("2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0"),
			Properties: &recoveryservices.StorageMappingInputPropertiesArgs{
				TargetStorageClassificationId: pulumi.String("/Subscriptions/9112a37f-0f3e-46ec-9c00-060c6edca071/resourceGroups/resourceGroupPS1/providers/Microsoft.RecoveryServices/vaults/vault1/replicationFabrics/2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0/replicationStorageClassifications/8891569e-aaef-4a46-a4a0-78c14f2d7b09"),
			},
			ResourceGroupName:                pulumi.String("resourceGroupPS1"),
			ResourceName:                     pulumi.String("vault1"),
			StorageClassificationMappingName: pulumi.String("testStorageMapping"),
			StorageClassificationName:        pulumi.String("8891569e-aaef-4a46-a4a0-78c14f2d7b09"),
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

replication_storage_classification_mapping = azure_native.recoveryservices.ReplicationStorageClassificationMapping("replicationStorageClassificationMapping",
    fabric_name="2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0",
    properties=azure_native.recoveryservices.StorageMappingInputPropertiesArgs(
        target_storage_classification_id="/Subscriptions/9112a37f-0f3e-46ec-9c00-060c6edca071/resourceGroups/resourceGroupPS1/providers/Microsoft.RecoveryServices/vaults/vault1/replicationFabrics/2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0/replicationStorageClassifications/8891569e-aaef-4a46-a4a0-78c14f2d7b09",
    ),
    resource_group_name="resourceGroupPS1",
    resource_name="vault1",
    storage_classification_mapping_name="testStorageMapping",
    storage_classification_name="8891569e-aaef-4a46-a4a0-78c14f2d7b09")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const replicationStorageClassificationMapping = new azure_native.recoveryservices.ReplicationStorageClassificationMapping("replicationStorageClassificationMapping", {
    fabricName: "2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0",
    properties: {
        targetStorageClassificationId: "/Subscriptions/9112a37f-0f3e-46ec-9c00-060c6edca071/resourceGroups/resourceGroupPS1/providers/Microsoft.RecoveryServices/vaults/vault1/replicationFabrics/2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0/replicationStorageClassifications/8891569e-aaef-4a46-a4a0-78c14f2d7b09",
    },
    resourceGroupName: "resourceGroupPS1",
    resourceName: "vault1",
    storageClassificationMappingName: "testStorageMapping",
    storageClassificationName: "8891569e-aaef-4a46-a4a0-78c14f2d7b09",
});

```


{{< /example >}}





{{% /examples %}}




## Create a ReplicationStorageClassificationMapping Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">ReplicationStorageClassificationMapping</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">ReplicationStorageClassificationMappingArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">ReplicationStorageClassificationMapping</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">fabric_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">properties</span><span class="p">:</span> <span class="nx">Optional[StorageMappingInputPropertiesArgs]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_name_</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">storage_classification_mapping_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">storage_classification_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewReplicationStorageClassificationMapping</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">ReplicationStorageClassificationMappingArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">ReplicationStorageClassificationMapping</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">ReplicationStorageClassificationMapping</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">ReplicationStorageClassificationMappingArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span class="property-type"><a href="#inputs">ReplicationStorageClassificationMappingArgs</a></span>
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
        <span class="property-type"><a href="#inputs">ReplicationStorageClassificationMappingArgs</a></span>
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
        <span class="property-type"><a href="#inputs">ReplicationStorageClassificationMappingArgs</a></span>
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

## ReplicationStorageClassificationMapping Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The ReplicationStorageClassificationMapping resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="fabricname_csharp">
<a href="#fabricname_csharp" style="color: inherit; text-decoration: inherit;">Fabric<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Fabric name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group where the recovery services vault is present.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcename_csharp">
<a href="#resourcename_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the recovery services vault.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="storageclassificationname_csharp">
<a href="#storageclassificationname_csharp" style="color: inherit; text-decoration: inherit;">Storage<wbr>Classification<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Storage classification name.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="properties_csharp">
<a href="#properties_csharp" style="color: inherit; text-decoration: inherit;">Properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#storagemappinginputproperties">Pulumi.<wbr>Azure<wbr>Native.<wbr>Recovery<wbr>Services.<wbr>Inputs.<wbr>Storage<wbr>Mapping<wbr>Input<wbr>Properties<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Storage mapping input properties.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="storageclassificationmappingname_csharp">
<a href="#storageclassificationmappingname_csharp" style="color: inherit; text-decoration: inherit;">Storage<wbr>Classification<wbr>Mapping<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Storage classification mapping name.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="fabricname_go">
<a href="#fabricname_go" style="color: inherit; text-decoration: inherit;">Fabric<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Fabric name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group where the recovery services vault is present.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcename_go">
<a href="#resourcename_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the recovery services vault.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="storageclassificationname_go">
<a href="#storageclassificationname_go" style="color: inherit; text-decoration: inherit;">Storage<wbr>Classification<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Storage classification name.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="properties_go">
<a href="#properties_go" style="color: inherit; text-decoration: inherit;">Properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#storagemappinginputproperties">Storage<wbr>Mapping<wbr>Input<wbr>Properties</a></span>
    </dt>
    <dd>{{% md %}}Storage mapping input properties.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="storageclassificationmappingname_go">
<a href="#storageclassificationmappingname_go" style="color: inherit; text-decoration: inherit;">Storage<wbr>Classification<wbr>Mapping<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Storage classification mapping name.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="fabricname_nodejs">
<a href="#fabricname_nodejs" style="color: inherit; text-decoration: inherit;">fabric<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Fabric name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group where the recovery services vault is present.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcename_nodejs">
<a href="#resourcename_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the recovery services vault.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="storageclassificationname_nodejs">
<a href="#storageclassificationname_nodejs" style="color: inherit; text-decoration: inherit;">storage<wbr>Classification<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Storage classification name.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="properties_nodejs">
<a href="#properties_nodejs" style="color: inherit; text-decoration: inherit;">properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#storagemappinginputproperties">Storage<wbr>Mapping<wbr>Input<wbr>Properties</a></span>
    </dt>
    <dd>{{% md %}}Storage mapping input properties.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="storageclassificationmappingname_nodejs">
<a href="#storageclassificationmappingname_nodejs" style="color: inherit; text-decoration: inherit;">storage<wbr>Classification<wbr>Mapping<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Storage classification mapping name.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="fabric_name_python">
<a href="#fabric_name_python" style="color: inherit; text-decoration: inherit;">fabric_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Fabric name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group where the recovery services vault is present.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_name_python">
<a href="#resource_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the recovery services vault.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="storage_classification_name_python">
<a href="#storage_classification_name_python" style="color: inherit; text-decoration: inherit;">storage_<wbr>classification_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Storage classification name.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="properties_python">
<a href="#properties_python" style="color: inherit; text-decoration: inherit;">properties</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#storagemappinginputproperties">Storage<wbr>Mapping<wbr>Input<wbr>Properties<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Storage mapping input properties.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="storage_classification_mapping_name_python">
<a href="#storage_classification_mapping_name_python" style="color: inherit; text-decoration: inherit;">storage_<wbr>classification_<wbr>mapping_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Storage classification mapping name.{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the ReplicationStorageClassificationMapping resource produces the following output properties:



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
    <dd>{{% md %}}Resource Name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="location_csharp">
<a href="#location_csharp" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Location{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}Resource Name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="location_go">
<a href="#location_go" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Location{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}Resource Name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="location_nodejs">
<a href="#location_nodejs" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Location{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}Resource Name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource Type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="location_python">
<a href="#location_python" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource Location{{% /md %}}</dd></dl>
{{% /choosable %}}







## Supporting Types



<h4 id="storageclassificationmappingpropertiesresponse">Storage<wbr>Classification<wbr>Mapping<wbr>Properties<wbr>Response</h4>

{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="targetstorageclassificationid_csharp">
<a href="#targetstorageclassificationid_csharp" style="color: inherit; text-decoration: inherit;">Target<wbr>Storage<wbr>Classification<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Target storage object Id.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="targetstorageclassificationid_go">
<a href="#targetstorageclassificationid_go" style="color: inherit; text-decoration: inherit;">Target<wbr>Storage<wbr>Classification<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Target storage object Id.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="targetstorageclassificationid_nodejs">
<a href="#targetstorageclassificationid_nodejs" style="color: inherit; text-decoration: inherit;">target<wbr>Storage<wbr>Classification<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Target storage object Id.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="target_storage_classification_id_python">
<a href="#target_storage_classification_id_python" style="color: inherit; text-decoration: inherit;">target_<wbr>storage_<wbr>classification_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Target storage object Id.{{% /md %}}</dd></dl>
{{% /choosable %}}

<h4 id="storagemappinginputproperties">Storage<wbr>Mapping<wbr>Input<wbr>Properties</h4>

{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="targetstorageclassificationid_csharp">
<a href="#targetstorageclassificationid_csharp" style="color: inherit; text-decoration: inherit;">Target<wbr>Storage<wbr>Classification<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the storage object.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="targetstorageclassificationid_go">
<a href="#targetstorageclassificationid_go" style="color: inherit; text-decoration: inherit;">Target<wbr>Storage<wbr>Classification<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the storage object.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="targetstorageclassificationid_nodejs">
<a href="#targetstorageclassificationid_nodejs" style="color: inherit; text-decoration: inherit;">target<wbr>Storage<wbr>Classification<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the storage object.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="target_storage_classification_id_python">
<a href="#target_storage_classification_id_python" style="color: inherit; text-decoration: inherit;">target_<wbr>storage_<wbr>classification_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the storage object.{{% /md %}}</dd></dl>
{{% /choosable %}}
## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:recoveryservices:ReplicationStorageClassificationMapping testStorageMapping /Subscriptions/9112a37f-0f3e-46ec-9c00-060c6edca071/resourceGroups/resourceGroupPS1/providers/Microsoft.RecoveryServices/vaults/vault1/replicationFabrics/2a48e3770ac08aa2be8bfbd94fcfb1cbf2dcc487b78fb9d3bd778304441b06a0/replicationStorageClassifications/8891569e-aaef-4a46-a4a0-78c14f2d7b09/replicationStorageClassificationMappings/testStorageMapping 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

