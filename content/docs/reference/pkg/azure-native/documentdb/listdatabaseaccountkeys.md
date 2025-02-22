
---
title: "listDatabaseAccountKeys"
title_tag: "azure-native.documentdb.listDatabaseAccountKeys"
meta_desc: "Documentation for the azure-native.documentdb.listDatabaseAccountKeys function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

The access keys for the given database account.
API Version: 2021-03-15.




## Using listDatabaseAccountKeys {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>listDatabaseAccountKeys<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">ListDatabaseAccountKeysArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">ListDatabaseAccountKeysResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>list_database_account_keys(</span><span class="nx">account_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> ListDatabaseAccountKeysResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>ListDatabaseAccountKeys<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">ListDatabaseAccountKeysArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">ListDatabaseAccountKeysResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `ListDatabaseAccountKeys` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">ListDatabaseAccountKeys </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">ListDatabaseAccountKeysResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">ListDatabaseAccountKeysArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="accountname_csharp">
<a href="#accountname_csharp" style="color: inherit; text-decoration: inherit;">Account<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Cosmos DB database account name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="accountname_go">
<a href="#accountname_go" style="color: inherit; text-decoration: inherit;">Account<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Cosmos DB database account name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="accountname_nodejs">
<a href="#accountname_nodejs" style="color: inherit; text-decoration: inherit;">account<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Cosmos DB database account name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="account_name_python">
<a href="#account_name_python" style="color: inherit; text-decoration: inherit;">account_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Cosmos DB database account name.{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group. The name is case insensitive.{{% /md %}}</dd></dl>
{{% /choosable %}}




## listDatabaseAccountKeys Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="primarymasterkey_csharp">
<a href="#primarymasterkey_csharp" style="color: inherit; text-decoration: inherit;">Primary<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="primaryreadonlymasterkey_csharp">
<a href="#primaryreadonlymasterkey_csharp" style="color: inherit; text-decoration: inherit;">Primary<wbr>Readonly<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-only key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondarymasterkey_csharp">
<a href="#secondarymasterkey_csharp" style="color: inherit; text-decoration: inherit;">Secondary<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondaryreadonlymasterkey_csharp">
<a href="#secondaryreadonlymasterkey_csharp" style="color: inherit; text-decoration: inherit;">Secondary<wbr>Readonly<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-only key.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="primarymasterkey_go">
<a href="#primarymasterkey_go" style="color: inherit; text-decoration: inherit;">Primary<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="primaryreadonlymasterkey_go">
<a href="#primaryreadonlymasterkey_go" style="color: inherit; text-decoration: inherit;">Primary<wbr>Readonly<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-only key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondarymasterkey_go">
<a href="#secondarymasterkey_go" style="color: inherit; text-decoration: inherit;">Secondary<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondaryreadonlymasterkey_go">
<a href="#secondaryreadonlymasterkey_go" style="color: inherit; text-decoration: inherit;">Secondary<wbr>Readonly<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-only key.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="primarymasterkey_nodejs">
<a href="#primarymasterkey_nodejs" style="color: inherit; text-decoration: inherit;">primary<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="primaryreadonlymasterkey_nodejs">
<a href="#primaryreadonlymasterkey_nodejs" style="color: inherit; text-decoration: inherit;">primary<wbr>Readonly<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-only key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondarymasterkey_nodejs">
<a href="#secondarymasterkey_nodejs" style="color: inherit; text-decoration: inherit;">secondary<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondaryreadonlymasterkey_nodejs">
<a href="#secondaryreadonlymasterkey_nodejs" style="color: inherit; text-decoration: inherit;">secondary<wbr>Readonly<wbr>Master<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-only key.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="primary_master_key_python">
<a href="#primary_master_key_python" style="color: inherit; text-decoration: inherit;">primary_<wbr>master_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="primary_readonly_master_key_python">
<a href="#primary_readonly_master_key_python" style="color: inherit; text-decoration: inherit;">primary_<wbr>readonly_<wbr>master_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the primary read-only key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondary_master_key_python">
<a href="#secondary_master_key_python" style="color: inherit; text-decoration: inherit;">secondary_<wbr>master_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-write key.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="secondary_readonly_master_key_python">
<a href="#secondary_readonly_master_key_python" style="color: inherit; text-decoration: inherit;">secondary_<wbr>readonly_<wbr>master_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Base 64 encoded value of the secondary read-only key.{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

