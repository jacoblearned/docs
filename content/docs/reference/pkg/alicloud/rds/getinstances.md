
---
title: "GetInstances"
block_external_search_index: true
---



The `alicloud.rds.getInstances` data source provides a collection of RDS instances available in Alibaba Cloud account.
Filters support regular expression for the instance name, searches by tags, and other filters which are listed below.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as alicloud from "@pulumi/alicloud";

const dbInstancesDs = pulumi.output(alicloud.rds.getInstances({
    nameRegex: "data-\\d+",
    status: "Running",
    tags: {
        size: "tiny",
        type: "database",
    },
}, { async: true }));

export const firstDbInstanceId = dbInstancesDs.instances[0].id;
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-alicloud/blob/master/website/docs/d/db_instances.html.markdown.





## Using GetInstances

{{< chooser language "javascript,typescript,python,go,csharp" / >}}


{{% choosable language typescript %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getInstances<span class="p">(</span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/alicloud/rds/#GetInstancesArgs">GetInstancesArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/alicloud/rds/#GetInstancesResult">GetInstancesResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">function </span> get_instances(</span>connection_mode=None<span class="p">, </span>db_type=None<span class="p">, </span>engine=None<span class="p">, </span>ids=None<span class="p">, </span>name_regex=None<span class="p">, </span>output_file=None<span class="p">, </span>status=None<span class="p">, </span>tags=None<span class="p">, </span>vpc_id=None<span class="p">, </span>vswitch_id=None<span class="p">, </span>opts=None<span class="p">)</span></code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupInstances<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/go/alicloud/rds?tab=doc#LookupInstancesArgs">LookupInstancesArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">pulumi.InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/go/alicloud/rds?tab=doc#LookupInstancesResult">LookupInstancesResult</a></span>, error)</span></code></pre></div>
{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetInstances </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Alicloud/Pulumi.Alicloud.Rds.GetInstancesResult.html">GetInstancesResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Alicloud/Pulumi.AliCloud.Rds.GetInstancesArgs.html">GetInstancesArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span>? <span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name<wbr>Regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A regex string to filter results by instance name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>File</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}A map of tags assigned to the DB instances. 
Note: Before 1.60.0, the value's format is a `json` string which including `TagKey` and `TagValue`. `TagKey` cannot be null, and `TagValue` can be empty. Format example `"{\"key1\":\"value1\"}"`
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name<wbr>Regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A regex string to filter results by instance name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>File</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}A map of tags assigned to the DB instances. 
Note: Before 1.60.0, the value's format is a `json` string which including `TagKey` and `TagValue`. `TagKey` cannot be null, and `TagValue` can be empty. Format example `"{\"key1\":\"value1\"}"`
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name<wbr>Regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A regex string to filter results by instance name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output<wbr>File</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}A map of tags assigned to the DB instances. 
Note: Before 1.60.0, the value's format is a `json` string which including `TagKey` and `TagValue`. `TagKey` cannot be null, and `TagValue` can be empty. Format example `"{\"key1\":\"value1\"}"`
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>connection_<wbr>mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>db_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name_<wbr>regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A regex string to filter results by instance name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output_<wbr>file</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}A map of tags assigned to the DB instances. 
Note: Before 1.60.0, the value's format is a `json` string which including `TagKey` and `TagValue`. `TagKey` cannot be null, and `TagValue` can be empty. Format example `"{\"key1\":\"value1\"}"`
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>vpc_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>vswitch_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## GetInstances Result

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Instances</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getinstancesinstance">List&lt;Pulumi.<wbr>Ali<wbr>Cloud.<wbr>Rds.<wbr>Outputs.<wbr>Get<wbr>Instances<wbr>Instance&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of RDS instances. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Names</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance names. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name<wbr>Regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Output<wbr>File</span>
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
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the VPC the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the VSwitch the instance belongs to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Instances</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getinstancesinstance">[]Get<wbr>Instances<wbr>Instance</a></span>
    </dt>
    <dd>{{% md %}}A list of RDS instances. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Names</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance names. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name<wbr>Regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Output<wbr>File</span>
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
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the VPC the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the VSwitch the instance belongs to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>instances</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getinstancesinstance">Get<wbr>Instances<wbr>Instance[]</a></span>
    </dt>
    <dd>{{% md %}}A list of RDS instances. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>names</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance names. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name<wbr>Regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>output<wbr>File</span>
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
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the VPC the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the VSwitch the instance belongs to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}id is the provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance IDs. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>instances</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getinstancesinstance">List[Get<wbr>Instances<wbr>Instance]</a></span>
    </dt>
    <dd>{{% md %}}A list of RDS instances. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>names</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}A list of RDS instance names. 
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>connection_<wbr>mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>db_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name_<wbr>regex</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>output_<wbr>file</span>
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
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>vpc_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the VPC the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>vswitch_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the VSwitch the instance belongs to.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Supporting Types

<h4>Get<wbr>Instances<wbr>Instance</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/alicloud/types/output/#GetInstancesInstance">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/go/alicloud/rds?tab=doc#GetInstancesInstance">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Availability<wbr>Zone</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Availability zone.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Charge<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Billing method. Value options: `Postpaid` for Pay-As-You-Go and `Prepaid` for subscription.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Connection<wbr>String</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection string.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Create<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Creation time of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Db<wbr>Instance<wbr>Storage<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) The storage type of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Engine<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Expire<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Expiration time. Pay-As-You-Go instances never expire.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Guard<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If a disaster recovery instance is attached to the current instance, the ID of the disaster recovery instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Instance<wbr>Storage</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) User-defined DB instance storage space.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Sizing of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Master<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the primary instance. If this parameter is not returned, the current instance is a primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Net<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Internet` for public network or `Intranet` for private network.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection port.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Readonly<wbr>Instance<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}A list of IDs of read-only instances attached to the primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Region<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Region ID the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Temp<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If a temporary instance is attached to the current instance, the ID of the temporary instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Availability<wbr>Zone</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Availability zone.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Charge<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Billing method. Value options: `Postpaid` for Pay-As-You-Go and `Prepaid` for subscription.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Connection<wbr>String</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection string.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Create<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Creation time of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Db<wbr>Instance<wbr>Storage<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) The storage type of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Engine<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Expire<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Expiration time. Pay-As-You-Go instances never expire.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Guard<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If a disaster recovery instance is attached to the current instance, the ID of the disaster recovery instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Instance<wbr>Storage</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) User-defined DB instance storage space.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Sizing of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Master<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the primary instance. If this parameter is not returned, the current instance is a primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Net<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Internet` for public network or `Intranet` for private network.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection port.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Readonly<wbr>Instance<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}A list of IDs of read-only instances attached to the primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Region<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Region ID the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Temp<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If a temporary instance is attached to the current instance, the ID of the temporary instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>availability<wbr>Zone</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Availability zone.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>charge<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Billing method. Value options: `Postpaid` for Pay-As-You-Go and `Prepaid` for subscription.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>connection<wbr>String</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection string.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>create<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Creation time of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>db<wbr>Instance<wbr>Storage<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) The storage type of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>db<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>engine<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>expire<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Expiration time. Pay-As-You-Go instances never expire.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>guard<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If a disaster recovery instance is attached to the current instance, the ID of the disaster recovery instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>instance<wbr>Storage</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) User-defined DB instance storage space.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>instance<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Sizing of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>master<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ID of the primary instance. If this parameter is not returned, the current instance is a primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>net<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}`Internet` for public network or `Intranet` for private network.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>port</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection port.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>readonly<wbr>Instance<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}A list of IDs of read-only instances attached to the primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>region<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Region ID the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>temp<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}If a temporary instance is attached to the current instance, the ID of the temporary instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>vpc<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>vswitch<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>availability_<wbr>zone</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Availability zone.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>charge_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Billing method. Value options: `Postpaid` for Pay-As-You-Go and `Prepaid` for subscription.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>connection<wbr>Mode</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Standard` for standard access mode and `Safe` for high security access mode.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>connection_<wbr>string</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection string.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>create_<wbr>time</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Creation time of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>db_<wbr>instance_<wbr>storage_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) The storage type of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>db_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Primary` for primary instance, `Readonly` for read-only instance, `Guard` for disaster recovery instance, and `Temp` for temporary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>engine</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database type. Options are `MySQL`, `SQLServer`, `PostgreSQL` and `PPAS`. If no value is specified, all types are returned.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>engine_<wbr>version</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>expire<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Expiration time. Pay-As-You-Go instances never expire.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>guard<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}If a disaster recovery instance is attached to the current instance, the ID of the disaster recovery instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>instance_<wbr>storage</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) User-defined DB instance storage space.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>instance_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Sizing of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>master<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the primary instance. If this parameter is not returned, the current instance is a primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the RDS instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>net_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}`Internet` for public network or `Intranet` for private network.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>port</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(Available in 1.70.3+) RDS database connection port.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>readonly<wbr>Instance<wbr>Ids</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}A list of IDs of read-only instances attached to the primary instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>region<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Region ID the instance belongs to.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Status of the instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>temp<wbr>Instance<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}If a temporary instance is attached to the current instance, the ID of the temporary instance applies.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>vpc_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified VPC.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>vswitch_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Used to retrieve instances belong to specified `vswitch` resources.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}






