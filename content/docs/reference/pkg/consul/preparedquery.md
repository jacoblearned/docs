
---
title: "PreparedQuery"
block_external_search_index: true
---






## Create a PreparedQuery Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/consul/#PreparedQuery">PreparedQuery</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/consul/#PreparedQueryArgs">PreparedQueryArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">PreparedQuery</span><span class="p">(resource_name, opts=None, </span>connect=None<span class="p">, </span>datacenter=None<span class="p">, </span>dns=None<span class="p">, </span>failover=None<span class="p">, </span>name=None<span class="p">, </span>near=None<span class="p">, </span>only_passing=None<span class="p">, </span>service=None<span class="p">, </span>session=None<span class="p">, </span>stored_token=None<span class="p">, </span>tags=None<span class="p">, </span>template=None<span class="p">, </span>token=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewPreparedQuery<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryArgs">PreparedQueryArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQuery">PreparedQuery</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Consul/Pulumi.Consul.PreparedQuery.html">PreparedQuery</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Consul/Pulumi.Consul.PreparedQueryArgs.html">PreparedQueryArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Service</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Prepared<wbr>Query<wbr>Dns<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Prepared<wbr>Query<wbr>Failover<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Near</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Only<wbr>Passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Session</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Stored<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Prepared<wbr>Query<wbr>Template<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Service</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Prepared<wbr>Query<wbr>Dns</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Prepared<wbr>Query<wbr>Failover</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Near</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Only<wbr>Passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Session</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Stored<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Prepared<wbr>Query<wbr>Template</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>service</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Prepared<wbr>Query<wbr>Dns</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Prepared<wbr>Query<wbr>Failover</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>near</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>only<wbr>Passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>session</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>stored<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Prepared<wbr>Query<wbr>Template</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>service</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Dict[Prepared<wbr>Query<wbr>Dns]</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Dict[Prepared<wbr>Query<wbr>Failover]</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>near</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>only_<wbr>passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>session</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>stored_<wbr>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Dict[Prepared<wbr>Query<wbr>Template]</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Look up an Existing PreparedQuery Resource

Get an existing PreparedQuery resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/consul/#PreparedQueryState">PreparedQueryState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/consul/#PreparedQuery">PreparedQuery</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>connect=None<span class="p">, </span>datacenter=None<span class="p">, </span>dns=None<span class="p">, </span>failover=None<span class="p">, </span>name=None<span class="p">, </span>near=None<span class="p">, </span>only_passing=None<span class="p">, </span>service=None<span class="p">, </span>session=None<span class="p">, </span>stored_token=None<span class="p">, </span>tags=None<span class="p">, </span>template=None<span class="p">, </span>token=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetPreparedQuery<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryState">PreparedQueryState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQuery">PreparedQuery</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Consul/Pulumi.Consul.PreparedQuery.html">PreparedQuery</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Consul/Pulumi.Consul..PreparedQueryState.html">PreparedQueryState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Prepared<wbr>Query<wbr>Dns<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Prepared<wbr>Query<wbr>Failover<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Near</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Only<wbr>Passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Service</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Session</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Stored<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Prepared<wbr>Query<wbr>Template<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Prepared<wbr>Query<wbr>Dns</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Prepared<wbr>Query<wbr>Failover</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Near</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Only<wbr>Passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Service</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Session</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Stored<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Prepared<wbr>Query<wbr>Template</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Prepared<wbr>Query<wbr>Dns</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Prepared<wbr>Query<wbr>Failover</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>near</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>only<wbr>Passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>service</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>session</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>stored<wbr>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Prepared<wbr>Query<wbr>Template</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>connect</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true` the prepared query will return connect
proxy services for a queried service.  Conditions such as `tags` in the
prepared query will be matched against the proxy service. Defaults to false.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>datacenter</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The datacenter to use. This overrides the
agent's default datacenter and the datacenter in the provider setup.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>dns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerydns">Dict[Prepared<wbr>Query<wbr>Dns]</a></span>
    </dt>
    <dd>{{% md %}}Settings for controlling the DNS response details.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>failover</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedqueryfailover">Dict[Prepared<wbr>Query<wbr>Failover]</a></span>
    </dt>
    <dd>{{% md %}}Options for controlling behavior when no healthy
nodes are available in the local DC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the prepared query. Used to identify
the prepared query during requests. Can be specified as an empty string
to configure the query as a catch-all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>near</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Allows specifying the name of a node to sort results
near using Consul's distance sorting and network coordinates. The magic
`_agent` value can be used to always sort nearest the node servicing the
request.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>only_<wbr>passing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}When `true`, the prepared query will only
return nodes with passing health checks in the result.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>service</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the service to query.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>session</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the Consul session to tie this query's
lifetime to.  This is an advanced parameter that should not be used without a
complete understanding of Consul sessions and the implications of their use
(it is recommended to leave this blank in nearly all cases).  If this
parameter is omitted the query will not expire.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>stored_<wbr>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ACL token to store with the prepared
query. This token will be used by default whenever the query is executed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The list of required and/or disallowed tags.  If a tag is
in this list it must be present.  If the tag is preceded with a "!" then it is
disallowed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>template</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#preparedquerytemplate">Dict[Prepared<wbr>Query<wbr>Template]</a></span>
    </dt>
    <dd>{{% md %}}Query templating options. This is used to make a
single prepared query respond to many different requests.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ACL token to use when saving the prepared query.
This overrides the token that the agent provides by default.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Prepared<wbr>Query<wbr>Dns</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/consul/types/input/#PreparedQueryDns">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/consul/types/output/#PreparedQueryDns">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryDnsArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryDnsOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Ttl</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The TTL to send when returning DNS results.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Ttl</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The TTL to send when returning DNS results.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>ttl</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The TTL to send when returning DNS results.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>ttl</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The TTL to send when returning DNS results.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Prepared<wbr>Query<wbr>Failover</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/consul/types/input/#PreparedQueryFailover">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/consul/types/output/#PreparedQueryFailover">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryFailoverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryFailoverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Datacenters</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}Remote datacenters to return results from.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Nearest<wbr>N</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Return results from this many datacenters,
sorted in ascending order of estimated RTT.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Datacenters</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}Remote datacenters to return results from.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Nearest<wbr>N</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Return results from this many datacenters,
sorted in ascending order of estimated RTT.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>datacenters</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}Remote datacenters to return results from.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>nearest<wbr>N</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Return results from this many datacenters,
sorted in ascending order of estimated RTT.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>datacenters</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}Remote datacenters to return results from.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>nearest<wbr>N</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Return results from this many datacenters,
sorted in ascending order of estimated RTT.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Prepared<wbr>Query<wbr>Template</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/consul/types/input/#PreparedQueryTemplate">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/consul/types/output/#PreparedQueryTemplate">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryTemplateArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-consul/sdk/go/consul/?tab=doc#PreparedQueryTemplateOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Regexp</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The regular expression to match with. When using
`name_prefix_match`, this regex is applied against the query name.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of template matching to perform. Currently
only `name_prefix_match` is supported.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Regexp</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The regular expression to match with. When using
`name_prefix_match`, this regex is applied against the query name.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of template matching to perform. Currently
only `name_prefix_match` is supported.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>regexp</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The regular expression to match with. When using
`name_prefix_match`, this regex is applied against the query name.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of template matching to perform. Currently
only `name_prefix_match` is supported.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>regexp</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The regular expression to match with. When using
`name_prefix_match`, this regex is applied against the query name.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of template matching to perform. Currently
only `name_prefix_match` is supported.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-consul">https://github.com/pulumi/pulumi-consul</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
