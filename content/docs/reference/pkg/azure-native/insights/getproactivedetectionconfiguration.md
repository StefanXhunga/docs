
---
title: "getProactiveDetectionConfiguration"
title_tag: "azure-native.insights.getProactiveDetectionConfiguration"
meta_desc: "Documentation for the azure-native.insights.getProactiveDetectionConfiguration function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Properties that define a ProactiveDetection configuration.
API Version: 2015-05-01.




## Using getProactiveDetectionConfiguration {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getProactiveDetectionConfiguration<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetProactiveDetectionConfigurationArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetProactiveDetectionConfigurationResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_proactive_detection_configuration(</span><span class="nx">configuration_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetProactiveDetectionConfigurationResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupProactiveDetectionConfiguration<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupProactiveDetectionConfigurationArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupProactiveDetectionConfigurationResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupProactiveDetectionConfiguration` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetProactiveDetectionConfiguration </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetProactiveDetectionConfigurationResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetProactiveDetectionConfigurationArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="configurationid_csharp">
<a href="#configurationid_csharp" style="color: inherit; text-decoration: inherit;">Configuration<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ProactiveDetection configuration ID. This is unique within a Application Insights component.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcename_csharp">
<a href="#resourcename_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Application Insights component resource.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="configurationid_go">
<a href="#configurationid_go" style="color: inherit; text-decoration: inherit;">Configuration<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ProactiveDetection configuration ID. This is unique within a Application Insights component.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcename_go">
<a href="#resourcename_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Application Insights component resource.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="configurationid_nodejs">
<a href="#configurationid_nodejs" style="color: inherit; text-decoration: inherit;">configuration<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ProactiveDetection configuration ID. This is unique within a Application Insights component.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcename_nodejs">
<a href="#resourcename_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Application Insights component resource.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="configuration_id_python">
<a href="#configuration_id_python" style="color: inherit; text-decoration: inherit;">configuration_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ProactiveDetection configuration ID. This is unique within a Application Insights component.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_name_python">
<a href="#resource_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Application Insights component resource.{{% /md %}}</dd></dl>
{{% /choosable %}}




## getProactiveDetectionConfiguration Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="customemails_csharp">
<a href="#customemails_csharp" style="color: inherit; text-decoration: inherit;">Custom<wbr>Emails</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}Custom email addresses for this rule notifications{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enabled_csharp">
<a href="#enabled_csharp" style="color: inherit; text-decoration: inherit;">Enabled</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag that indicates whether this rule is enabled by the user{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="lastupdatedtime_csharp">
<a href="#lastupdatedtime_csharp" style="color: inherit; text-decoration: inherit;">Last<wbr>Updated<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The last time this rule was updated{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ruledefinitions_csharp">
<a href="#ruledefinitions_csharp" style="color: inherit; text-decoration: inherit;">Rule<wbr>Definitions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#applicationinsightscomponentproactivedetectionconfigurationresponseruledefinitions">Pulumi.<wbr>Azure<wbr>Native.<wbr>Insights.<wbr>Outputs.<wbr>Application<wbr>Insights<wbr>Component<wbr>Proactive<wbr>Detection<wbr>Configuration<wbr>Response<wbr>Rule<wbr>Definitions</a></span>
    </dt>
    <dd>{{% md %}}Static definitions of the ProactiveDetection configuration rule (same values for all components).{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sendemailstosubscriptionowners_csharp">
<a href="#sendemailstosubscriptionowners_csharp" style="color: inherit; text-decoration: inherit;">Send<wbr>Emails<wbr>To<wbr>Subscription<wbr>Owners</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag that indicated whether notifications on this rule should be sent to subscription owners{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="customemails_go">
<a href="#customemails_go" style="color: inherit; text-decoration: inherit;">Custom<wbr>Emails</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}Custom email addresses for this rule notifications{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enabled_go">
<a href="#enabled_go" style="color: inherit; text-decoration: inherit;">Enabled</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag that indicates whether this rule is enabled by the user{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="lastupdatedtime_go">
<a href="#lastupdatedtime_go" style="color: inherit; text-decoration: inherit;">Last<wbr>Updated<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The last time this rule was updated{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ruledefinitions_go">
<a href="#ruledefinitions_go" style="color: inherit; text-decoration: inherit;">Rule<wbr>Definitions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#applicationinsightscomponentproactivedetectionconfigurationresponseruledefinitions">Application<wbr>Insights<wbr>Component<wbr>Proactive<wbr>Detection<wbr>Configuration<wbr>Response<wbr>Rule<wbr>Definitions</a></span>
    </dt>
    <dd>{{% md %}}Static definitions of the ProactiveDetection configuration rule (same values for all components).{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sendemailstosubscriptionowners_go">
<a href="#sendemailstosubscriptionowners_go" style="color: inherit; text-decoration: inherit;">Send<wbr>Emails<wbr>To<wbr>Subscription<wbr>Owners</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag that indicated whether notifications on this rule should be sent to subscription owners{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="customemails_nodejs">
<a href="#customemails_nodejs" style="color: inherit; text-decoration: inherit;">custom<wbr>Emails</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}Custom email addresses for this rule notifications{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enabled_nodejs">
<a href="#enabled_nodejs" style="color: inherit; text-decoration: inherit;">enabled</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A flag that indicates whether this rule is enabled by the user{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="lastupdatedtime_nodejs">
<a href="#lastupdatedtime_nodejs" style="color: inherit; text-decoration: inherit;">last<wbr>Updated<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The last time this rule was updated{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ruledefinitions_nodejs">
<a href="#ruledefinitions_nodejs" style="color: inherit; text-decoration: inherit;">rule<wbr>Definitions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#applicationinsightscomponentproactivedetectionconfigurationresponseruledefinitions">Application<wbr>Insights<wbr>Component<wbr>Proactive<wbr>Detection<wbr>Configuration<wbr>Response<wbr>Rule<wbr>Definitions</a></span>
    </dt>
    <dd>{{% md %}}Static definitions of the ProactiveDetection configuration rule (same values for all components).{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sendemailstosubscriptionowners_nodejs">
<a href="#sendemailstosubscriptionowners_nodejs" style="color: inherit; text-decoration: inherit;">send<wbr>Emails<wbr>To<wbr>Subscription<wbr>Owners</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A flag that indicated whether notifications on this rule should be sent to subscription owners{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="custom_emails_python">
<a href="#custom_emails_python" style="color: inherit; text-decoration: inherit;">custom_<wbr>emails</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Sequence[str]</span>
    </dt>
    <dd>{{% md %}}Custom email addresses for this rule notifications{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="enabled_python">
<a href="#enabled_python" style="color: inherit; text-decoration: inherit;">enabled</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag that indicates whether this rule is enabled by the user{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="last_updated_time_python">
<a href="#last_updated_time_python" style="color: inherit; text-decoration: inherit;">last_<wbr>updated_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The last time this rule was updated{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="rule_definitions_python">
<a href="#rule_definitions_python" style="color: inherit; text-decoration: inherit;">rule_<wbr>definitions</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#applicationinsightscomponentproactivedetectionconfigurationresponseruledefinitions">Application<wbr>Insights<wbr>Component<wbr>Proactive<wbr>Detection<wbr>Configuration<wbr>Response<wbr>Rule<wbr>Definitions</a></span>
    </dt>
    <dd>{{% md %}}Static definitions of the ProactiveDetection configuration rule (same values for all components).{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="send_emails_to_subscription_owners_python">
<a href="#send_emails_to_subscription_owners_python" style="color: inherit; text-decoration: inherit;">send_<wbr>emails_<wbr>to_<wbr>subscription_<wbr>owners</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag that indicated whether notifications on this rule should be sent to subscription owners{{% /md %}}</dd></dl>
{{% /choosable %}}




## Supporting Types


<h4 id="applicationinsightscomponentproactivedetectionconfigurationresponseruledefinitions">Application<wbr>Insights<wbr>Component<wbr>Proactive<wbr>Detection<wbr>Configuration<wbr>Response<wbr>Rule<wbr>Definitions</h4>



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="description_csharp">
<a href="#description_csharp" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule description{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="displayname_csharp">
<a href="#displayname_csharp" style="color: inherit; text-decoration: inherit;">Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name as it is displayed in UI{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="helpurl_csharp">
<a href="#helpurl_csharp" style="color: inherit; text-decoration: inherit;">Help<wbr>Url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL which displays additional info about the proactive detection rule{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="isenabledbydefault_csharp">
<a href="#isenabledbydefault_csharp" style="color: inherit; text-decoration: inherit;">Is<wbr>Enabled<wbr>By<wbr>Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is enabled by default{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="ishidden_csharp">
<a href="#ishidden_csharp" style="color: inherit; text-decoration: inherit;">Is<wbr>Hidden</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is hidden (from the UI){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="isinpreview_csharp">
<a href="#isinpreview_csharp" style="color: inherit; text-decoration: inherit;">Is<wbr>In<wbr>Preview</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is in preview{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="supportsemailnotifications_csharp">
<a href="#supportsemailnotifications_csharp" style="color: inherit; text-decoration: inherit;">Supports<wbr>Email<wbr>Notifications</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether email notifications are supported for detections for this rule{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="description_go">
<a href="#description_go" style="color: inherit; text-decoration: inherit;">Description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule description{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="displayname_go">
<a href="#displayname_go" style="color: inherit; text-decoration: inherit;">Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name as it is displayed in UI{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="helpurl_go">
<a href="#helpurl_go" style="color: inherit; text-decoration: inherit;">Help<wbr>Url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL which displays additional info about the proactive detection rule{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="isenabledbydefault_go">
<a href="#isenabledbydefault_go" style="color: inherit; text-decoration: inherit;">Is<wbr>Enabled<wbr>By<wbr>Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is enabled by default{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="ishidden_go">
<a href="#ishidden_go" style="color: inherit; text-decoration: inherit;">Is<wbr>Hidden</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is hidden (from the UI){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="isinpreview_go">
<a href="#isinpreview_go" style="color: inherit; text-decoration: inherit;">Is<wbr>In<wbr>Preview</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is in preview{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="supportsemailnotifications_go">
<a href="#supportsemailnotifications_go" style="color: inherit; text-decoration: inherit;">Supports<wbr>Email<wbr>Notifications</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether email notifications are supported for detections for this rule{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="description_nodejs">
<a href="#description_nodejs" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule description{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="displayname_nodejs">
<a href="#displayname_nodejs" style="color: inherit; text-decoration: inherit;">display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name as it is displayed in UI{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="helpurl_nodejs">
<a href="#helpurl_nodejs" style="color: inherit; text-decoration: inherit;">help<wbr>Url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL which displays additional info about the proactive detection rule{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="isenabledbydefault_nodejs">
<a href="#isenabledbydefault_nodejs" style="color: inherit; text-decoration: inherit;">is<wbr>Enabled<wbr>By<wbr>Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is enabled by default{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="ishidden_nodejs">
<a href="#ishidden_nodejs" style="color: inherit; text-decoration: inherit;">is<wbr>Hidden</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is hidden (from the UI){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="isinpreview_nodejs">
<a href="#isinpreview_nodejs" style="color: inherit; text-decoration: inherit;">is<wbr>In<wbr>Preview</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is in preview{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="supportsemailnotifications_nodejs">
<a href="#supportsemailnotifications_nodejs" style="color: inherit; text-decoration: inherit;">supports<wbr>Email<wbr>Notifications</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether email notifications are supported for detections for this rule{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="description_python">
<a href="#description_python" style="color: inherit; text-decoration: inherit;">description</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The rule description{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="display_name_python">
<a href="#display_name_python" style="color: inherit; text-decoration: inherit;">display_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The rule name as it is displayed in UI{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="help_url_python">
<a href="#help_url_python" style="color: inherit; text-decoration: inherit;">help_<wbr>url</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}URL which displays additional info about the proactive detection rule{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="is_enabled_by_default_python">
<a href="#is_enabled_by_default_python" style="color: inherit; text-decoration: inherit;">is_<wbr>enabled_<wbr>by_<wbr>default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is enabled by default{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="is_hidden_python">
<a href="#is_hidden_python" style="color: inherit; text-decoration: inherit;">is_<wbr>hidden</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is hidden (from the UI){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="is_in_preview_python">
<a href="#is_in_preview_python" style="color: inherit; text-decoration: inherit;">is_<wbr>in_<wbr>preview</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether the rule is in preview{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The rule name{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="supports_email_notifications_python">
<a href="#supports_email_notifications_python" style="color: inherit; text-decoration: inherit;">supports_<wbr>email_<wbr>notifications</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A flag indicating whether email notifications are supported for detections for this rule{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

