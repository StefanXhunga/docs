
---
title: "getPrefix"
title_tag: "azure-native.peering.getPrefix"
meta_desc: "Documentation for the azure-native.peering.getPrefix function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

The peering service prefix class.
API Version: 2021-01-01.




## Using getPrefix {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getPrefix<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetPrefixArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetPrefixResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_prefix(</span><span class="nx">expand</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">peering_service_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">prefix_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetPrefixResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupPrefix<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupPrefixArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupPrefixResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupPrefix` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetPrefix </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetPrefixResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetPrefixArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="peeringservicename_csharp">
<a href="#peeringservicename_csharp" style="color: inherit; text-decoration: inherit;">Peering<wbr>Service<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the peering service.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="prefixname_csharp">
<a href="#prefixname_csharp" style="color: inherit; text-decoration: inherit;">Prefix<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="expand_csharp">
<a href="#expand_csharp" style="color: inherit; text-decoration: inherit;">Expand</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The properties to be expanded.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="peeringservicename_go">
<a href="#peeringservicename_go" style="color: inherit; text-decoration: inherit;">Peering<wbr>Service<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the peering service.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="prefixname_go">
<a href="#prefixname_go" style="color: inherit; text-decoration: inherit;">Prefix<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="expand_go">
<a href="#expand_go" style="color: inherit; text-decoration: inherit;">Expand</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The properties to be expanded.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="peeringservicename_nodejs">
<a href="#peeringservicename_nodejs" style="color: inherit; text-decoration: inherit;">peering<wbr>Service<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the peering service.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="prefixname_nodejs">
<a href="#prefixname_nodejs" style="color: inherit; text-decoration: inherit;">prefix<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="expand_nodejs">
<a href="#expand_nodejs" style="color: inherit; text-decoration: inherit;">expand</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The properties to be expanded.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="peering_service_name_python">
<a href="#peering_service_name_python" style="color: inherit; text-decoration: inherit;">peering_<wbr>service_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the peering service.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="prefix_name_python">
<a href="#prefix_name_python" style="color: inherit; text-decoration: inherit;">prefix_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="expand_python">
<a href="#expand_python" style="color: inherit; text-decoration: inherit;">expand</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The properties to be expanded.{{% /md %}}</dd></dl>
{{% /choosable %}}




## getPrefix Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="errormessage_csharp">
<a href="#errormessage_csharp" style="color: inherit; text-decoration: inherit;">Error<wbr>Message</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The error message for validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="events_csharp">
<a href="#events_csharp" style="color: inherit; text-decoration: inherit;">Events</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#peeringserviceprefixeventresponse">List&lt;Pulumi.<wbr>Azure<wbr>Native.<wbr>Peering.<wbr>Outputs.<wbr>Peering<wbr>Service<wbr>Prefix<wbr>Event<wbr>Response&gt;</a></span>
    </dt>
    <dd>{{% md %}}The list of events for peering service prefix{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learnedtype_csharp">
<a href="#learnedtype_csharp" style="color: inherit; text-decoration: inherit;">Learned<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix learned type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefixvalidationstate_csharp">
<a href="#prefixvalidationstate_csharp" style="color: inherit; text-decoration: inherit;">Prefix<wbr>Validation<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="provisioningstate_csharp">
<a href="#provisioningstate_csharp" style="color: inherit; text-decoration: inherit;">Provisioning<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provisioning state of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="peeringserviceprefixkey_csharp">
<a href="#peeringserviceprefixkey_csharp" style="color: inherit; text-decoration: inherit;">Peering<wbr>Service<wbr>Prefix<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The peering service prefix key{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefix_csharp">
<a href="#prefix_csharp" style="color: inherit; text-decoration: inherit;">Prefix</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix from which your traffic originates.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="errormessage_go">
<a href="#errormessage_go" style="color: inherit; text-decoration: inherit;">Error<wbr>Message</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The error message for validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="events_go">
<a href="#events_go" style="color: inherit; text-decoration: inherit;">Events</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#peeringserviceprefixeventresponse">[]Peering<wbr>Service<wbr>Prefix<wbr>Event<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}The list of events for peering service prefix{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learnedtype_go">
<a href="#learnedtype_go" style="color: inherit; text-decoration: inherit;">Learned<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix learned type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefixvalidationstate_go">
<a href="#prefixvalidationstate_go" style="color: inherit; text-decoration: inherit;">Prefix<wbr>Validation<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="provisioningstate_go">
<a href="#provisioningstate_go" style="color: inherit; text-decoration: inherit;">Provisioning<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provisioning state of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="peeringserviceprefixkey_go">
<a href="#peeringserviceprefixkey_go" style="color: inherit; text-decoration: inherit;">Peering<wbr>Service<wbr>Prefix<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The peering service prefix key{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefix_go">
<a href="#prefix_go" style="color: inherit; text-decoration: inherit;">Prefix</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix from which your traffic originates.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="errormessage_nodejs">
<a href="#errormessage_nodejs" style="color: inherit; text-decoration: inherit;">error<wbr>Message</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The error message for validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="events_nodejs">
<a href="#events_nodejs" style="color: inherit; text-decoration: inherit;">events</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#peeringserviceprefixeventresponse">Peering<wbr>Service<wbr>Prefix<wbr>Event<wbr>Response[]</a></span>
    </dt>
    <dd>{{% md %}}The list of events for peering service prefix{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learnedtype_nodejs">
<a href="#learnedtype_nodejs" style="color: inherit; text-decoration: inherit;">learned<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix learned type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefixvalidationstate_nodejs">
<a href="#prefixvalidationstate_nodejs" style="color: inherit; text-decoration: inherit;">prefix<wbr>Validation<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="provisioningstate_nodejs">
<a href="#provisioningstate_nodejs" style="color: inherit; text-decoration: inherit;">provisioning<wbr>State</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provisioning state of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="peeringserviceprefixkey_nodejs">
<a href="#peeringserviceprefixkey_nodejs" style="color: inherit; text-decoration: inherit;">peering<wbr>Service<wbr>Prefix<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The peering service prefix key{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefix_nodejs">
<a href="#prefix_nodejs" style="color: inherit; text-decoration: inherit;">prefix</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The prefix from which your traffic originates.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="error_message_python">
<a href="#error_message_python" style="color: inherit; text-decoration: inherit;">error_<wbr>message</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The error message for validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="events_python">
<a href="#events_python" style="color: inherit; text-decoration: inherit;">events</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#peeringserviceprefixeventresponse">Sequence[Peering<wbr>Service<wbr>Prefix<wbr>Event<wbr>Response]</a></span>
    </dt>
    <dd>{{% md %}}The list of events for peering service prefix{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learned_type_python">
<a href="#learned_type_python" style="color: inherit; text-decoration: inherit;">learned_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The prefix learned type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefix_validation_state_python">
<a href="#prefix_validation_state_python" style="color: inherit; text-decoration: inherit;">prefix_<wbr>validation_<wbr>state</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The prefix validation state{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="provisioning_state_python">
<a href="#provisioning_state_python" style="color: inherit; text-decoration: inherit;">provisioning_<wbr>state</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provisioning state of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="peering_service_prefix_key_python">
<a href="#peering_service_prefix_key_python" style="color: inherit; text-decoration: inherit;">peering_<wbr>service_<wbr>prefix_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The peering service prefix key{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="prefix_python">
<a href="#prefix_python" style="color: inherit; text-decoration: inherit;">prefix</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The prefix from which your traffic originates.{{% /md %}}</dd></dl>
{{% /choosable %}}




## Supporting Types


<h4 id="peeringserviceprefixeventresponse">Peering<wbr>Service<wbr>Prefix<wbr>Event<wbr>Response</h4>



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="eventdescription_csharp">
<a href="#eventdescription_csharp" style="color: inherit; text-decoration: inherit;">Event<wbr>Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The description of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventlevel_csharp">
<a href="#eventlevel_csharp" style="color: inherit; text-decoration: inherit;">Event<wbr>Level</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The level of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventsummary_csharp">
<a href="#eventsummary_csharp" style="color: inherit; text-decoration: inherit;">Event<wbr>Summary</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The summary of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventtimestamp_csharp">
<a href="#eventtimestamp_csharp" style="color: inherit; text-decoration: inherit;">Event<wbr>Timestamp</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The timestamp of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventtype_csharp">
<a href="#eventtype_csharp" style="color: inherit; text-decoration: inherit;">Event<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the event associated with a prefix.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="eventdescription_go">
<a href="#eventdescription_go" style="color: inherit; text-decoration: inherit;">Event<wbr>Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The description of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventlevel_go">
<a href="#eventlevel_go" style="color: inherit; text-decoration: inherit;">Event<wbr>Level</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The level of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventsummary_go">
<a href="#eventsummary_go" style="color: inherit; text-decoration: inherit;">Event<wbr>Summary</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The summary of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventtimestamp_go">
<a href="#eventtimestamp_go" style="color: inherit; text-decoration: inherit;">Event<wbr>Timestamp</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The timestamp of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventtype_go">
<a href="#eventtype_go" style="color: inherit; text-decoration: inherit;">Event<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the event associated with a prefix.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="eventdescription_nodejs">
<a href="#eventdescription_nodejs" style="color: inherit; text-decoration: inherit;">event<wbr>Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The description of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventlevel_nodejs">
<a href="#eventlevel_nodejs" style="color: inherit; text-decoration: inherit;">event<wbr>Level</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The level of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventsummary_nodejs">
<a href="#eventsummary_nodejs" style="color: inherit; text-decoration: inherit;">event<wbr>Summary</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The summary of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventtimestamp_nodejs">
<a href="#eventtimestamp_nodejs" style="color: inherit; text-decoration: inherit;">event<wbr>Timestamp</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The timestamp of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="eventtype_nodejs">
<a href="#eventtype_nodejs" style="color: inherit; text-decoration: inherit;">event<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the event associated with a prefix.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="event_description_python">
<a href="#event_description_python" style="color: inherit; text-decoration: inherit;">event_<wbr>description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The description of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="event_level_python">
<a href="#event_level_python" style="color: inherit; text-decoration: inherit;">event_<wbr>level</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The level of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="event_summary_python">
<a href="#event_summary_python" style="color: inherit; text-decoration: inherit;">event_<wbr>summary</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The summary of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="event_timestamp_python">
<a href="#event_timestamp_python" style="color: inherit; text-decoration: inherit;">event_<wbr>timestamp</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The timestamp of the event associated with a prefix.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="event_type_python">
<a href="#event_type_python" style="color: inherit; text-decoration: inherit;">event_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of the event associated with a prefix.{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

