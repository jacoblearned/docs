
---
title: "getNamespaceAuthorizationRule"
title_tag: "azure-native.notificationhubs.getNamespaceAuthorizationRule"
meta_desc: "Documentation for the azure-native.notificationhubs.getNamespaceAuthorizationRule function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Description of a Namespace AuthorizationRules.
API Version: 2017-04-01.




## Using getNamespaceAuthorizationRule {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getNamespaceAuthorizationRule<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetNamespaceAuthorizationRuleArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetNamespaceAuthorizationRuleResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_namespace_authorization_rule(</span><span class="nx">authorization_rule_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">namespace_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetNamespaceAuthorizationRuleResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupNamespaceAuthorizationRule<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupNamespaceAuthorizationRuleArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupNamespaceAuthorizationRuleResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupNamespaceAuthorizationRule` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetNamespaceAuthorizationRule </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetNamespaceAuthorizationRuleResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetNamespaceAuthorizationRuleArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="authorizationrulename_csharp">
<a href="#authorizationrulename_csharp" style="color: inherit; text-decoration: inherit;">Authorization<wbr>Rule<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Authorization rule name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="namespacename_csharp">
<a href="#namespacename_csharp" style="color: inherit; text-decoration: inherit;">Namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The namespace name{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="authorizationrulename_go">
<a href="#authorizationrulename_go" style="color: inherit; text-decoration: inherit;">Authorization<wbr>Rule<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Authorization rule name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="namespacename_go">
<a href="#namespacename_go" style="color: inherit; text-decoration: inherit;">Namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The namespace name{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="authorizationrulename_nodejs">
<a href="#authorizationrulename_nodejs" style="color: inherit; text-decoration: inherit;">authorization<wbr>Rule<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Authorization rule name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="namespacename_nodejs">
<a href="#namespacename_nodejs" style="color: inherit; text-decoration: inherit;">namespace<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The namespace name{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="authorization_rule_name_python">
<a href="#authorization_rule_name_python" style="color: inherit; text-decoration: inherit;">authorization_<wbr>rule_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Authorization rule name.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="namespace_name_python">
<a href="#namespace_name_python" style="color: inherit; text-decoration: inherit;">namespace_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The namespace name{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
</dl>
{{% /choosable %}}




## getNamespaceAuthorizationRule Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="claimtype_csharp">
<a href="#claimtype_csharp" style="color: inherit; text-decoration: inherit;">Claim<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="claimvalue_csharp">
<a href="#claimvalue_csharp" style="color: inherit; text-decoration: inherit;">Claim<wbr>Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim value{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="createdtime_csharp">
<a href="#createdtime_csharp" style="color: inherit; text-decoration: inherit;">Created<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The created time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="keyname_csharp">
<a href="#keyname_csharp" style="color: inherit; text-decoration: inherit;">Key<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the authorization rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="modifiedtime_csharp">
<a href="#modifiedtime_csharp" style="color: inherit; text-decoration: inherit;">Modified<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The last modified time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="primarykey_csharp">
<a href="#primarykey_csharp" style="color: inherit; text-decoration: inherit;">Primary<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="revision_csharp">
<a href="#revision_csharp" style="color: inherit; text-decoration: inherit;">Revision</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The revision number for the rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="secondarykey_csharp">
<a href="#secondarykey_csharp" style="color: inherit; text-decoration: inherit;">Secondary<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="location_csharp">
<a href="#location_csharp" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="rights_csharp">
<a href="#rights_csharp" style="color: inherit; text-decoration: inherit;">Rights</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}The rights associated with the rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="sku_csharp">
<a href="#sku_csharp" style="color: inherit; text-decoration: inherit;">Sku</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#skuresponse">Pulumi.<wbr>Azure<wbr>Native.<wbr>Notification<wbr>Hubs.<wbr>Outputs.<wbr>Sku<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}The sku of the created namespace{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="tags_csharp">
<a href="#tags_csharp" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, string&gt;</span>
    </dt>
    <dd>{{% md %}}Resource tags{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="claimtype_go">
<a href="#claimtype_go" style="color: inherit; text-decoration: inherit;">Claim<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="claimvalue_go">
<a href="#claimvalue_go" style="color: inherit; text-decoration: inherit;">Claim<wbr>Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim value{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="createdtime_go">
<a href="#createdtime_go" style="color: inherit; text-decoration: inherit;">Created<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The created time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="keyname_go">
<a href="#keyname_go" style="color: inherit; text-decoration: inherit;">Key<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the authorization rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="modifiedtime_go">
<a href="#modifiedtime_go" style="color: inherit; text-decoration: inherit;">Modified<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The last modified time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="primarykey_go">
<a href="#primarykey_go" style="color: inherit; text-decoration: inherit;">Primary<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="revision_go">
<a href="#revision_go" style="color: inherit; text-decoration: inherit;">Revision</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The revision number for the rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="secondarykey_go">
<a href="#secondarykey_go" style="color: inherit; text-decoration: inherit;">Secondary<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="location_go">
<a href="#location_go" style="color: inherit; text-decoration: inherit;">Location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="rights_go">
<a href="#rights_go" style="color: inherit; text-decoration: inherit;">Rights</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The rights associated with the rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="sku_go">
<a href="#sku_go" style="color: inherit; text-decoration: inherit;">Sku</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#skuresponse">Sku<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}The sku of the created namespace{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="tags_go">
<a href="#tags_go" style="color: inherit; text-decoration: inherit;">Tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]string</span>
    </dt>
    <dd>{{% md %}}Resource tags{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="claimtype_nodejs">
<a href="#claimtype_nodejs" style="color: inherit; text-decoration: inherit;">claim<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="claimvalue_nodejs">
<a href="#claimvalue_nodejs" style="color: inherit; text-decoration: inherit;">claim<wbr>Value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim value{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="createdtime_nodejs">
<a href="#createdtime_nodejs" style="color: inherit; text-decoration: inherit;">created<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The created time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="keyname_nodejs">
<a href="#keyname_nodejs" style="color: inherit; text-decoration: inherit;">key<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A string that describes the authorization rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="modifiedtime_nodejs">
<a href="#modifiedtime_nodejs" style="color: inherit; text-decoration: inherit;">modified<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The last modified time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="primarykey_nodejs">
<a href="#primarykey_nodejs" style="color: inherit; text-decoration: inherit;">primary<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="revision_nodejs">
<a href="#revision_nodejs" style="color: inherit; text-decoration: inherit;">revision</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The revision number for the rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="secondarykey_nodejs">
<a href="#secondarykey_nodejs" style="color: inherit; text-decoration: inherit;">secondary<wbr>Key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="location_nodejs">
<a href="#location_nodejs" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="rights_nodejs">
<a href="#rights_nodejs" style="color: inherit; text-decoration: inherit;">rights</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}The rights associated with the rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="sku_nodejs">
<a href="#sku_nodejs" style="color: inherit; text-decoration: inherit;">sku</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#skuresponse">Sku<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}The sku of the created namespace{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="tags_nodejs">
<a href="#tags_nodejs" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: string}</span>
    </dt>
    <dd>{{% md %}}Resource tags{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="claim_type_python">
<a href="#claim_type_python" style="color: inherit; text-decoration: inherit;">claim_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="claim_value_python">
<a href="#claim_value_python" style="color: inherit; text-decoration: inherit;">claim_<wbr>value</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A string that describes the claim value{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="created_time_python">
<a href="#created_time_python" style="color: inherit; text-decoration: inherit;">created_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The created time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="key_name_python">
<a href="#key_name_python" style="color: inherit; text-decoration: inherit;">key_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A string that describes the authorization rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="modified_time_python">
<a href="#modified_time_python" style="color: inherit; text-decoration: inherit;">modified_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The last modified time for this rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="primary_key_python">
<a href="#primary_key_python" style="color: inherit; text-decoration: inherit;">primary_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="revision_python">
<a href="#revision_python" style="color: inherit; text-decoration: inherit;">revision</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The revision number for the rule{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="secondary_key_python">
<a href="#secondary_key_python" style="color: inherit; text-decoration: inherit;">secondary_<wbr>key</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A base64-encoded 256-bit primary key for signing and validating the SAS token.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="location_python">
<a href="#location_python" style="color: inherit; text-decoration: inherit;">location</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource location{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="rights_python">
<a href="#rights_python" style="color: inherit; text-decoration: inherit;">rights</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Sequence[str]</span>
    </dt>
    <dd>{{% md %}}The rights associated with the rule.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="sku_python">
<a href="#sku_python" style="color: inherit; text-decoration: inherit;">sku</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#skuresponse">Sku<wbr>Response</a></span>
    </dt>
    <dd>{{% md %}}The sku of the created namespace{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="tags_python">
<a href="#tags_python" style="color: inherit; text-decoration: inherit;">tags</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">Mapping[str, str]</span>
    </dt>
    <dd>{{% md %}}Resource tags{{% /md %}}</dd>
</dl>
{{% /choosable %}}




## Supporting Types


<h4 id="skuresponse">Sku<wbr>Response</h4>



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the notification hub sku{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="capacity_csharp">
<a href="#capacity_csharp" style="color: inherit; text-decoration: inherit;">Capacity</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The capacity of the resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="family_csharp">
<a href="#family_csharp" style="color: inherit; text-decoration: inherit;">Family</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Sku Family{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="size_csharp">
<a href="#size_csharp" style="color: inherit; text-decoration: inherit;">Size</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Sku size{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="tier_csharp">
<a href="#tier_csharp" style="color: inherit; text-decoration: inherit;">Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The tier of particular sku{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the notification hub sku{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="capacity_go">
<a href="#capacity_go" style="color: inherit; text-decoration: inherit;">Capacity</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The capacity of the resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="family_go">
<a href="#family_go" style="color: inherit; text-decoration: inherit;">Family</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Sku Family{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="size_go">
<a href="#size_go" style="color: inherit; text-decoration: inherit;">Size</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Sku size{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="tier_go">
<a href="#tier_go" style="color: inherit; text-decoration: inherit;">Tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The tier of particular sku{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the notification hub sku{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="capacity_nodejs">
<a href="#capacity_nodejs" style="color: inherit; text-decoration: inherit;">capacity</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The capacity of the resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="family_nodejs">
<a href="#family_nodejs" style="color: inherit; text-decoration: inherit;">family</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Sku Family{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="size_nodejs">
<a href="#size_nodejs" style="color: inherit; text-decoration: inherit;">size</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The Sku size{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="tier_nodejs">
<a href="#tier_nodejs" style="color: inherit; text-decoration: inherit;">tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The tier of particular sku{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the notification hub sku{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="capacity_python">
<a href="#capacity_python" style="color: inherit; text-decoration: inherit;">capacity</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The capacity of the resource{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="family_python">
<a href="#family_python" style="color: inherit; text-decoration: inherit;">family</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Sku Family{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="size_python">
<a href="#size_python" style="color: inherit; text-decoration: inherit;">size</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The Sku size{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="tier_python">
<a href="#tier_python" style="color: inherit; text-decoration: inherit;">tier</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The tier of particular sku{{% /md %}}</dd>
</dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>
