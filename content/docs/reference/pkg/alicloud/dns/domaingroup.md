
---
title: "DomainGroup"
title_tag: "alicloud.dns.DomainGroup"
meta_desc: "Documentation for the alicloud.dns.DomainGroup resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Provides a Alidns Domain Group resource. For information about Alidns Domain Group and how to use it, see [What is Resource Alidns Domain Group](https://www.alibabacloud.com/help/en/doc-detail/29762.htm).

> **NOTE:** Available in v1.84.0+.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using AliCloud = Pulumi.AliCloud;

class MyStack : Stack
{
    public MyStack()
    {
        // Add a new Alinds Domain Group.
        var example = new AliCloud.Dns.DomainGroup("example", new AliCloud.Dns.DomainGroupArgs
        {
            DomainGroupName = "tf-testDG",
        });
    }

}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/dns"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := dns.NewDomainGroup(ctx, "example", &dns.DomainGroupArgs{
			DomainGroupName: pulumi.String("tf-testDG"),
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
import pulumi_alicloud as alicloud

# Add a new Alinds Domain Group.
example = alicloud.dns.DomainGroup("example", domain_group_name="tf-testDG")
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as alicloud from "@pulumi/alicloud";

// Add a new Alinds Domain Group.
const example = new alicloud.dns.DomainGroup("example", {
    domainGroupName: "tf-testDG",
});
```


{{< /example >}}





{{% /examples %}}




## Create a DomainGroup Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">DomainGroup</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">?:</span> <span class="nx"><a href="#inputs">DomainGroupArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">DomainGroup</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">domain_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">lang</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewDomainGroup</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx"><a href="#inputs">DomainGroupArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">DomainGroup</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">DomainGroup</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">DomainGroupArgs</a></span><span class="p">? </span><span class="nx">args = null<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">DomainGroupArgs</a></span>
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
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span>
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
        class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">DomainGroupArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
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
        class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">DomainGroupArgs</a></span>
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

## DomainGroup Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The DomainGroup resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="domaingroupname_csharp">
<a href="#domaingroupname_csharp" style="color: inherit; text-decoration: inherit;">Domain<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="groupname_csharp">
<a href="#groupname_csharp" style="color: inherit; text-decoration: inherit;">Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="lang_csharp">
<a href="#lang_csharp" style="color: inherit; text-decoration: inherit;">Lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="domaingroupname_go">
<a href="#domaingroupname_go" style="color: inherit; text-decoration: inherit;">Domain<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="groupname_go">
<a href="#groupname_go" style="color: inherit; text-decoration: inherit;">Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="lang_go">
<a href="#lang_go" style="color: inherit; text-decoration: inherit;">Lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="domaingroupname_nodejs">
<a href="#domaingroupname_nodejs" style="color: inherit; text-decoration: inherit;">domain<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="groupname_nodejs">
<a href="#groupname_nodejs" style="color: inherit; text-decoration: inherit;">group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="lang_nodejs">
<a href="#lang_nodejs" style="color: inherit; text-decoration: inherit;">lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="domain_group_name_python">
<a href="#domain_group_name_python" style="color: inherit; text-decoration: inherit;">domain_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="group_name_python">
<a href="#group_name_python" style="color: inherit; text-decoration: inherit;">group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="lang_python">
<a href="#lang_python" style="color: inherit; text-decoration: inherit;">lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the DomainGroup resource produces the following output properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd></dl>
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
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd></dl>
{{% /choosable %}}



## Look up an Existing DomainGroup Resource {#look-up}

Get an existing DomainGroup resource's state with the given name, ID, and optional extra properties used to qualify the lookup.
{{< chooser language "typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">id</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span><span class="p">?:</span> <span class="nx">DomainGroupState</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx">DomainGroup</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class=nd>@staticmethod</span>
<span class="k">def </span><span class="nf">get</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">id</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">domain_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">lang</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">) -&gt;</span> DomainGroup</code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetDomainGroup<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">id</span><span class="p"> </span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span><span class="p"> *</span><span class="nx">DomainGroupState</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">DomainGroup</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx">DomainGroup</span><span class="nf"> Get</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input-1.html">Input&lt;string&gt;</a></span><span class="p"> </span><span class="nx">id<span class="p">, </span><span class="nx">DomainGroupState</span><span class="p">? </span><span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_domaingroupname_csharp">
<a href="#state_domaingroupname_csharp" style="color: inherit; text-decoration: inherit;">Domain<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="state_groupname_csharp">
<a href="#state_groupname_csharp" style="color: inherit; text-decoration: inherit;">Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="state_lang_csharp">
<a href="#state_lang_csharp" style="color: inherit; text-decoration: inherit;">Lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_domaingroupname_go">
<a href="#state_domaingroupname_go" style="color: inherit; text-decoration: inherit;">Domain<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="state_groupname_go">
<a href="#state_groupname_go" style="color: inherit; text-decoration: inherit;">Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="state_lang_go">
<a href="#state_lang_go" style="color: inherit; text-decoration: inherit;">Lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_domaingroupname_nodejs">
<a href="#state_domaingroupname_nodejs" style="color: inherit; text-decoration: inherit;">domain<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="state_groupname_nodejs">
<a href="#state_groupname_nodejs" style="color: inherit; text-decoration: inherit;">group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="state_lang_nodejs">
<a href="#state_lang_nodejs" style="color: inherit; text-decoration: inherit;">lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_domain_group_name_python">
<a href="#state_domain_group_name_python" style="color: inherit; text-decoration: inherit;">domain_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the domain group.
{{% /md %}}</dd><dt class="property-optional property-deprecated"
            title="Optional, Deprecated">
        <span id="state_group_name_python">
<a href="#state_group_name_python" style="color: inherit; text-decoration: inherit;">group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Replaced by `domain_group_name` after version 1.97.0.
{{% /md %}}<p class="property-message">Deprecated: {{% md %}}Field &#39;group_name&#39; has been deprecated from version 1.97.0. Use &#39;domain_group_name&#39; instead.{{% /md %}}</p></dd><dt class="property-optional"
            title="Optional">
        <span id="state_lang_python">
<a href="#state_lang_python" style="color: inherit; text-decoration: inherit;">lang</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}User language.
{{% /md %}}</dd></dl>
{{% /choosable %}}





## Import


Alidns domain group can be imported using the id, e.g.

```sh
 $ pulumi import alicloud:dns/domainGroup:DomainGroup example 0932eb3ddee7499085c4d13d45*****
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-alicloud">https://github.com/pulumi/pulumi-alicloud</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`alicloud` Terraform Provider](https://github.com/aliyun/terraform-provider-alicloud).{{% /md %}}</dd>
</dl>

