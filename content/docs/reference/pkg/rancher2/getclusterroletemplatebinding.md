
---
title: "getClusterRoleTemplateBinding"
title_tag: "rancher2.getClusterRoleTemplateBinding"
meta_desc: "Documentation for the rancher2.getClusterRoleTemplateBinding function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Use this data source to retrieve information about a Rancher v2 cluster role template binding.


{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using Rancher2 = Pulumi.Rancher2;

class MyStack : Stack
{
    public MyStack()
    {
        var foo = Output.Create(Rancher2.GetClusterRoleTemplateBinding.InvokeAsync(new Rancher2.GetClusterRoleTemplateBindingArgs
        {
            ClusterId = "foo_id",
            Name = "foo",
        }));
    }

}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-rancher2/sdk/v2/go/rancher2"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := rancher2.LookupClusterRoleTemplateBinding(ctx, &rancher2.LookupClusterRoleTemplateBindingArgs{
			ClusterId: "foo_id",
			Name:      "foo",
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
import pulumi_rancher2 as rancher2

foo = rancher2.get_cluster_role_template_binding(cluster_id="foo_id",
    name="foo")
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as rancher2 from "@pulumi/rancher2";

const foo = pulumi.output(rancher2.getClusterRoleTemplateBinding({
    clusterId: "foo_id",
    name: "foo",
}, { async: true }));
```


{{< /example >}}





{{% /examples %}}




## Using getClusterRoleTemplateBinding {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getClusterRoleTemplateBinding<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetClusterRoleTemplateBindingArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetClusterRoleTemplateBindingResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_cluster_role_template_binding(</span><span class="nx">cluster_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">role_template_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetClusterRoleTemplateBindingResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupClusterRoleTemplateBinding<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupClusterRoleTemplateBindingArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupClusterRoleTemplateBindingResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupClusterRoleTemplateBinding` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetClusterRoleTemplateBinding </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetClusterRoleTemplateBindingResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetClusterRoleTemplateBindingArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="clusterid_csharp">
<a href="#clusterid_csharp" style="color: inherit; text-decoration: inherit;">Cluster<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where bind cluster role template (string)
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster role template binding (string)
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="roletemplateid_csharp">
<a href="#roletemplateid_csharp" style="color: inherit; text-decoration: inherit;">Role<wbr>Template<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The role template id from create cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="clusterid_go">
<a href="#clusterid_go" style="color: inherit; text-decoration: inherit;">Cluster<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where bind cluster role template (string)
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster role template binding (string)
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="roletemplateid_go">
<a href="#roletemplateid_go" style="color: inherit; text-decoration: inherit;">Role<wbr>Template<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The role template id from create cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="clusterid_nodejs">
<a href="#clusterid_nodejs" style="color: inherit; text-decoration: inherit;">cluster<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where bind cluster role template (string)
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster role template binding (string)
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="roletemplateid_nodejs">
<a href="#roletemplateid_nodejs" style="color: inherit; text-decoration: inherit;">role<wbr>Template<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The role template id from create cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="cluster_id_python">
<a href="#cluster_id_python" style="color: inherit; text-decoration: inherit;">cluster_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id where bind cluster role template (string)
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the cluster role template binding (string)
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="role_template_id_python">
<a href="#role_template_id_python" style="color: inherit; text-decoration: inherit;">role_<wbr>template_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The role template id from create cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}




## getClusterRoleTemplateBinding Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="annotations_csharp">
<a href="#annotations_csharp" style="color: inherit; text-decoration: inherit;">Annotations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations of the resource (map)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="clusterid_csharp">
<a href="#clusterid_csharp" style="color: inherit; text-decoration: inherit;">Cluster<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="groupid_csharp">
<a href="#groupid_csharp" style="color: inherit; text-decoration: inherit;">Group<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The group ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="groupprincipalid_csharp">
<a href="#groupprincipalid_csharp" style="color: inherit; text-decoration: inherit;">Group<wbr>Principal<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The group_principal ID to assign cluster role template binding (string)
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
        <span id="labels_csharp">
<a href="#labels_csharp" style="color: inherit; text-decoration: inherit;">Labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels of the resource (map)
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
        <span id="roletemplateid_csharp">
<a href="#roletemplateid_csharp" style="color: inherit; text-decoration: inherit;">Role<wbr>Template<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userid_csharp">
<a href="#userid_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The user ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userprincipalid_csharp">
<a href="#userprincipalid_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Principal<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The user_principal ID to assign cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="annotations_go">
<a href="#annotations_go" style="color: inherit; text-decoration: inherit;">Annotations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations of the resource (map)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="clusterid_go">
<a href="#clusterid_go" style="color: inherit; text-decoration: inherit;">Cluster<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="groupid_go">
<a href="#groupid_go" style="color: inherit; text-decoration: inherit;">Group<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The group ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="groupprincipalid_go">
<a href="#groupprincipalid_go" style="color: inherit; text-decoration: inherit;">Group<wbr>Principal<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The group_principal ID to assign cluster role template binding (string)
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
        <span id="labels_go">
<a href="#labels_go" style="color: inherit; text-decoration: inherit;">Labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels of the resource (map)
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
        <span id="roletemplateid_go">
<a href="#roletemplateid_go" style="color: inherit; text-decoration: inherit;">Role<wbr>Template<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userid_go">
<a href="#userid_go" style="color: inherit; text-decoration: inherit;">User<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The user ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userprincipalid_go">
<a href="#userprincipalid_go" style="color: inherit; text-decoration: inherit;">User<wbr>Principal<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The user_principal ID to assign cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="annotations_nodejs">
<a href="#annotations_nodejs" style="color: inherit; text-decoration: inherit;">annotations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations of the resource (map)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="clusterid_nodejs">
<a href="#clusterid_nodejs" style="color: inherit; text-decoration: inherit;">cluster<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="groupid_nodejs">
<a href="#groupid_nodejs" style="color: inherit; text-decoration: inherit;">group<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The group ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="groupprincipalid_nodejs">
<a href="#groupprincipalid_nodejs" style="color: inherit; text-decoration: inherit;">group<wbr>Principal<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The group_principal ID to assign cluster role template binding (string)
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
        <span id="labels_nodejs">
<a href="#labels_nodejs" style="color: inherit; text-decoration: inherit;">labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels of the resource (map)
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
        <span id="roletemplateid_nodejs">
<a href="#roletemplateid_nodejs" style="color: inherit; text-decoration: inherit;">role<wbr>Template<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userid_nodejs">
<a href="#userid_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The user ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userprincipalid_nodejs">
<a href="#userprincipalid_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Principal<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Computed) The user_principal ID to assign cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="annotations_python">
<a href="#annotations_python" style="color: inherit; text-decoration: inherit;">annotations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, Any]</span>
    </dt>
    <dd>{{% md %}}(Computed) Annotations of the resource (map)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cluster_id_python">
<a href="#cluster_id_python" style="color: inherit; text-decoration: inherit;">cluster_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="group_id_python">
<a href="#group_id_python" style="color: inherit; text-decoration: inherit;">group_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The group ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="group_principal_id_python">
<a href="#group_principal_id_python" style="color: inherit; text-decoration: inherit;">group_<wbr>principal_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The group_principal ID to assign cluster role template binding (string)
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
        <span id="labels_python">
<a href="#labels_python" style="color: inherit; text-decoration: inherit;">labels</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, Any]</span>
    </dt>
    <dd>{{% md %}}(Computed) Labels of the resource (map)
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
        <span id="role_template_id_python">
<a href="#role_template_id_python" style="color: inherit; text-decoration: inherit;">role_<wbr>template_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="user_id_python">
<a href="#user_id_python" style="color: inherit; text-decoration: inherit;">user_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The user ID to assign cluster role template binding (string)
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="user_principal_id_python">
<a href="#user_principal_id_python" style="color: inherit; text-decoration: inherit;">user_<wbr>principal_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Computed) The user_principal ID to assign cluster role template binding (string)
{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-rancher2">https://github.com/pulumi/pulumi-rancher2</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`rancher2` Terraform Provider](https://github.com/rancher/terraform-provider-rancher2).{{% /md %}}</dd>
</dl>

