
---
title: "RateLimit"
block_external_search_index: true
---



Provides a Cloudflare rate limit resource for a given zone. This can be used to limit the traffic you receive zone-wide, or matching more specific types of requests/responses.

> This content is derived from https://github.com/terraform-providers/terraform-provider-cloudflare/blob/master/website/docs/r/rate_limit.html.markdown.



## Create a RateLimit Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/#RateLimit">RateLimit</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/#RateLimitArgs">RateLimitArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">RateLimit</span><span class="p">(resource_name, opts=None, </span>action=None<span class="p">, </span>bypass_url_patterns=None<span class="p">, </span>correlate=None<span class="p">, </span>description=None<span class="p">, </span>disabled=None<span class="p">, </span>match=None<span class="p">, </span>period=None<span class="p">, </span>threshold=None<span class="p">, </span>zone_id=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewRateLimit<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitArgs">RateLimitArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimit">RateLimit</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Cloudflare/Pulumi.Cloudflare.RateLimit.html">RateLimit</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Cloudflare/Pulumi.Cloudflare.RateLimitArgs.html">RateLimitArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
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
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
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
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Rate<wbr>Limit<wbr>Action<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Period</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Zone<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bypass<wbr>Url<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Rate<wbr>Limit<wbr>Correlate<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Rate<wbr>Limit<wbr>Match<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Rate<wbr>Limit<wbr>Action</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Period</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Zone<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bypass<wbr>Url<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Rate<wbr>Limit<wbr>Correlate</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Rate<wbr>Limit<wbr>Match</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Rate<wbr>Limit<wbr>Action</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>period</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>zone<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bypass<wbr>Url<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Rate<wbr>Limit<wbr>Correlate</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Rate<wbr>Limit<wbr>Match</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Dict[Rate<wbr>Limit<wbr>Action]</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>period</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>zone_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bypass_<wbr>url_<wbr>patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Dict[Rate<wbr>Limit<wbr>Correlate]</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Dict[Rate<wbr>Limit<wbr>Match]</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Look up an Existing RateLimit Resource

Get an existing RateLimit resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/#RateLimitState">RateLimitState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/#RateLimit">RateLimit</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>action=None<span class="p">, </span>bypass_url_patterns=None<span class="p">, </span>correlate=None<span class="p">, </span>description=None<span class="p">, </span>disabled=None<span class="p">, </span>match=None<span class="p">, </span>period=None<span class="p">, </span>threshold=None<span class="p">, </span>zone_id=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetRateLimit<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitState">RateLimitState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimit">RateLimit</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Cloudflare/Pulumi.Cloudflare.RateLimit.html">RateLimit</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Cloudflare/Pulumi.Cloudflare..RateLimitState.html">RateLimitState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Rate<wbr>Limit<wbr>Action<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bypass<wbr>Url<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Rate<wbr>Limit<wbr>Correlate<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Rate<wbr>Limit<wbr>Match<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Period</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Zone<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Rate<wbr>Limit<wbr>Action</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Bypass<wbr>Url<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Rate<wbr>Limit<wbr>Correlate</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Rate<wbr>Limit<wbr>Match</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Period</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Zone<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Rate<wbr>Limit<wbr>Action</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bypass<wbr>Url<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Rate<wbr>Limit<wbr>Correlate</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Rate<wbr>Limit<wbr>Match</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>period</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>zone<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>action</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitaction">Dict[Rate<wbr>Limit<wbr>Action]</a></span>
    </dt>
    <dd>{{% md %}}The action to be performed when the threshold of matched traffic within the period defined is exceeded.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>bypass_<wbr>url_<wbr>patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}URLs matching the patterns specified here will be excluded from rate limiting.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>correlate</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitcorrelate">Dict[Rate<wbr>Limit<wbr>Correlate]</a></span>
    </dt>
    <dd>{{% md %}}Determines how rate limiting is applied. By default if not specified, rate limiting applies to the clients IP address.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A note that you can use to describe the reason for a rate limit. This value is sanitized and all tags are removed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>disabled</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether this ratelimit is currently disabled. Default: `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>match</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatch">Dict[Rate<wbr>Limit<wbr>Match]</a></span>
    </dt>
    <dd>{{% md %}}Determines which traffic the rate limit counts towards the threshold. By default matches all traffic in the zone. See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>period</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The time in seconds to count matching traffic. If the count exceeds threshold within this period the action will be performed (min: 1, max: 86,400).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The threshold that triggers the rate limit mitigations, combine with period. i.e. threshold per period (min: 2, max: 1,000,000).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>zone_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The DNS zone ID to apply rate limiting to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Rate<wbr>Limit<wbr>Action</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/input/#RateLimitAction">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/output/#RateLimitAction">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitActionArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitActionOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of action to perform. Allowable values are 'simulate', 'ban', 'challenge' and 'js_challenge'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitactionresponse">Rate<wbr>Limit<wbr>Action<wbr>Response<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time in seconds as an integer to perform the mitigation action. This field is required if the `mode` is either `simulate` or `ban`. Must be the same or greater than the period (min: 1, max: 86400).
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of action to perform. Allowable values are 'simulate', 'ban', 'challenge' and 'js_challenge'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitactionresponse">Rate<wbr>Limit<wbr>Action<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The time in seconds as an integer to perform the mitigation action. This field is required if the `mode` is either `simulate` or `ban`. Must be the same or greater than the period (min: 1, max: 86400).
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of action to perform. Allowable values are 'simulate', 'ban', 'challenge' and 'js_challenge'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitactionresponse">Rate<wbr>Limit<wbr>Action<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The time in seconds as an integer to perform the mitigation action. This field is required if the `mode` is either `simulate` or `ban`. Must be the same or greater than the period (min: 1, max: 86400).
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of action to perform. Allowable values are 'simulate', 'ban', 'challenge' and 'js_challenge'.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitactionresponse">Dict[Rate<wbr>Limit<wbr>Action<wbr>Response]</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>timeout</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The time in seconds as an integer to perform the mitigation action. This field is required if the `mode` is either `simulate` or `ban`. Must be the same or greater than the period (min: 1, max: 86400).
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rate<wbr>Limit<wbr>Action<wbr>Response</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/input/#RateLimitActionResponse">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/output/#RateLimitActionResponse">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitActionResponseArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitActionResponseOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Body</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The body to return, the content here should conform to the content_type.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Content<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The content-type of the body, must be one of: 'text/plain', 'text/xml', 'application/json'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Body</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The body to return, the content here should conform to the content_type.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Content<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The content-type of the body, must be one of: 'text/plain', 'text/xml', 'application/json'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>body</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The body to return, the content here should conform to the content_type.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>content<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The content-type of the body, must be one of: 'text/plain', 'text/xml', 'application/json'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>body</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The body to return, the content here should conform to the content_type.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>content<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The content-type of the body, must be one of: 'text/plain', 'text/xml', 'application/json'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rate<wbr>Limit<wbr>Correlate</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/input/#RateLimitCorrelate">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/output/#RateLimitCorrelate">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitCorrelateArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitCorrelateOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If set to 'nat', NAT support will be enabled for rate limiting.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If set to 'nat', NAT support will be enabled for rate limiting.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>by</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If set to 'nat', NAT support will be enabled for rate limiting.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>by</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}If set to 'nat', NAT support will be enabled for rate limiting.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rate<wbr>Limit<wbr>Match</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/input/#RateLimitMatch">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/output/#RateLimitMatch">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitMatchArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitMatchOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Request</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchrequest">Rate<wbr>Limit<wbr>Match<wbr>Request<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Matches HTTP requests (from the client to Cloudflare). See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchresponse">Rate<wbr>Limit<wbr>Match<wbr>Response<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Request</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchrequest">Rate<wbr>Limit<wbr>Match<wbr>Request</a></span>
    </dt>
    <dd>{{% md %}}Matches HTTP requests (from the client to Cloudflare). See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchresponse">Rate<wbr>Limit<wbr>Match<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>request</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchrequest">Rate<wbr>Limit<wbr>Match<wbr>Request</a></span>
    </dt>
    <dd>{{% md %}}Matches HTTP requests (from the client to Cloudflare). See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchresponse">Rate<wbr>Limit<wbr>Match<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>request</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchrequest">Dict[Rate<wbr>Limit<wbr>Match<wbr>Request]</a></span>
    </dt>
    <dd>{{% md %}}Matches HTTP requests (from the client to Cloudflare). See definition below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>response</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ratelimitmatchresponse">Dict[Rate<wbr>Limit<wbr>Match<wbr>Response]</a></span>
    </dt>
    <dd>{{% md %}}Custom content-type and body to return, this overrides the custom error for the zone. This field is not required. Omission will result in default HTML error page. Definition below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rate<wbr>Limit<wbr>Match<wbr>Request</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/input/#RateLimitMatchRequest">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/output/#RateLimitMatchRequest">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitMatchRequestArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitMatchRequestOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Methods</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}HTTP Methods, can be a subset ['POST','PUT'] or all ['\_ALL\_']. Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Schemes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}HTTP Schemes, can be one ['HTTPS'], both ['HTTP','HTTPS'] or all ['\_ALL\_'].  Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url<wbr>Pattern</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URL pattern to match comprised of the host and path, i.e. example.org/path. Wildcard are expanded to match applicable traffic, query strings are not matched. Use * for all traffic to your zone. Default: '*'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Methods</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}HTTP Methods, can be a subset ['POST','PUT'] or all ['\_ALL\_']. Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Schemes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}HTTP Schemes, can be one ['HTTPS'], both ['HTTP','HTTPS'] or all ['\_ALL\_'].  Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url<wbr>Pattern</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URL pattern to match comprised of the host and path, i.e. example.org/path. Wildcard are expanded to match applicable traffic, query strings are not matched. Use * for all traffic to your zone. Default: '*'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>methods</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}HTTP Methods, can be a subset ['POST','PUT'] or all ['\_ALL\_']. Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>schemes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}HTTP Schemes, can be one ['HTTPS'], both ['HTTP','HTTPS'] or all ['\_ALL\_'].  Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url<wbr>Pattern</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The URL pattern to match comprised of the host and path, i.e. example.org/path. Wildcard are expanded to match applicable traffic, query strings are not matched. Use * for all traffic to your zone. Default: '*'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>methods</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}HTTP Methods, can be a subset ['POST','PUT'] or all ['\_ALL\_']. Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>schemes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}HTTP Schemes, can be one ['HTTPS'], both ['HTTP','HTTPS'] or all ['\_ALL\_'].  Default: ['\_ALL\_'].
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url<wbr>Pattern</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The URL pattern to match comprised of the host and path, i.e. example.org/path. Wildcard are expanded to match applicable traffic, query strings are not matched. Use * for all traffic to your zone. Default: '*'.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rate<wbr>Limit<wbr>Match<wbr>Response</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/input/#RateLimitMatchResponse">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/cloudflare/types/output/#RateLimitMatchResponse">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitMatchResponseArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-cloudflare/sdk/go/cloudflare/?tab=doc#RateLimitMatchResponseOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Origin<wbr>Traffic</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Only count traffic that has come from your origin servers. If true, cached items that Cloudflare serve will not count towards rate limiting. Default: `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Statuses</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;int&gt;</span>
    </dt>
    <dd>{{% md %}}HTTP Status codes, can be one [403], many [401,403] or indicate all by not providing this value.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Origin<wbr>Traffic</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Only count traffic that has come from your origin servers. If true, cached items that Cloudflare serve will not count towards rate limiting. Default: `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Statuses</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]int</span>
    </dt>
    <dd>{{% md %}}HTTP Status codes, can be one [403], many [401,403] or indicate all by not providing this value.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>origin<wbr>Traffic</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Only count traffic that has come from your origin servers. If true, cached items that Cloudflare serve will not count towards rate limiting. Default: `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>statuses</span>
        <span class="property-indicator"></span>
        <span class="property-type">number[]</span>
    </dt>
    <dd>{{% md %}}HTTP Status codes, can be one [403], many [401,403] or indicate all by not providing this value.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>origin<wbr>Traffic</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Only count traffic that has come from your origin servers. If true, cached items that Cloudflare serve will not count towards rate limiting. Default: `true`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>statuses</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[Integer]</span>
    </dt>
    <dd>{{% md %}}HTTP Status codes, can be one [403], many [401,403] or indicate all by not providing this value.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-cloudflare">https://github.com/pulumi/pulumi-cloudflare</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
