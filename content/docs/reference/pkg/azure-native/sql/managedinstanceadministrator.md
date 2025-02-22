
---
title: "ManagedInstanceAdministrator"
title_tag: "azure-native.sql.ManagedInstanceAdministrator"
meta_desc: "Documentation for the azure-native.sql.ManagedInstanceAdministrator resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

An Azure SQL managed instance administrator.
API Version: 2020-11-01-preview.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}


### Create administrator of managed instance


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var managedInstanceAdministrator = new AzureNative.Sql.ManagedInstanceAdministrator("managedInstanceAdministrator", new AzureNative.Sql.ManagedInstanceAdministratorArgs
        {
            AdministratorName = "ActiveDirectory",
            AdministratorType = "ActiveDirectory",
            Login = "bob@contoso.com",
            ManagedInstanceName = "managedInstance",
            ResourceGroupName = "Default-SQL-SouthEastAsia",
            Sid = "44444444-3333-2222-1111-000000000000",
            TenantId = "55555555-4444-3333-2222-111111111111",
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
		_, err := sql.NewManagedInstanceAdministrator(ctx, "managedInstanceAdministrator", &sql.ManagedInstanceAdministratorArgs{
			AdministratorName:   pulumi.String("ActiveDirectory"),
			AdministratorType:   pulumi.String("ActiveDirectory"),
			Login:               pulumi.String("bob@contoso.com"),
			ManagedInstanceName: pulumi.String("managedInstance"),
			ResourceGroupName:   pulumi.String("Default-SQL-SouthEastAsia"),
			Sid:                 pulumi.String("44444444-3333-2222-1111-000000000000"),
			TenantId:            pulumi.String("55555555-4444-3333-2222-111111111111"),
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

managed_instance_administrator = azure_native.sql.ManagedInstanceAdministrator("managedInstanceAdministrator",
    administrator_name="ActiveDirectory",
    administrator_type="ActiveDirectory",
    login="bob@contoso.com",
    managed_instance_name="managedInstance",
    resource_group_name="Default-SQL-SouthEastAsia",
    sid="44444444-3333-2222-1111-000000000000",
    tenant_id="55555555-4444-3333-2222-111111111111")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const managedInstanceAdministrator = new azure_native.sql.ManagedInstanceAdministrator("managedInstanceAdministrator", {
    administratorName: "ActiveDirectory",
    administratorType: "ActiveDirectory",
    login: "bob@contoso.com",
    managedInstanceName: "managedInstance",
    resourceGroupName: "Default-SQL-SouthEastAsia",
    sid: "44444444-3333-2222-1111-000000000000",
    tenantId: "55555555-4444-3333-2222-111111111111",
});

```


{{< /example >}}




### Update administrator of managed instance


{{< example csharp >}}

```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var managedInstanceAdministrator = new AzureNative.Sql.ManagedInstanceAdministrator("managedInstanceAdministrator", new AzureNative.Sql.ManagedInstanceAdministratorArgs
        {
            AdministratorName = "ActiveDirectory",
            AdministratorType = "ActiveDirectory",
            Login = "bob@contoso.com",
            ManagedInstanceName = "managedInstance",
            ResourceGroupName = "Default-SQL-SouthEastAsia",
            Sid = "44444444-3333-2222-1111-000000000000",
            TenantId = "55555555-4444-3333-2222-111111111111",
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
		_, err := sql.NewManagedInstanceAdministrator(ctx, "managedInstanceAdministrator", &sql.ManagedInstanceAdministratorArgs{
			AdministratorName:   pulumi.String("ActiveDirectory"),
			AdministratorType:   pulumi.String("ActiveDirectory"),
			Login:               pulumi.String("bob@contoso.com"),
			ManagedInstanceName: pulumi.String("managedInstance"),
			ResourceGroupName:   pulumi.String("Default-SQL-SouthEastAsia"),
			Sid:                 pulumi.String("44444444-3333-2222-1111-000000000000"),
			TenantId:            pulumi.String("55555555-4444-3333-2222-111111111111"),
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

managed_instance_administrator = azure_native.sql.ManagedInstanceAdministrator("managedInstanceAdministrator",
    administrator_name="ActiveDirectory",
    administrator_type="ActiveDirectory",
    login="bob@contoso.com",
    managed_instance_name="managedInstance",
    resource_group_name="Default-SQL-SouthEastAsia",
    sid="44444444-3333-2222-1111-000000000000",
    tenant_id="55555555-4444-3333-2222-111111111111")

```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const managedInstanceAdministrator = new azure_native.sql.ManagedInstanceAdministrator("managedInstanceAdministrator", {
    administratorName: "ActiveDirectory",
    administratorType: "ActiveDirectory",
    login: "bob@contoso.com",
    managedInstanceName: "managedInstance",
    resourceGroupName: "Default-SQL-SouthEastAsia",
    sid: "44444444-3333-2222-1111-000000000000",
    tenantId: "55555555-4444-3333-2222-111111111111",
});

```


{{< /example >}}





{{% /examples %}}




## Create a ManagedInstanceAdministrator Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">ManagedInstanceAdministrator</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">ManagedInstanceAdministratorArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">ManagedInstanceAdministrator</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">administrator_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">administrator_type</span><span class="p">:</span> <span class="nx">Optional[Union[str, ManagedInstanceAdministratorType]]</span> = None<span class="p">, </span><span class="nx">login</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">managed_instance_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">sid</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">tenant_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewManagedInstanceAdministrator</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">ManagedInstanceAdministratorArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">ManagedInstanceAdministrator</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">ManagedInstanceAdministrator</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">ManagedInstanceAdministratorArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span class="property-type"><a href="#inputs">ManagedInstanceAdministratorArgs</a></span>
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
        <span class="property-type"><a href="#inputs">ManagedInstanceAdministratorArgs</a></span>
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
        <span class="property-type"><a href="#inputs">ManagedInstanceAdministratorArgs</a></span>
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

## ManagedInstanceAdministrator Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The ManagedInstanceAdministrator resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="administratortype_csharp">
<a href="#administratortype_csharp" style="color: inherit; text-decoration: inherit;">Administrator<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string | <a href="#managedinstanceadministratortype">Pulumi.<wbr>Azure<wbr>Native.<wbr>Sql.<wbr>Managed<wbr>Instance<wbr>Administrator<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}Type of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="login_csharp">
<a href="#login_csharp" style="color: inherit; text-decoration: inherit;">Login</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Login name of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="managedinstancename_csharp">
<a href="#managedinstancename_csharp" style="color: inherit; text-decoration: inherit;">Managed<wbr>Instance<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the managed instance.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sid_csharp">
<a href="#sid_csharp" style="color: inherit; text-decoration: inherit;">Sid</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}SID (object ID) of the managed instance administrator.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="administratorname_csharp">
<a href="#administratorname_csharp" style="color: inherit; text-decoration: inherit;">Administrator<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tenantid_csharp">
<a href="#tenantid_csharp" style="color: inherit; text-decoration: inherit;">Tenant<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Tenant ID of the managed instance administrator.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="administratortype_go">
<a href="#administratortype_go" style="color: inherit; text-decoration: inherit;">Administrator<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string | <a href="#managedinstanceadministratortype">Managed<wbr>Instance<wbr>Administrator<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}Type of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="login_go">
<a href="#login_go" style="color: inherit; text-decoration: inherit;">Login</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Login name of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="managedinstancename_go">
<a href="#managedinstancename_go" style="color: inherit; text-decoration: inherit;">Managed<wbr>Instance<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the managed instance.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sid_go">
<a href="#sid_go" style="color: inherit; text-decoration: inherit;">Sid</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}SID (object ID) of the managed instance administrator.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="administratorname_go">
<a href="#administratorname_go" style="color: inherit; text-decoration: inherit;">Administrator<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tenantid_go">
<a href="#tenantid_go" style="color: inherit; text-decoration: inherit;">Tenant<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Tenant ID of the managed instance administrator.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="administratortype_nodejs">
<a href="#administratortype_nodejs" style="color: inherit; text-decoration: inherit;">administrator<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string | <a href="#managedinstanceadministratortype">Managed<wbr>Instance<wbr>Administrator<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}Type of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="login_nodejs">
<a href="#login_nodejs" style="color: inherit; text-decoration: inherit;">login</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Login name of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="managedinstancename_nodejs">
<a href="#managedinstancename_nodejs" style="color: inherit; text-decoration: inherit;">managed<wbr>Instance<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the managed instance.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sid_nodejs">
<a href="#sid_nodejs" style="color: inherit; text-decoration: inherit;">sid</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}SID (object ID) of the managed instance administrator.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="administratorname_nodejs">
<a href="#administratorname_nodejs" style="color: inherit; text-decoration: inherit;">administrator<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tenantid_nodejs">
<a href="#tenantid_nodejs" style="color: inherit; text-decoration: inherit;">tenant<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Tenant ID of the managed instance administrator.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="administrator_type_python">
<a href="#administrator_type_python" style="color: inherit; text-decoration: inherit;">administrator_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str | <a href="#managedinstanceadministratortype">Managed<wbr>Instance<wbr>Administrator<wbr>Type</a></span>
    </dt>
    <dd>{{% md %}}Type of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="login_python">
<a href="#login_python" style="color: inherit; text-decoration: inherit;">login</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Login name of the managed instance administrator.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="managed_instance_name_python">
<a href="#managed_instance_name_python" style="color: inherit; text-decoration: inherit;">managed_<wbr>instance_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the managed instance.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sid_python">
<a href="#sid_python" style="color: inherit; text-decoration: inherit;">sid</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SID (object ID) of the managed instance administrator.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="administrator_name_python">
<a href="#administrator_name_python" style="color: inherit; text-decoration: inherit;">administrator_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tenant_id_python">
<a href="#tenant_id_python" style="color: inherit; text-decoration: inherit;">tenant_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Tenant ID of the managed instance administrator.{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the ManagedInstanceAdministrator resource produces the following output properties:



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







## Supporting Types



<h4 id="managedinstanceadministratortype">Managed<wbr>Instance<wbr>Administrator<wbr>Type</h4>

{{% choosable language csharp %}}
<dl class="tabular"><dt>Active<wbr>Directory</dt>
    <dd>ActiveDirectory</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="tabular"><dt>Managed<wbr>Instance<wbr>Administrator<wbr>Type<wbr>Active<wbr>Directory</dt>
    <dd>ActiveDirectory</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="tabular"><dt>Active<wbr>Directory</dt>
    <dd>ActiveDirectory</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="tabular"><dt>ACTIVE_DIRECTORY</dt>
    <dd>ActiveDirectory</dd></dl>
{{% /choosable %}}
## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:sql:ManagedInstanceAdministrator ActiveDirectory /subscriptions/00000000-1111-2222-3333-444444444444/resourceGroups/Default-SQL-SouthEastAsia/providers/Microsoft.Sql/managedInstances/managedInstance/administrators/ActiveDirectory 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

