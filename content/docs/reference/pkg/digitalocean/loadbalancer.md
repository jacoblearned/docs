
---
title: "LoadBalancer"
block_external_search_index: true
---



Provides a DigitalOcean Load Balancer resource. This can be used to create,
modify, and delete Load Balancers.

> This content is derived from https://github.com/terraform-providers/terraform-provider-digitalocean/blob/master/website/docs/r/loadbalancer.html.markdown.



## Create a LoadBalancer Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#LoadBalancer">LoadBalancer</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#LoadBalancerArgs">LoadBalancerArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">LoadBalancer</span><span class="p">(resource_name, opts=None, </span>algorithm=None<span class="p">, </span>droplet_ids=None<span class="p">, </span>droplet_tag=None<span class="p">, </span>enable_proxy_protocol=None<span class="p">, </span>forwarding_rules=None<span class="p">, </span>healthcheck=None<span class="p">, </span>name=None<span class="p">, </span>redirect_http_to_https=None<span class="p">, </span>region=None<span class="p">, </span>sticky_sessions=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewLoadBalancer<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerArgs">LoadBalancerArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancer">LoadBalancer</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.Digitalocean.LoadBalancer.html">LoadBalancer</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.DigitalOcean.LoadBalancerArgs.html">LoadBalancerArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Forwarding<wbr>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">List&lt;Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Load<wbr>Balancer<wbr>Forwarding<wbr>Rule<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;int&gt;</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Proxy<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Load<wbr>Balancer<wbr>Healthcheck<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Redirect<wbr>Http<wbr>To<wbr>Https</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sticky<wbr>Sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Load<wbr>Balancer<wbr>Sticky<wbr>Sessions<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Forwarding<wbr>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">[]Load<wbr>Balancer<wbr>Forwarding<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]int</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Proxy<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Load<wbr>Balancer<wbr>Healthcheck</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Redirect<wbr>Http<wbr>To<wbr>Https</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sticky<wbr>Sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Load<wbr>Balancer<wbr>Sticky<wbr>Sessions</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>forwarding<wbr>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">Load<wbr>Balancer<wbr>Forwarding<wbr>Rule[]</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">Region</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">Algorithm</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">number[]</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet<wbr>Tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable<wbr>Proxy<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Load<wbr>Balancer<wbr>Healthcheck</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>redirect<wbr>Http<wbr>To<wbr>Https</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sticky<wbr>Sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Load<wbr>Balancer<wbr>Sticky<wbr>Sessions</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>forwarding_<wbr>rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">List[Load<wbr>Balancer<wbr>Forwarding<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet_<wbr>ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[Integer]</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet_<wbr>tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable_<wbr>proxy_<wbr>protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Dict[Load<wbr>Balancer<wbr>Healthcheck]</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>redirect_<wbr>http_<wbr>to_<wbr>https</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sticky_<wbr>sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Dict[Load<wbr>Balancer<wbr>Sticky<wbr>Sessions]</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## LoadBalancer Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing LoadBalancer Resource

Get an existing LoadBalancer resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#LoadBalancerState">LoadBalancerState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/#LoadBalancer">LoadBalancer</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>algorithm=None<span class="p">, </span>droplet_ids=None<span class="p">, </span>droplet_tag=None<span class="p">, </span>enable_proxy_protocol=None<span class="p">, </span>forwarding_rules=None<span class="p">, </span>healthcheck=None<span class="p">, </span>ip=None<span class="p">, </span>name=None<span class="p">, </span>redirect_http_to_https=None<span class="p">, </span>region=None<span class="p">, </span>status=None<span class="p">, </span>sticky_sessions=None<span class="p">, </span>urn=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetLoadBalancer<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerState">LoadBalancerState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancer">LoadBalancer</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.Digitalocean.LoadBalancer.html">LoadBalancer</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Digitalocean/Pulumi.Digitalocean..LoadBalancerState.html">LoadBalancerState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;int&gt;</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Proxy<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Forwarding<wbr>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">List&lt;Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Load<wbr>Balancer<wbr>Forwarding<wbr>Rule<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Load<wbr>Balancer<wbr>Healthcheck<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Redirect<wbr>Http<wbr>To<wbr>Https</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sticky<wbr>Sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Pulumi.<wbr>Digital<wbr>Ocean.<wbr>Inputs.<wbr>Load<wbr>Balancer<wbr>Sticky<wbr>Sessions<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]int</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Droplet<wbr>Tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Proxy<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Forwarding<wbr>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">[]Load<wbr>Balancer<wbr>Forwarding<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Load<wbr>Balancer<wbr>Healthcheck</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Redirect<wbr>Http<wbr>To<wbr>Https</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Sticky<wbr>Sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Load<wbr>Balancer<wbr>Sticky<wbr>Sessions</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">Algorithm</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">number[]</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet<wbr>Tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable<wbr>Proxy<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>forwarding<wbr>Rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">Load<wbr>Balancer<wbr>Forwarding<wbr>Rule[]</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Load<wbr>Balancer<wbr>Healthcheck</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>redirect<wbr>Http<wbr>To<wbr>Https</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">Region</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sticky<wbr>Sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Load<wbr>Balancer<wbr>Sticky<wbr>Sessions</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The load balancing algorithm used to determine
which backend Droplet will be selected by a client. It must be either `round_robin`
or `least_connections`. The default value is `round_robin`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet_<wbr>ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[Integer]</span>
    </dt>
    <dd>{{% md %}}A list of the IDs of each droplet to be attached to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>droplet_<wbr>tag</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of a Droplet tag corresponding to Droplets to be assigned to the Load Balancer.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable_<wbr>proxy_<wbr>protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether PROXY
Protocol should be used to pass information from connecting client requests to
the backend service. Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>forwarding_<wbr>rules</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerforwardingrule">List[Load<wbr>Balancer<wbr>Forwarding<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}A list of `forwarding_rule` to be assigned to the
Load Balancer. The `forwarding_rule` block is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>healthcheck</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerhealthcheck">Dict[Load<wbr>Balancer<wbr>Healthcheck]</a></span>
    </dt>
    <dd>{{% md %}}A `healthcheck` block to be assigned to the
Load Balancer. The `healthcheck` block is documented below. Only 1 healthcheck is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ip</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Load Balancer name
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>redirect_<wbr>http_<wbr>to_<wbr>https</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether
HTTP requests to the Load Balancer on port 80 will be redirected to HTTPS on port 443.
Default value is `false`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region to start in
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>sticky_<wbr>sessions</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#loadbalancerstickysessions">Dict[Load<wbr>Balancer<wbr>Sticky<wbr>Sessions]</a></span>
    </dt>
    <dd>{{% md %}}A `sticky_sessions` block to be assigned to the
Load Balancer. The `sticky_sessions` block is documented below. Only 1 sticky_sessions block is allowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>urn</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The uniform resource name for the Load Balancer
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Load<wbr>Balancer<wbr>Forwarding<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/input/#LoadBalancerForwardingRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/output/#LoadBalancerForwardingRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerForwardingRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerForwardingRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Entry<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on which the Load Balancer instance will listen.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Entry<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic to the Load Balancer. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Target<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets to which the Load Balancer will send traffic.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Target<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic from the Load Balancer to the backend Droplets. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Certificate<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the TLS certificate to be used for SSL termination.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tls<wbr>Passthrough</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether SSL encrypted traffic will be passed through to the backend Droplets. The default value is `false`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Entry<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on which the Load Balancer instance will listen.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Entry<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic to the Load Balancer. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Target<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets to which the Load Balancer will send traffic.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Target<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic from the Load Balancer to the backend Droplets. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Certificate<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the TLS certificate to be used for SSL termination.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tls<wbr>Passthrough</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether SSL encrypted traffic will be passed through to the backend Droplets. The default value is `false`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>entry<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on which the Load Balancer instance will listen.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>entry<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic to the Load Balancer. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>target<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets to which the Load Balancer will send traffic.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>target<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic from the Load Balancer to the backend Droplets. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>certificate<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the TLS certificate to be used for SSL termination.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tls<wbr>Passthrough</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether SSL encrypted traffic will be passed through to the backend Droplets. The default value is `false`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>entry<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on which the Load Balancer instance will listen.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>entry<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic to the Load Balancer. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>target<wbr>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets to which the Load Balancer will send traffic.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>target<wbr>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The protocol used for traffic from the Load Balancer to the backend Droplets. The possible values are: `http`, `https`, `http2` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>certificate_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the TLS certificate to be used for SSL termination.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tls<wbr>Passthrough</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}A boolean value indicating whether SSL encrypted traffic will be passed through to the backend Droplets. The default value is `false`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Load<wbr>Balancer<wbr>Healthcheck</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/input/#LoadBalancerHealthcheck">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/output/#LoadBalancerHealthcheck">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerHealthcheckArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerHealthcheckOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets on which the health check will attempt a connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for health checks sent to the backend Droplets. The possible values are `http` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Check<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of seconds between between two consecutive health checks. If not specified, the default value is `10`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Healthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must pass for a backend Droplet to be marked "healthy" and be re-added to the pool. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The path on the backend Droplets to which the Load Balancer instance will send a request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Response<wbr>Timeout<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of seconds the Load Balancer instance will wait for a response until marking a health check as failed. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Unhealthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must fail for a backend Droplet to be marked "unhealthy" and be removed from the pool. If not specified, the default value is `3`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets on which the health check will attempt a connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for health checks sent to the backend Droplets. The possible values are `http` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Check<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of seconds between between two consecutive health checks. If not specified, the default value is `10`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Healthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must pass for a backend Droplet to be marked "healthy" and be re-added to the pool. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The path on the backend Droplets to which the Load Balancer instance will send a request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Response<wbr>Timeout<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of seconds the Load Balancer instance will wait for a response until marking a health check as failed. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Unhealthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must fail for a backend Droplet to be marked "unhealthy" and be removed from the pool. If not specified, the default value is `3`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>port</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets on which the health check will attempt a connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The protocol used for health checks sent to the backend Droplets. The possible values are `http` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>check<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of seconds between between two consecutive health checks. If not specified, the default value is `10`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>healthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must pass for a backend Droplet to be marked "healthy" and be re-added to the pool. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>path</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The path on the backend Droplets to which the Load Balancer instance will send a request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>response<wbr>Timeout<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of seconds the Load Balancer instance will wait for a response until marking a health check as failed. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>unhealthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must fail for a backend Droplet to be marked "unhealthy" and be removed from the pool. If not specified, the default value is `3`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>port</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}An integer representing the port on the backend Droplets on which the health check will attempt a connection.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The protocol used for health checks sent to the backend Droplets. The possible values are `http` or `tcp`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>check<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of seconds between between two consecutive health checks. If not specified, the default value is `10`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>healthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must pass for a backend Droplet to be marked "healthy" and be re-added to the pool. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>path</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The path on the backend Droplets to which the Load Balancer instance will send a request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>response<wbr>Timeout<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of seconds the Load Balancer instance will wait for a response until marking a health check as failed. If not specified, the default value is `5`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>unhealthy<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of times a health check must fail for a backend Droplet to be marked "unhealthy" and be removed from the pool. If not specified, the default value is `3`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Load<wbr>Balancer<wbr>Sticky<wbr>Sessions</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/input/#LoadBalancerStickySessions">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/digitalocean/types/output/#LoadBalancerStickySessions">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerStickySessionsArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-digitalocean/sdk/go/digitalocean/?tab=doc#LoadBalancerStickySessionsOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Cookie<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name to be used for the cookie sent to the client. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cookie<wbr>Ttl<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of seconds until the cookie set by the Load Balancer expires. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}An attribute indicating how and if requests from a client will be persistently served by the same backend Droplet. The possible values are `cookies` or `none`. If not specified, the default value is `none`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Cookie<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name to be used for the cookie sent to the client. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cookie<wbr>Ttl<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of seconds until the cookie set by the Load Balancer expires. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}An attribute indicating how and if requests from a client will be persistently served by the same backend Droplet. The possible values are `cookies` or `none`. If not specified, the default value is `none`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>cookie<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name to be used for the cookie sent to the client. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cookie<wbr>Ttl<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of seconds until the cookie set by the Load Balancer expires. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}An attribute indicating how and if requests from a client will be persistently served by the same backend Droplet. The possible values are `cookies` or `none`. If not specified, the default value is `none`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>cookie<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name to be used for the cookie sent to the client. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cookie<wbr>Ttl<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of seconds until the cookie set by the Load Balancer expires. This attribute is required when using `cookies` for the sticky sessions type.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}An attribute indicating how and if requests from a client will be persistently served by the same backend Droplet. The possible values are `cookies` or `none`. If not specified, the default value is `none`.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-digitalocean">https://github.com/pulumi/pulumi-digitalocean</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
