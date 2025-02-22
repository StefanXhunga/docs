
---
title: "getDomainName"
title_tag: "aws.apigateway.getDomainName"
meta_desc: "Documentation for the aws.apigateway.getDomainName function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Use this data source to get the custom domain name for use with AWS API Gateway.


{{% examples %}}

## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}





{{< example csharp >}}

```csharp
using Pulumi;
using Aws = Pulumi.Aws;

class MyStack : Stack
{
    public MyStack()
    {
        var example = Output.Create(Aws.ApiGateway.GetDomainName.InvokeAsync(new Aws.ApiGateway.GetDomainNameArgs
        {
            DomainName = "api.example.com",
        }));
    }

}
```


{{< /example >}}


{{< example go >}}

```go
package main

import (
	"github.com/pulumi/pulumi-aws/sdk/v3/go/aws/apigateway"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := apigateway.LookupDomainName(ctx, &apigateway.LookupDomainNameArgs{
			DomainName: "api.example.com",
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
import pulumi_aws as aws

example = aws.apigateway.get_domain_name(domain_name="api.example.com")
```


{{< /example >}}


{{< example typescript >}}


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const example = pulumi.output(aws.apigateway.getDomainName({
    domainName: "api.example.com",
}, { async: true }));
```


{{< /example >}}





{{% /examples %}}




## Using getDomainName {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getDomainName<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetDomainNameArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetDomainNameResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_domain_name(</span><span class="nx">domain_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">tags</span><span class="p">:</span> <span class="nx">Optional[Mapping[str, str]]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetDomainNameResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupDomainName<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupDomainNameArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupDomainNameResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupDomainName` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetDomainName </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetDomainNameResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetDomainNameArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="domainname_csharp">
<a href="#domainname_csharp" style="color: inherit; text-decoration: inherit;">Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The fully-qualified domain name to look up. If no domain name is found, an error will be returned.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_csharp">
<a href="#tags_csharp" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="domainname_go">
<a href="#domainname_go" style="color: inherit; text-decoration: inherit;">Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The fully-qualified domain name to look up. If no domain name is found, an error will be returned.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_go">
<a href="#tags_go" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="domainname_nodejs">
<a href="#domainname_nodejs" style="color: inherit; text-decoration: inherit;">domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The fully-qualified domain name to look up. If no domain name is found, an error will be returned.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_nodejs">
<a href="#tags_nodejs" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="domain_name_python">
<a href="#domain_name_python" style="color: inherit; text-decoration: inherit;">domain_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The fully-qualified domain name to look up. If no domain name is found, an error will be returned.
{{% /md %}}</dd><dt class="property-optional"
            title="Optional">
        <span id="tags_python">
<a href="#tags_python" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}




## getDomainName Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="arn_csharp">
<a href="#arn_csharp" style="color: inherit; text-decoration: inherit;">Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN of the found custom domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificatearn_csharp">
<a href="#certificatearn_csharp" style="color: inherit; text-decoration: inherit;">Certificate<wbr>Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificatename_csharp">
<a href="#certificatename_csharp" style="color: inherit; text-decoration: inherit;">Certificate<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificateuploaddate_csharp">
<a href="#certificateuploaddate_csharp" style="color: inherit; text-decoration: inherit;">Certificate<wbr>Upload<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The upload date associated with the domain certificate.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfrontdomainname_csharp">
<a href="#cloudfrontdomainname_csharp" style="color: inherit; text-decoration: inherit;">Cloudfront<wbr>Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hostname created by Cloudfront to represent the distribution that implements this domain name mapping.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfrontzoneid_csharp">
<a href="#cloudfrontzoneid_csharp" style="color: inherit; text-decoration: inherit;">Cloudfront<wbr>Zone<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}For convenience, the hosted zone ID (`Z2FDTNDATAQYW2`) that can be used to create a Route53 alias record for the distribution.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="domainname_csharp">
<a href="#domainname_csharp" style="color: inherit; text-decoration: inherit;">Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="endpointconfigurations_csharp">
<a href="#endpointconfigurations_csharp" style="color: inherit; text-decoration: inherit;">Endpoint<wbr>Configurations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getdomainnameendpointconfiguration">List&lt;Get<wbr>Domain<wbr>Name<wbr>Endpoint<wbr>Configuration&gt;</a></span>
    </dt>
    <dd>{{% md %}}List of objects with the endpoint configuration of this domain name.
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
        <span id="regionalcertificatearn_csharp">
<a href="#regionalcertificatearn_csharp" style="color: inherit; text-decoration: inherit;">Regional<wbr>Certificate<wbr>Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used for validating the regional domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionalcertificatename_csharp">
<a href="#regionalcertificatename_csharp" style="color: inherit; text-decoration: inherit;">Regional<wbr>Certificate<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user-friendly name of the certificate that is used by regional endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionaldomainname_csharp">
<a href="#regionaldomainname_csharp" style="color: inherit; text-decoration: inherit;">Regional<wbr>Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hostname for the custom domain's regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionalzoneid_csharp">
<a href="#regionalzoneid_csharp" style="color: inherit; text-decoration: inherit;">Regional<wbr>Zone<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hosted zone ID that can be used to create a Route53 alias record for the regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="securitypolicy_csharp">
<a href="#securitypolicy_csharp" style="color: inherit; text-decoration: inherit;">Security<wbr>Policy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The security policy for the domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tags_csharp">
<a href="#tags_csharp" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="arn_go">
<a href="#arn_go" style="color: inherit; text-decoration: inherit;">Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN of the found custom domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificatearn_go">
<a href="#certificatearn_go" style="color: inherit; text-decoration: inherit;">Certificate<wbr>Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificatename_go">
<a href="#certificatename_go" style="color: inherit; text-decoration: inherit;">Certificate<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificateuploaddate_go">
<a href="#certificateuploaddate_go" style="color: inherit; text-decoration: inherit;">Certificate<wbr>Upload<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The upload date associated with the domain certificate.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfrontdomainname_go">
<a href="#cloudfrontdomainname_go" style="color: inherit; text-decoration: inherit;">Cloudfront<wbr>Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hostname created by Cloudfront to represent the distribution that implements this domain name mapping.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfrontzoneid_go">
<a href="#cloudfrontzoneid_go" style="color: inherit; text-decoration: inherit;">Cloudfront<wbr>Zone<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}For convenience, the hosted zone ID (`Z2FDTNDATAQYW2`) that can be used to create a Route53 alias record for the distribution.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="domainname_go">
<a href="#domainname_go" style="color: inherit; text-decoration: inherit;">Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="endpointconfigurations_go">
<a href="#endpointconfigurations_go" style="color: inherit; text-decoration: inherit;">Endpoint<wbr>Configurations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getdomainnameendpointconfiguration">[]Get<wbr>Domain<wbr>Name<wbr>Endpoint<wbr>Configuration</a></span>
    </dt>
    <dd>{{% md %}}List of objects with the endpoint configuration of this domain name.
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
        <span id="regionalcertificatearn_go">
<a href="#regionalcertificatearn_go" style="color: inherit; text-decoration: inherit;">Regional<wbr>Certificate<wbr>Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used for validating the regional domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionalcertificatename_go">
<a href="#regionalcertificatename_go" style="color: inherit; text-decoration: inherit;">Regional<wbr>Certificate<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user-friendly name of the certificate that is used by regional endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionaldomainname_go">
<a href="#regionaldomainname_go" style="color: inherit; text-decoration: inherit;">Regional<wbr>Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hostname for the custom domain's regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionalzoneid_go">
<a href="#regionalzoneid_go" style="color: inherit; text-decoration: inherit;">Regional<wbr>Zone<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hosted zone ID that can be used to create a Route53 alias record for the regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="securitypolicy_go">
<a href="#securitypolicy_go" style="color: inherit; text-decoration: inherit;">Security<wbr>Policy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The security policy for the domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tags_go">
<a href="#tags_go" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="arn_nodejs">
<a href="#arn_nodejs" style="color: inherit; text-decoration: inherit;">arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN of the found custom domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificatearn_nodejs">
<a href="#certificatearn_nodejs" style="color: inherit; text-decoration: inherit;">certificate<wbr>Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificatename_nodejs">
<a href="#certificatename_nodejs" style="color: inherit; text-decoration: inherit;">certificate<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificateuploaddate_nodejs">
<a href="#certificateuploaddate_nodejs" style="color: inherit; text-decoration: inherit;">certificate<wbr>Upload<wbr>Date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The upload date associated with the domain certificate.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfrontdomainname_nodejs">
<a href="#cloudfrontdomainname_nodejs" style="color: inherit; text-decoration: inherit;">cloudfront<wbr>Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hostname created by Cloudfront to represent the distribution that implements this domain name mapping.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfrontzoneid_nodejs">
<a href="#cloudfrontzoneid_nodejs" style="color: inherit; text-decoration: inherit;">cloudfront<wbr>Zone<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}For convenience, the hosted zone ID (`Z2FDTNDATAQYW2`) that can be used to create a Route53 alias record for the distribution.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="domainname_nodejs">
<a href="#domainname_nodejs" style="color: inherit; text-decoration: inherit;">domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="endpointconfigurations_nodejs">
<a href="#endpointconfigurations_nodejs" style="color: inherit; text-decoration: inherit;">endpoint<wbr>Configurations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getdomainnameendpointconfiguration">Get<wbr>Domain<wbr>Name<wbr>Endpoint<wbr>Configuration[]</a></span>
    </dt>
    <dd>{{% md %}}List of objects with the endpoint configuration of this domain name.
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
        <span id="regionalcertificatearn_nodejs">
<a href="#regionalcertificatearn_nodejs" style="color: inherit; text-decoration: inherit;">regional<wbr>Certificate<wbr>Arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used for validating the regional domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionalcertificatename_nodejs">
<a href="#regionalcertificatename_nodejs" style="color: inherit; text-decoration: inherit;">regional<wbr>Certificate<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The user-friendly name of the certificate that is used by regional endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionaldomainname_nodejs">
<a href="#regionaldomainname_nodejs" style="color: inherit; text-decoration: inherit;">regional<wbr>Domain<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hostname for the custom domain's regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regionalzoneid_nodejs">
<a href="#regionalzoneid_nodejs" style="color: inherit; text-decoration: inherit;">regional<wbr>Zone<wbr>Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The hosted zone ID that can be used to create a Route53 alias record for the regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="securitypolicy_nodejs">
<a href="#securitypolicy_nodejs" style="color: inherit; text-decoration: inherit;">security<wbr>Policy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The security policy for the domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tags_nodejs">
<a href="#tags_nodejs" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="arn_python">
<a href="#arn_python" style="color: inherit; text-decoration: inherit;">arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ARN of the found custom domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificate_arn_python">
<a href="#certificate_arn_python" style="color: inherit; text-decoration: inherit;">certificate_<wbr>arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificate_name_python">
<a href="#certificate_name_python" style="color: inherit; text-decoration: inherit;">certificate_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the certificate that is used by edge-optimized endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="certificate_upload_date_python">
<a href="#certificate_upload_date_python" style="color: inherit; text-decoration: inherit;">certificate_<wbr>upload_<wbr>date</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The upload date associated with the domain certificate.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfront_domain_name_python">
<a href="#cloudfront_domain_name_python" style="color: inherit; text-decoration: inherit;">cloudfront_<wbr>domain_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The hostname created by Cloudfront to represent the distribution that implements this domain name mapping.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="cloudfront_zone_id_python">
<a href="#cloudfront_zone_id_python" style="color: inherit; text-decoration: inherit;">cloudfront_<wbr>zone_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}For convenience, the hosted zone ID (`Z2FDTNDATAQYW2`) that can be used to create a Route53 alias record for the distribution.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="domain_name_python">
<a href="#domain_name_python" style="color: inherit; text-decoration: inherit;">domain_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="endpoint_configurations_python">
<a href="#endpoint_configurations_python" style="color: inherit; text-decoration: inherit;">endpoint_<wbr>configurations</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getdomainnameendpointconfiguration">Sequence[Get<wbr>Domain<wbr>Name<wbr>Endpoint<wbr>Configuration]</a></span>
    </dt>
    <dd>{{% md %}}List of objects with the endpoint configuration of this domain name.
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
        <span id="regional_certificate_arn_python">
<a href="#regional_certificate_arn_python" style="color: inherit; text-decoration: inherit;">regional_<wbr>certificate_<wbr>arn</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ARN for an AWS-managed certificate that is used for validating the regional domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regional_certificate_name_python">
<a href="#regional_certificate_name_python" style="color: inherit; text-decoration: inherit;">regional_<wbr>certificate_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The user-friendly name of the certificate that is used by regional endpoint for this domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regional_domain_name_python">
<a href="#regional_domain_name_python" style="color: inherit; text-decoration: inherit;">regional_<wbr>domain_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The hostname for the custom domain's regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="regional_zone_id_python">
<a href="#regional_zone_id_python" style="color: inherit; text-decoration: inherit;">regional_<wbr>zone_<wbr>id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The hosted zone ID that can be used to create a Route53 alias record for the regional endpoint.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="security_policy_python">
<a href="#security_policy_python" style="color: inherit; text-decoration: inherit;">security_<wbr>policy</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The security policy for the domain name.
{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tags_python">
<a href="#tags_python" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}Key-value map of tags for the resource.
{{% /md %}}</dd></dl>
{{% /choosable %}}




## Supporting Types


<h4 id="getdomainnameendpointconfiguration">Get<wbr>Domain<wbr>Name<wbr>Endpoint<wbr>Configuration</h4>



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="types_csharp">
<a href="#types_csharp" style="color: inherit; text-decoration: inherit;">Types</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}List of endpoint types.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="types_go">
<a href="#types_go" style="color: inherit; text-decoration: inherit;">Types</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}List of endpoint types.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="types_nodejs">
<a href="#types_nodejs" style="color: inherit; text-decoration: inherit;">types</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}List of endpoint types.
{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="types_python">
<a href="#types_python" style="color: inherit; text-decoration: inherit;">types</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Sequence[str]</span>
    </dt>
    <dd>{{% md %}}List of endpoint types.
{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-aws">https://github.com/pulumi/pulumi-aws</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`aws` Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws).{{% /md %}}</dd>
</dl>

