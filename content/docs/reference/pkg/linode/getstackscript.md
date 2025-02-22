
---
title: "getStackScript"
title_tag: "linode.getStackScript"
meta_desc: "Documentation for the linode.getStackScript function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Provides details about a specific Linode StackScript.
## Attributes

This resource exports the following attributes:

* `label` - The StackScript's label is for display purposes only.

* `script` - The script to execute when provisioning a new Linode with this StackScript.

* `description` - A description for the StackScript.

* `rev_note` - This field allows you to add notes for the set of revisions made to this StackScript.

* `is_public` - This determines whether other users can use your StackScript. Once a StackScript is made public, it cannot be made private.

* `images` - An array of Image IDs representing the Images that this StackScript is compatible for deploying with.

* `deployments_active` - Count of currently active, deployed Linodes created from this StackScript.

* `user_gravatar_id` - The Gravatar ID for the User who created the StackScript.

* `deployments_total` - The total number of times this StackScript has been deployed.

* `username` - The User who created the StackScript.

* `created` - The date this StackScript was created.

* `updated` - The date this StackScript was updated.

* `user_defined_fields` - This is a list of fields defined with a special syntax inside this StackScript that allow for supplying customized parameters during deployment.
  
  * `label` - A human-readable label for the field that will serve as the input prompt for entering the value during deployment.
  
  * `name` - The name of the field.
  
  * `example` - An example value for the field.
  
  * `one_of` - A list of acceptable single values for the field.
  
  * `many_of` - A list of acceptable values for the field in any quantity, combination or order.
  
  * `default` - The default value. If not specified, this value will be used.


{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using Linode = Pulumi.Linode;

class MyStack : Stack
{
    public MyStack()
    {
        var myStackscript = Output.Create(Linode.GetStackScript.InvokeAsync(new Linode.GetStackScriptArgs
        {
            Id = 355872,
        }));
    }

}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-linode/sdk/v2/go/linode"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := linode.LookupStackScript(ctx, &linode.LookupStackScriptArgs{
			Id: 355872,
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
import pulumi_linode as linode

my_stackscript = linode.get_stack_script(id=355872)
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as linode from "@pulumi/linode";

const myStackscript = pulumi.output(linode.getStackScript({
    id: 355872,
}, { async: true }));
```


{{< /example >}}





{{% /examples %}}




## Using getStackScript {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getStackScript<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetStackScriptArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetStackScriptResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_stack_script(</span><span class="nx">id</span><span class="p">:</span> <span class="nx">Optional[int]</span> = None<span class="p">, </span><span class="nx">user_defined_fields</span><span class="p">:</span> <span class="nx">Optional[Sequence[GetStackScriptUserDefinedFieldArgs]]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetStackScriptResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupStackScript<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupStackScriptArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupStackScriptResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupStackScript` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetStackScript </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetStackScriptResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetStackScriptArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The unique numeric ID of the StackScript to query.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="userdefinedfields_csharp">
<a href="#userdefinedfields_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Defined<wbr>Fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">List&lt;Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The unique numeric ID of the StackScript to query.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="userdefinedfields_go">
<a href="#userdefinedfields_go" style="color: inherit; text-decoration: inherit;">User<wbr>Defined<wbr>Fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">[]Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The unique numeric ID of the StackScript to query.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="userdefinedfields_nodejs">
<a href="#userdefinedfields_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Defined<wbr>Fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field[]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The unique numeric ID of the StackScript to query.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="user_defined_fields_python">
<a href="#user_defined_fields_python" style="color: inherit; text-decoration: inherit;">user_<wbr>defined_<wbr>fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">Sequence[Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field<wbr>Args]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}




## getStackScript Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="created_csharp">
<a href="#created_csharp" style="color: inherit; text-decoration: inherit;">Created</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deploymentsactive_csharp">
<a href="#deploymentsactive_csharp" style="color: inherit; text-decoration: inherit;">Deployments<wbr>Active</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deploymentstotal_csharp">
<a href="#deploymentstotal_csharp" style="color: inherit; text-decoration: inherit;">Deployments<wbr>Total</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_csharp">
<a href="#description_csharp" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="images_csharp">
<a href="#images_csharp" style="color: inherit; text-decoration: inherit;">Images</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ispublic_csharp">
<a href="#ispublic_csharp" style="color: inherit; text-decoration: inherit;">Is<wbr>Public</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="label_csharp">
<a href="#label_csharp" style="color: inherit; text-decoration: inherit;">Label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="revnote_csharp">
<a href="#revnote_csharp" style="color: inherit; text-decoration: inherit;">Rev<wbr>Note</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="script_csharp">
<a href="#script_csharp" style="color: inherit; text-decoration: inherit;">Script</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updated_csharp">
<a href="#updated_csharp" style="color: inherit; text-decoration: inherit;">Updated</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userdefinedfields_csharp">
<a href="#userdefinedfields_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Defined<wbr>Fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">List&lt;Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field&gt;</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="usergravatarid_csharp">
<a href="#usergravatarid_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Gravatar<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="username_csharp">
<a href="#username_csharp" style="color: inherit; text-decoration: inherit;">Username</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="created_go">
<a href="#created_go" style="color: inherit; text-decoration: inherit;">Created</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deploymentsactive_go">
<a href="#deploymentsactive_go" style="color: inherit; text-decoration: inherit;">Deployments<wbr>Active</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deploymentstotal_go">
<a href="#deploymentstotal_go" style="color: inherit; text-decoration: inherit;">Deployments<wbr>Total</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_go">
<a href="#description_go" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="images_go">
<a href="#images_go" style="color: inherit; text-decoration: inherit;">Images</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ispublic_go">
<a href="#ispublic_go" style="color: inherit; text-decoration: inherit;">Is<wbr>Public</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="label_go">
<a href="#label_go" style="color: inherit; text-decoration: inherit;">Label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="revnote_go">
<a href="#revnote_go" style="color: inherit; text-decoration: inherit;">Rev<wbr>Note</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="script_go">
<a href="#script_go" style="color: inherit; text-decoration: inherit;">Script</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updated_go">
<a href="#updated_go" style="color: inherit; text-decoration: inherit;">Updated</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userdefinedfields_go">
<a href="#userdefinedfields_go" style="color: inherit; text-decoration: inherit;">User<wbr>Defined<wbr>Fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">[]Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="usergravatarid_go">
<a href="#usergravatarid_go" style="color: inherit; text-decoration: inherit;">User<wbr>Gravatar<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="username_go">
<a href="#username_go" style="color: inherit; text-decoration: inherit;">Username</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="created_nodejs">
<a href="#created_nodejs" style="color: inherit; text-decoration: inherit;">created</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deploymentsactive_nodejs">
<a href="#deploymentsactive_nodejs" style="color: inherit; text-decoration: inherit;">deployments<wbr>Active</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deploymentstotal_nodejs">
<a href="#deploymentstotal_nodejs" style="color: inherit; text-decoration: inherit;">deployments<wbr>Total</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_nodejs">
<a href="#description_nodejs" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="images_nodejs">
<a href="#images_nodejs" style="color: inherit; text-decoration: inherit;">images</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ispublic_nodejs">
<a href="#ispublic_nodejs" style="color: inherit; text-decoration: inherit;">is<wbr>Public</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="label_nodejs">
<a href="#label_nodejs" style="color: inherit; text-decoration: inherit;">label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="revnote_nodejs">
<a href="#revnote_nodejs" style="color: inherit; text-decoration: inherit;">rev<wbr>Note</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="script_nodejs">
<a href="#script_nodejs" style="color: inherit; text-decoration: inherit;">script</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updated_nodejs">
<a href="#updated_nodejs" style="color: inherit; text-decoration: inherit;">updated</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="userdefinedfields_nodejs">
<a href="#userdefinedfields_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Defined<wbr>Fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field[]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="usergravatarid_nodejs">
<a href="#usergravatarid_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Gravatar<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="username_nodejs">
<a href="#username_nodejs" style="color: inherit; text-decoration: inherit;">username</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="created_python">
<a href="#created_python" style="color: inherit; text-decoration: inherit;">created</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deployments_active_python">
<a href="#deployments_active_python" style="color: inherit; text-decoration: inherit;">deployments_<wbr>active</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="deployments_total_python">
<a href="#deployments_total_python" style="color: inherit; text-decoration: inherit;">deployments_<wbr>total</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="description_python">
<a href="#description_python" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="images_python">
<a href="#images_python" style="color: inherit; text-decoration: inherit;">images</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Sequence[str]</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="is_public_python">
<a href="#is_public_python" style="color: inherit; text-decoration: inherit;">is_<wbr>public</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="label_python">
<a href="#label_python" style="color: inherit; text-decoration: inherit;">label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="rev_note_python">
<a href="#rev_note_python" style="color: inherit; text-decoration: inherit;">rev_<wbr>note</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="script_python">
<a href="#script_python" style="color: inherit; text-decoration: inherit;">script</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updated_python">
<a href="#updated_python" style="color: inherit; text-decoration: inherit;">updated</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="user_defined_fields_python">
<a href="#user_defined_fields_python" style="color: inherit; text-decoration: inherit;">user_<wbr>defined_<wbr>fields</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getstackscriptuserdefinedfield">Sequence[Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="user_gravatar_id_python">
<a href="#user_gravatar_id_python" style="color: inherit; text-decoration: inherit;">user_<wbr>gravatar_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="username_python">
<a href="#username_python" style="color: inherit; text-decoration: inherit;">username</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}




## Supporting Types


<h4 id="getstackscriptuserdefinedfield">Get<wbr>Stack<wbr>Script<wbr>User<wbr>Defined<wbr>Field</h4>



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="default_csharp">
<a href="#default_csharp" style="color: inherit; text-decoration: inherit;">Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="example_csharp">
<a href="#example_csharp" style="color: inherit; text-decoration: inherit;">Example</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="label_csharp">
<a href="#label_csharp" style="color: inherit; text-decoration: inherit;">Label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="manyof_csharp">
<a href="#manyof_csharp" style="color: inherit; text-decoration: inherit;">Many<wbr>Of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="oneof_csharp">
<a href="#oneof_csharp" style="color: inherit; text-decoration: inherit;">One<wbr>Of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="default_go">
<a href="#default_go" style="color: inherit; text-decoration: inherit;">Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="example_go">
<a href="#example_go" style="color: inherit; text-decoration: inherit;">Example</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="label_go">
<a href="#label_go" style="color: inherit; text-decoration: inherit;">Label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="manyof_go">
<a href="#manyof_go" style="color: inherit; text-decoration: inherit;">Many<wbr>Of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="oneof_go">
<a href="#oneof_go" style="color: inherit; text-decoration: inherit;">One<wbr>Of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="default_nodejs">
<a href="#default_nodejs" style="color: inherit; text-decoration: inherit;">default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="example_nodejs">
<a href="#example_nodejs" style="color: inherit; text-decoration: inherit;">example</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="label_nodejs">
<a href="#label_nodejs" style="color: inherit; text-decoration: inherit;">label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="manyof_nodejs">
<a href="#manyof_nodejs" style="color: inherit; text-decoration: inherit;">many<wbr>Of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="oneof_nodejs">
<a href="#oneof_nodejs" style="color: inherit; text-decoration: inherit;">one<wbr>Of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="default_python">
<a href="#default_python" style="color: inherit; text-decoration: inherit;">default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="example_python">
<a href="#example_python" style="color: inherit; text-decoration: inherit;">example</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="label_python">
<a href="#label_python" style="color: inherit; text-decoration: inherit;">label</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="many_of_python">
<a href="#many_of_python" style="color: inherit; text-decoration: inherit;">many_<wbr>of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="one_of_python">
<a href="#one_of_python" style="color: inherit; text-decoration: inherit;">one_<wbr>of</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-linode">https://github.com/pulumi/pulumi-linode</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`linode` Terraform Provider](https://github.com/linode/terraform-provider-linode).{{% /md %}}</dd>
</dl>

