
---
title: "getPrivateStoreOffer"
title_tag: "azure-native.marketplace.getPrivateStoreOffer"
meta_desc: "Documentation for the azure-native.marketplace.getPrivateStoreOffer function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

The privateStore offer data structure.
API Version: 2020-01-01.




## Using getPrivateStoreOffer {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getPrivateStoreOffer<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetPrivateStoreOfferArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetPrivateStoreOfferResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_private_store_offer(</span><span class="nx">offer_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">private_store_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetPrivateStoreOfferResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupPrivateStoreOffer<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupPrivateStoreOfferArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupPrivateStoreOfferResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupPrivateStoreOffer` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetPrivateStoreOffer </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetPrivateStoreOfferResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetPrivateStoreOfferArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="offerid_csharp">
<a href="#offerid_csharp" style="color: inherit; text-decoration: inherit;">Offer<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The offer ID to update or delete{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="privatestoreid_csharp">
<a href="#privatestoreid_csharp" style="color: inherit; text-decoration: inherit;">Private<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The store ID - must use the tenant ID{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="offerid_go">
<a href="#offerid_go" style="color: inherit; text-decoration: inherit;">Offer<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The offer ID to update or delete{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="privatestoreid_go">
<a href="#privatestoreid_go" style="color: inherit; text-decoration: inherit;">Private<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The store ID - must use the tenant ID{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="offerid_nodejs">
<a href="#offerid_nodejs" style="color: inherit; text-decoration: inherit;">offer<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The offer ID to update or delete{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="privatestoreid_nodejs">
<a href="#privatestoreid_nodejs" style="color: inherit; text-decoration: inherit;">private<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The store ID - must use the tenant ID{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="offer_id_python">
<a href="#offer_id_python" style="color: inherit; text-decoration: inherit;">offer_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The offer ID to update or delete{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="private_store_id_python">
<a href="#private_store_id_python" style="color: inherit; text-decoration: inherit;">private_<wbr>store_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The store ID - must use the tenant ID{{% /md %}}</dd></dl>
{{% /choosable %}}




## getPrivateStoreOffer Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="createdat_csharp">
<a href="#createdat_csharp" style="color: inherit; text-decoration: inherit;">Created<wbr>At</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store offer creation date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource ID.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="modifiedat_csharp">
<a href="#modifiedat_csharp" style="color: inherit; text-decoration: inherit;">Modified<wbr>At</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store offer modification date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="offerdisplayname_csharp">
<a href="#offerdisplayname_csharp" style="color: inherit; text-decoration: inherit;">Offer<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}It will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="privatestoreid_csharp">
<a href="#privatestoreid_csharp" style="color: inherit; text-decoration: inherit;">Private<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="publisherdisplayname_csharp">
<a href="#publisherdisplayname_csharp" style="color: inherit; text-decoration: inherit;">Publisher<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Publisher name that will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="uniqueofferid_csharp">
<a href="#uniqueofferid_csharp" style="color: inherit; text-decoration: inherit;">Unique<wbr>Offer<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Offers unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="etag_csharp">
<a href="#etag_csharp" style="color: inherit; text-decoration: inherit;">ETag</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Identifier for purposes of race condition{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="iconfileuris_csharp">
<a href="#iconfileuris_csharp" style="color: inherit; text-decoration: inherit;">Icon<wbr>File<wbr>Uris</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}Icon File Uris{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="plans_csharp">
<a href="#plans_csharp" style="color: inherit; text-decoration: inherit;">Plans</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#planresponse">List&lt;Pulumi.<wbr>Azure<wbr>Native.<wbr>Marketplace.<wbr>Outputs.<wbr>Plan<wbr>Response&gt;</a></span>
    </dt>
    <dd>{{% md %}}Offer plans{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="specificplanidslimitation_csharp">
<a href="#specificplanidslimitation_csharp" style="color: inherit; text-decoration: inherit;">Specific<wbr>Plan<wbr>Ids<wbr>Limitation</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}Plan ids limitation for this offer{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updatesuppresseddueidempotence_csharp">
<a href="#updatesuppresseddueidempotence_csharp" style="color: inherit; text-decoration: inherit;">Update<wbr>Suppressed<wbr>Due<wbr>Idempotence</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicating whether the offer was not updated to db (true = not updated). If the allow list is identical to the existed one in db, the offer would not be updated.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="createdat_go">
<a href="#createdat_go" style="color: inherit; text-decoration: inherit;">Created<wbr>At</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store offer creation date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource ID.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="modifiedat_go">
<a href="#modifiedat_go" style="color: inherit; text-decoration: inherit;">Modified<wbr>At</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store offer modification date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="offerdisplayname_go">
<a href="#offerdisplayname_go" style="color: inherit; text-decoration: inherit;">Offer<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}It will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="privatestoreid_go">
<a href="#privatestoreid_go" style="color: inherit; text-decoration: inherit;">Private<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="publisherdisplayname_go">
<a href="#publisherdisplayname_go" style="color: inherit; text-decoration: inherit;">Publisher<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Publisher name that will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="uniqueofferid_go">
<a href="#uniqueofferid_go" style="color: inherit; text-decoration: inherit;">Unique<wbr>Offer<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Offers unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="etag_go">
<a href="#etag_go" style="color: inherit; text-decoration: inherit;">ETag</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Identifier for purposes of race condition{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="iconfileuris_go">
<a href="#iconfileuris_go" style="color: inherit; text-decoration: inherit;">Icon<wbr>File<wbr>Uris</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}Icon File Uris{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="plans_go">
<a href="#plans_go" style="color: inherit; text-decoration: inherit;">Plans</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#planresponse">[]Plan<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}Offer plans{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="specificplanidslimitation_go">
<a href="#specificplanidslimitation_go" style="color: inherit; text-decoration: inherit;">Specific<wbr>Plan<wbr>Ids<wbr>Limitation</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}Plan ids limitation for this offer{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updatesuppresseddueidempotence_go">
<a href="#updatesuppresseddueidempotence_go" style="color: inherit; text-decoration: inherit;">Update<wbr>Suppressed<wbr>Due<wbr>Idempotence</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicating whether the offer was not updated to db (true = not updated). If the allow list is identical to the existed one in db, the offer would not be updated.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="createdat_nodejs">
<a href="#createdat_nodejs" style="color: inherit; text-decoration: inherit;">created<wbr>At</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store offer creation date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The resource ID.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="modifiedat_nodejs">
<a href="#modifiedat_nodejs" style="color: inherit; text-decoration: inherit;">modified<wbr>At</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store offer modification date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="offerdisplayname_nodejs">
<a href="#offerdisplayname_nodejs" style="color: inherit; text-decoration: inherit;">offer<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}It will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="privatestoreid_nodejs">
<a href="#privatestoreid_nodejs" style="color: inherit; text-decoration: inherit;">private<wbr>Store<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Private store unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="publisherdisplayname_nodejs">
<a href="#publisherdisplayname_nodejs" style="color: inherit; text-decoration: inherit;">publisher<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Publisher name that will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="uniqueofferid_nodejs">
<a href="#uniqueofferid_nodejs" style="color: inherit; text-decoration: inherit;">unique<wbr>Offer<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Offers unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="etag_nodejs">
<a href="#etag_nodejs" style="color: inherit; text-decoration: inherit;">e<wbr>Tag</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Identifier for purposes of race condition{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="iconfileuris_nodejs">
<a href="#iconfileuris_nodejs" style="color: inherit; text-decoration: inherit;">icon<wbr>File<wbr>Uris</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}Icon File Uris{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="plans_nodejs">
<a href="#plans_nodejs" style="color: inherit; text-decoration: inherit;">plans</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#planresponse">Plan<wbr>Response[]</a></span>
    </dt>
    <dd>{{% md %}}Offer plans{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="specificplanidslimitation_nodejs">
<a href="#specificplanidslimitation_nodejs" style="color: inherit; text-decoration: inherit;">specific<wbr>Plan<wbr>Ids<wbr>Limitation</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}Plan ids limitation for this offer{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="updatesuppresseddueidempotence_nodejs">
<a href="#updatesuppresseddueidempotence_nodejs" style="color: inherit; text-decoration: inherit;">update<wbr>Suppressed<wbr>Due<wbr>Idempotence</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Indicating whether the offer was not updated to db (true = not updated). If the allow list is identical to the existed one in db, the offer would not be updated.{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="created_at_python">
<a href="#created_at_python" style="color: inherit; text-decoration: inherit;">created_<wbr>at</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Private store offer creation date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The resource ID.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="modified_at_python">
<a href="#modified_at_python" style="color: inherit; text-decoration: inherit;">modified_<wbr>at</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Private store offer modification date{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="offer_display_name_python">
<a href="#offer_display_name_python" style="color: inherit; text-decoration: inherit;">offer_<wbr>display_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}It will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="private_store_id_python">
<a href="#private_store_id_python" style="color: inherit; text-decoration: inherit;">private_<wbr>store_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Private store unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="publisher_display_name_python">
<a href="#publisher_display_name_python" style="color: inherit; text-decoration: inherit;">publisher_<wbr>display_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Publisher name that will be displayed prominently in the marketplace{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of the resource.{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="unique_offer_id_python">
<a href="#unique_offer_id_python" style="color: inherit; text-decoration: inherit;">unique_<wbr>offer_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Offers unique id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="e_tag_python">
<a href="#e_tag_python" style="color: inherit; text-decoration: inherit;">e_<wbr>tag</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Identifier for purposes of race condition{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="icon_file_uris_python">
<a href="#icon_file_uris_python" style="color: inherit; text-decoration: inherit;">icon_<wbr>file_<wbr>uris</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}Icon File Uris{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="plans_python">
<a href="#plans_python" style="color: inherit; text-decoration: inherit;">plans</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#planresponse">Sequence[Plan<wbr>Response]</a></span>
    </dt>
    <dd>{{% md %}}Offer plans{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="specific_plan_ids_limitation_python">
<a href="#specific_plan_ids_limitation_python" style="color: inherit; text-decoration: inherit;">specific_<wbr>plan_<wbr>ids_<wbr>limitation</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Sequence[str]</span>
    </dt>
    <dd>{{% md %}}Plan ids limitation for this offer{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="update_suppressed_due_idempotence_python">
<a href="#update_suppressed_due_idempotence_python" style="color: inherit; text-decoration: inherit;">update_<wbr>suppressed_<wbr>due_<wbr>idempotence</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Indicating whether the offer was not updated to db (true = not updated). If the allow list is identical to the existed one in db, the offer would not be updated.{{% /md %}}</dd></dl>
{{% /choosable %}}




## Supporting Types


<h4 id="planresponse">Plan<wbr>Response</h4>



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="altstackreference_csharp">
<a href="#altstackreference_csharp" style="color: inherit; text-decoration: inherit;">Alt<wbr>Stack<wbr>Reference</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Alternative stack type{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="plandisplayname_csharp">
<a href="#plandisplayname_csharp" style="color: inherit; text-decoration: inherit;">Plan<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Friendly name for the plan for display in the marketplace{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="planid_csharp">
<a href="#planid_csharp" style="color: inherit; text-decoration: inherit;">Plan<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Text identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="skuid_csharp">
<a href="#skuid_csharp" style="color: inherit; text-decoration: inherit;">Sku<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="stacktype_csharp">
<a href="#stacktype_csharp" style="color: inherit; text-decoration: inherit;">Stack<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Stack type (classic or arm){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="accessibility_csharp">
<a href="#accessibility_csharp" style="color: inherit; text-decoration: inherit;">Accessibility</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Plan accessibility{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="altstackreference_go">
<a href="#altstackreference_go" style="color: inherit; text-decoration: inherit;">Alt<wbr>Stack<wbr>Reference</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Alternative stack type{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="plandisplayname_go">
<a href="#plandisplayname_go" style="color: inherit; text-decoration: inherit;">Plan<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Friendly name for the plan for display in the marketplace{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="planid_go">
<a href="#planid_go" style="color: inherit; text-decoration: inherit;">Plan<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Text identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="skuid_go">
<a href="#skuid_go" style="color: inherit; text-decoration: inherit;">Sku<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="stacktype_go">
<a href="#stacktype_go" style="color: inherit; text-decoration: inherit;">Stack<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Stack type (classic or arm){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="accessibility_go">
<a href="#accessibility_go" style="color: inherit; text-decoration: inherit;">Accessibility</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Plan accessibility{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="altstackreference_nodejs">
<a href="#altstackreference_nodejs" style="color: inherit; text-decoration: inherit;">alt<wbr>Stack<wbr>Reference</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Alternative stack type{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="plandisplayname_nodejs">
<a href="#plandisplayname_nodejs" style="color: inherit; text-decoration: inherit;">plan<wbr>Display<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Friendly name for the plan for display in the marketplace{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="planid_nodejs">
<a href="#planid_nodejs" style="color: inherit; text-decoration: inherit;">plan<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Text identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="skuid_nodejs">
<a href="#skuid_nodejs" style="color: inherit; text-decoration: inherit;">sku<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="stacktype_nodejs">
<a href="#stacktype_nodejs" style="color: inherit; text-decoration: inherit;">stack<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Stack type (classic or arm){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="accessibility_nodejs">
<a href="#accessibility_nodejs" style="color: inherit; text-decoration: inherit;">accessibility</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Plan accessibility{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="alt_stack_reference_python">
<a href="#alt_stack_reference_python" style="color: inherit; text-decoration: inherit;">alt_<wbr>stack_<wbr>reference</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Alternative stack type{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="plan_display_name_python">
<a href="#plan_display_name_python" style="color: inherit; text-decoration: inherit;">plan_<wbr>display_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Friendly name for the plan for display in the marketplace{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="plan_id_python">
<a href="#plan_id_python" style="color: inherit; text-decoration: inherit;">plan_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Text identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="sku_id_python">
<a href="#sku_id_python" style="color: inherit; text-decoration: inherit;">sku_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Identifier for this plan{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="stack_type_python">
<a href="#stack_type_python" style="color: inherit; text-decoration: inherit;">stack_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Stack type (classic or arm){{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="accessibility_python">
<a href="#accessibility_python" style="color: inherit; text-decoration: inherit;">accessibility</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Plan accessibility{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

