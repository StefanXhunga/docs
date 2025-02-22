
---
title: "TopicPermissions"
title_tag: "rabbitmq.TopicPermissions"
meta_desc: "Documentation for the rabbitmq.TopicPermissions resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

The ``rabbitmq.TopicPermissions`` resource creates and manages a user's set of
topic permissions.

{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using RabbitMQ = Pulumi.RabbitMQ;

class MyStack : Stack
{
    public MyStack()
    {
        var testVHost = new RabbitMQ.VHost("testVHost", new RabbitMQ.VHostArgs
        {
        });
        var testUser = new RabbitMQ.User("testUser", new RabbitMQ.UserArgs
        {
            Password = "foobar",
            Tags = 
            {
                "administrator",
            },
        });
        var testTopicPermissions = new RabbitMQ.TopicPermissions("testTopicPermissions", new RabbitMQ.TopicPermissionsArgs
        {
            Permissions = 
            {
                new RabbitMQ.Inputs.TopicPermissionsPermissionArgs
                {
                    Exchange = "amq.topic",
                    Read = ".*",
                    Write = ".*",
                },
            },
            User = testUser.Name,
            Vhost = testVHost.Name,
        });
    }

}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-rabbitmq/sdk/v2/go/rabbitmq"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		testVHost, err := rabbitmq.NewVHost(ctx, "testVHost", nil)
		if err != nil {
			return err
		}
		testUser, err := rabbitmq.NewUser(ctx, "testUser", &rabbitmq.UserArgs{
			Password: pulumi.String("foobar"),
			Tags: pulumi.StringArray{
				pulumi.String("administrator"),
			},
		})
		if err != nil {
			return err
		}
		_, err = rabbitmq.NewTopicPermissions(ctx, "testTopicPermissions", &rabbitmq.TopicPermissionsArgs{
			Permissions: rabbitmq.TopicPermissionsPermissionArray{
				&rabbitmq.TopicPermissionsPermissionArgs{
					Exchange: pulumi.String("amq.topic"),
					Read:     pulumi.String(".*"),
					Write:    pulumi.String(".*"),
				},
			},
			User:  testUser.Name,
			Vhost: testVHost.Name,
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
import pulumi_rabbitmq as rabbitmq

test_v_host = rabbitmq.VHost("testVHost")
test_user = rabbitmq.User("testUser",
    password="foobar",
    tags=["administrator"])
test_topic_permissions = rabbitmq.TopicPermissions("testTopicPermissions",
    permissions=[rabbitmq.TopicPermissionsPermissionArgs(
        exchange="amq.topic",
        read=".*",
        write=".*",
    )],
    user=test_user.name,
    vhost=test_v_host.name)
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as rabbitmq from "@pulumi/rabbitmq";

const testVHost = new rabbitmq.VHost("test", {});
const testUser = new rabbitmq.User("test", {
    password: "foobar",
    tags: ["administrator"],
});
const testTopicPermissions = new rabbitmq.TopicPermissions("test", {
    permissions: [{
        exchange: "amq.topic",
        read: ".*",
        write: ".*",
    }],
    user: testUser.name,
    vhost: testVHost.name,
});
```


{{< /example >}}





{{% /examples %}}




## Create a TopicPermissions Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">TopicPermissions</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">TopicPermissionsArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">TopicPermissions</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">permissions</span><span class="p">:</span> <span class="nx">Optional[Sequence[TopicPermissionsPermissionArgs]]</span> = None<span class="p">, </span><span class="nx">user</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">vhost</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewTopicPermissions</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">TopicPermissionsArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">TopicPermissions</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">TopicPermissions</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">TopicPermissionsArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span class="property-type"><a href="#inputs">TopicPermissionsArgs</a></span>
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
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">TopicPermissionsArgs</a></span>
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
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">TopicPermissionsArgs</a></span>
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

## TopicPermissions Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The TopicPermissions resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="permissions_csharp">
<a href="#permissions_csharp" style="color: inherit; text-decoration: inherit;">Permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">List&lt;Pulumi.<wbr>Rabbit<wbr>MQ.<wbr>Inputs.<wbr>Topic<wbr>Permissions<wbr>Permission<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="user_csharp">
<a href="#user_csharp" style="color: inherit; text-decoration: inherit;">User</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="vhost_csharp">
<a href="#vhost_csharp" style="color: inherit; text-decoration: inherit;">Vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="permissions_go">
<a href="#permissions_go" style="color: inherit; text-decoration: inherit;">Permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">[]Topic<wbr>Permissions<wbr>Permission</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="user_go">
<a href="#user_go" style="color: inherit; text-decoration: inherit;">User</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="vhost_go">
<a href="#vhost_go" style="color: inherit; text-decoration: inherit;">Vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="permissions_nodejs">
<a href="#permissions_nodejs" style="color: inherit; text-decoration: inherit;">permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">Topic<wbr>Permissions<wbr>Permission[]</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="user_nodejs">
<a href="#user_nodejs" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="vhost_nodejs">
<a href="#vhost_nodejs" style="color: inherit; text-decoration: inherit;">vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="permissions_python">
<a href="#permissions_python" style="color: inherit; text-decoration: inherit;">permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">Sequence[Topic<wbr>Permissions<wbr>Permission<wbr>Args]</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="user_python">
<a href="#user_python" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="vhost_python">
<a href="#vhost_python" style="color: inherit; text-decoration: inherit;">vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the TopicPermissions resource produces the following output properties:



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



## Look up an Existing TopicPermissions Resource {#look-up}

Get an existing TopicPermissions resource's state with the given name, ID, and optional extra properties used to qualify the lookup.
{{< chooser language "typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">id</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span><span class="p">?:</span> <span class="nx">TopicPermissionsState</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx">TopicPermissions</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class=nd>@staticmethod</span>
<span class="k">def </span><span class="nf">get</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">id</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">permissions</span><span class="p">:</span> <span class="nx">Optional[Sequence[TopicPermissionsPermissionArgs]]</span> = None<span class="p">, </span><span class="nx">user</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">vhost</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">) -&gt;</span> TopicPermissions</code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetTopicPermissions<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">id</span><span class="p"> </span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span><span class="p"> *</span><span class="nx">TopicPermissionsState</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">TopicPermissions</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx">TopicPermissions</span><span class="nf"> Get</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input-1.html">Input&lt;string&gt;</a></span><span class="p"> </span><span class="nx">id<span class="p">, </span><span class="nx">TopicPermissionsState</span><span class="p">? </span><span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span id="state_permissions_csharp">
<a href="#state_permissions_csharp" style="color: inherit; text-decoration: inherit;">Permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">List&lt;Pulumi.<wbr>Rabbit<wbr>MQ.<wbr>Inputs.<wbr>Topic<wbr>Permissions<wbr>Permission<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_user_csharp">
<a href="#state_user_csharp" style="color: inherit; text-decoration: inherit;">User</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_vhost_csharp">
<a href="#state_vhost_csharp" style="color: inherit; text-decoration: inherit;">Vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_permissions_go">
<a href="#state_permissions_go" style="color: inherit; text-decoration: inherit;">Permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">[]Topic<wbr>Permissions<wbr>Permission</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_user_go">
<a href="#state_user_go" style="color: inherit; text-decoration: inherit;">User</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_vhost_go">
<a href="#state_vhost_go" style="color: inherit; text-decoration: inherit;">Vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_permissions_nodejs">
<a href="#state_permissions_nodejs" style="color: inherit; text-decoration: inherit;">permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">Topic<wbr>Permissions<wbr>Permission[]</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_user_nodejs">
<a href="#state_user_nodejs" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_vhost_nodejs">
<a href="#state_vhost_nodejs" style="color: inherit; text-decoration: inherit;">vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="state_permissions_python">
<a href="#state_permissions_python" style="color: inherit; text-decoration: inherit;">permissions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#topicpermissionspermission">Sequence[Topic<wbr>Permissions<wbr>Permission<wbr>Args]</a></span>
    </dt>
    <dd>{{% md %}}The settings of the permissions. The structure is
described below.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_user_python">
<a href="#state_user_python" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The user to apply the permissions to.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="state_vhost_python">
<a href="#state_vhost_python" style="color: inherit; text-decoration: inherit;">vhost</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The vhost to create the resource in.
{{% /md %}}</dd></dl>
{{% /choosable %}}






## Supporting Types



<h4 id="topicpermissionspermission">Topic<wbr>Permissions<wbr>Permission</h4>

{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="exchange_csharp">
<a href="#exchange_csharp" style="color: inherit; text-decoration: inherit;">Exchange</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The exchange to set the permissions for.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="read_csharp">
<a href="#read_csharp" style="color: inherit; text-decoration: inherit;">Read</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The "read" ACL.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="write_csharp">
<a href="#write_csharp" style="color: inherit; text-decoration: inherit;">Write</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The "write" ACL.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="exchange_go">
<a href="#exchange_go" style="color: inherit; text-decoration: inherit;">Exchange</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The exchange to set the permissions for.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="read_go">
<a href="#read_go" style="color: inherit; text-decoration: inherit;">Read</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The "read" ACL.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="write_go">
<a href="#write_go" style="color: inherit; text-decoration: inherit;">Write</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The "write" ACL.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="exchange_nodejs">
<a href="#exchange_nodejs" style="color: inherit; text-decoration: inherit;">exchange</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The exchange to set the permissions for.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="read_nodejs">
<a href="#read_nodejs" style="color: inherit; text-decoration: inherit;">read</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The "read" ACL.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="write_nodejs">
<a href="#write_nodejs" style="color: inherit; text-decoration: inherit;">write</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The "write" ACL.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="exchange_python">
<a href="#exchange_python" style="color: inherit; text-decoration: inherit;">exchange</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The exchange to set the permissions for.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="read_python">
<a href="#read_python" style="color: inherit; text-decoration: inherit;">read</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The "read" ACL.
{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="write_python">
<a href="#write_python" style="color: inherit; text-decoration: inherit;">write</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The "write" ACL.
{{% /md %}}</dd></dl>
{{% /choosable %}}
## Import


Permissions can be imported using the `id` which is composed of

`user@vhost`. E.g.

```sh
 $ pulumi import rabbitmq:index/topicPermissions:TopicPermissions test user@vhost
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-rabbitmq">https://github.com/pulumi/pulumi-rabbitmq</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`rabbitmq` Terraform Provider](https://github.com/terraform-providers/terraform-provider-rabbitmq).{{% /md %}}</dd>
</dl>

