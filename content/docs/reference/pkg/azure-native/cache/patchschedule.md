
---
title: "PatchSchedule"
title_tag: "azure-native.cache.PatchSchedule"
meta_desc: "Documentation for the azure-native.cache.PatchSchedule resource with examples, input properties, output properties, lookup functions, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Response to put/get patch schedules for Redis cache.
API Version: 2020-06-01.

{{% examples %}}
## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}
### RedisCachePatchSchedulesCreateOrUpdate
{{% example csharp %}}
```csharp
using Pulumi;
using AzureNative = Pulumi.AzureNative;

class MyStack : Stack
{
    public MyStack()
    {
        var patchSchedule = new AzureNative.Cache.PatchSchedule("patchSchedule", new AzureNative.Cache.PatchScheduleArgs
        {
            Default = "default",
            Name = "cache1",
            ResourceGroupName = "rg1",
            ScheduleEntries = 
            {
                new AzureNative.Cache.Inputs.ScheduleEntryArgs
                {
                    DayOfWeek = "Monday",
                    MaintenanceWindow = "PT5H",
                    StartHourUtc = 12,
                },
                new AzureNative.Cache.Inputs.ScheduleEntryArgs
                {
                    DayOfWeek = "Tuesday",
                    StartHourUtc = 12,
                },
            },
        });
    }

}

```

{{% /example %}}

{{% example go %}}

```go
package main

import (
	cache "github.com/pulumi/pulumi-azure-native/sdk/go/azure/cache"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := cache.NewPatchSchedule(ctx, "patchSchedule", &cache.PatchScheduleArgs{
			Default:           pulumi.String("default"),
			Name:              pulumi.String("cache1"),
			ResourceGroupName: pulumi.String("rg1"),
			ScheduleEntries: cache.ScheduleEntryArray{
				&cache.ScheduleEntryArgs{
					DayOfWeek:         "Monday",
					MaintenanceWindow: pulumi.String("PT5H"),
					StartHourUtc:      pulumi.Int(12),
				},
				&cache.ScheduleEntryArgs{
					DayOfWeek:    "Tuesday",
					StartHourUtc: pulumi.Int(12),
				},
			},
		})
		if err != nil {
			return err
		}
		return nil
	})
}

```

{{% /example %}}

{{% example python %}}

```python
import pulumi
import pulumi_azure_native as azure_native

patch_schedule = azure_native.cache.PatchSchedule("patchSchedule",
    default="default",
    name="cache1",
    resource_group_name="rg1",
    schedule_entries=[
        azure_native.cache.ScheduleEntryArgs(
            day_of_week="Monday",
            maintenance_window="PT5H",
            start_hour_utc=12,
        ),
        azure_native.cache.ScheduleEntryArgs(
            day_of_week="Tuesday",
            start_hour_utc=12,
        ),
    ])

```

{{% /example %}}

{{% example typescript %}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure_native from "@pulumi/azure-native";

const patchSchedule = new azure_native.cache.PatchSchedule("patchSchedule", {
    "default": "default",
    name: "cache1",
    resourceGroupName: "rg1",
    scheduleEntries: [
        {
            dayOfWeek: "Monday",
            maintenanceWindow: "PT5H",
            startHourUtc: 12,
        },
        {
            dayOfWeek: "Tuesday",
            startHourUtc: 12,
        },
    ],
});

```

{{% /example %}}

{{% /examples %}}


## Create a PatchSchedule Resource {#create}
{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">PatchSchedule</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">PatchScheduleArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nx">PatchSchedule</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">, </span><span class="nx">default</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">resource_group_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">schedule_entries</span><span class="p">:</span> <span class="nx">Optional[Sequence[ScheduleEntryArgs]]</span> = None<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewPatchSchedule</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">, </span><span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">PatchScheduleArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">PatchSchedule</span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">PatchSchedule</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">, </span><span class="nx"><a href="#inputs">PatchScheduleArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">PatchScheduleArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language python %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type">
            <a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a>
        </span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
  
    <dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>
      Context object for the current deployment.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">PatchScheduleArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
  
    <dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>
      The unique name of the resource.
    </dd>
  
    <dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">PatchScheduleArgs</a></span>
    </dt>
    <dd>
      The arguments to resource properties.
    </dd>
  
    <dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>
      Bag of options to control resource&#39;s behavior.
    </dd>
  

</dl>

{{% /choosable %}}

## PatchSchedule Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) in the Programming Model docs.

### Inputs

The PatchSchedule resource accepts the following [input]({{< relref "/docs/intro/concepts/inputs-outputs" >}}) properties:



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
    <dd>{{% md %}}The name of the Redis cache.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_csharp">
<a href="#resourcegroupname_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="scheduleentries_csharp">
<a href="#scheduleentries_csharp" style="color: inherit; text-decoration: inherit;">Schedule<wbr>Entries</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#scheduleentry">List&lt;Pulumi.<wbr>Azure<wbr>Native.<wbr>Cache.<wbr>Inputs.<wbr>Schedule<wbr>Entry<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}List of patch schedules for a Redis cache.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="default_csharp">
<a href="#default_csharp" style="color: inherit; text-decoration: inherit;">Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Default string modeled as parameter for auto generation to work correctly.{{% /md %}}</dd>
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
    <dd>{{% md %}}The name of the Redis cache.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_go">
<a href="#resourcegroupname_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="scheduleentries_go">
<a href="#scheduleentries_go" style="color: inherit; text-decoration: inherit;">Schedule<wbr>Entries</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#scheduleentry">[]Schedule<wbr>Entry</a></span>
    </dt>
    <dd>{{% md %}}List of patch schedules for a Redis cache.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="default_go">
<a href="#default_go" style="color: inherit; text-decoration: inherit;">Default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Default string modeled as parameter for auto generation to work correctly.{{% /md %}}</dd>
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
    <dd>{{% md %}}The name of the Redis cache.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resourcegroupname_nodejs">
<a href="#resourcegroupname_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Group<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="scheduleentries_nodejs">
<a href="#scheduleentries_nodejs" style="color: inherit; text-decoration: inherit;">schedule<wbr>Entries</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#scheduleentry">Schedule<wbr>Entry[]</a></span>
    </dt>
    <dd>{{% md %}}List of patch schedules for a Redis cache.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="default_nodejs">
<a href="#default_nodejs" style="color: inherit; text-decoration: inherit;">default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Default string modeled as parameter for auto generation to work correctly.{{% /md %}}</dd>
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
    <dd>{{% md %}}The name of the Redis cache.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="resource_group_name_python">
<a href="#resource_group_name_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>group_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the resource group.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="schedule_entries_python">
<a href="#schedule_entries_python" style="color: inherit; text-decoration: inherit;">schedule_<wbr>entries</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#scheduleentry">Sequence[Schedule<wbr>Entry<wbr>Args]</a></span>
    </dt>
    <dd>{{% md %}}List of patch schedules for a Redis cache.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="default_python">
<a href="#default_python" style="color: inherit; text-decoration: inherit;">default</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Default string modeled as parameter for auto generation to work correctly.{{% /md %}}</dd>
</dl>
{{% /choosable %}}


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the PatchSchedule resource produces the following output properties:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.{{% /md %}}</dd>
    <dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource type.{{% /md %}}</dd>
</dl>
{{% /choosable %}}







## Supporting Types



<h4 id="dayofweek">Day<wbr>Of<wbr>Week</h4>

{{% choosable language csharp %}}
<dl class="tabular">
    <dt>Monday</dt>
    <dd>Monday</dd>
    <dt>Tuesday</dt>
    <dd>Tuesday</dd>
    <dt>Wednesday</dt>
    <dd>Wednesday</dd>
    <dt>Thursday</dt>
    <dd>Thursday</dd>
    <dt>Friday</dt>
    <dd>Friday</dd>
    <dt>Saturday</dt>
    <dd>Saturday</dd>
    <dt>Sunday</dt>
    <dd>Sunday</dd>
    <dt>Everyday</dt>
    <dd>Everyday</dd>
    <dt>Weekend</dt>
    <dd>Weekend</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="tabular">
    <dt>Day<wbr>Of<wbr>Week<wbr>Monday</dt>
    <dd>Monday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Tuesday</dt>
    <dd>Tuesday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Wednesday</dt>
    <dd>Wednesday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Thursday</dt>
    <dd>Thursday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Friday</dt>
    <dd>Friday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Saturday</dt>
    <dd>Saturday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Sunday</dt>
    <dd>Sunday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Everyday</dt>
    <dd>Everyday</dd>
    <dt>Day<wbr>Of<wbr>Week<wbr>Weekend</dt>
    <dd>Weekend</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="tabular">
    <dt>Monday</dt>
    <dd>Monday</dd>
    <dt>Tuesday</dt>
    <dd>Tuesday</dd>
    <dt>Wednesday</dt>
    <dd>Wednesday</dd>
    <dt>Thursday</dt>
    <dd>Thursday</dd>
    <dt>Friday</dt>
    <dd>Friday</dd>
    <dt>Saturday</dt>
    <dd>Saturday</dd>
    <dt>Sunday</dt>
    <dd>Sunday</dd>
    <dt>Everyday</dt>
    <dd>Everyday</dd>
    <dt>Weekend</dt>
    <dd>Weekend</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="tabular">
    <dt>MONDAY</dt>
    <dd>Monday</dd>
    <dt>TUESDAY</dt>
    <dd>Tuesday</dd>
    <dt>WEDNESDAY</dt>
    <dd>Wednesday</dd>
    <dt>THURSDAY</dt>
    <dd>Thursday</dd>
    <dt>FRIDAY</dt>
    <dd>Friday</dd>
    <dt>SATURDAY</dt>
    <dd>Saturday</dd>
    <dt>SUNDAY</dt>
    <dd>Sunday</dd>
    <dt>EVERYDAY</dt>
    <dd>Everyday</dd>
    <dt>WEEKEND</dt>
    <dd>Weekend</dd>
</dl>
{{% /choosable %}}

<h4 id="scheduleentry">Schedule<wbr>Entry</h4>

{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="dayofweek_csharp">
<a href="#dayofweek_csharp" style="color: inherit; text-decoration: inherit;">Day<wbr>Of<wbr>Week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#dayofweek">Pulumi.<wbr>Azure<wbr>Native.<wbr>Cache.<wbr>Day<wbr>Of<wbr>Week</a></span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="starthourutc_csharp">
<a href="#starthourutc_csharp" style="color: inherit; text-decoration: inherit;">Start<wbr>Hour<wbr>Utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenancewindow_csharp">
<a href="#maintenancewindow_csharp" style="color: inherit; text-decoration: inherit;">Maintenance<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="dayofweek_go">
<a href="#dayofweek_go" style="color: inherit; text-decoration: inherit;">Day<wbr>Of<wbr>Week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#dayofweek">Day<wbr>Of<wbr>Week</a></span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="starthourutc_go">
<a href="#starthourutc_go" style="color: inherit; text-decoration: inherit;">Start<wbr>Hour<wbr>Utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenancewindow_go">
<a href="#maintenancewindow_go" style="color: inherit; text-decoration: inherit;">Maintenance<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="dayofweek_nodejs">
<a href="#dayofweek_nodejs" style="color: inherit; text-decoration: inherit;">day<wbr>Of<wbr>Week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#dayofweek">Day<wbr>Of<wbr>Week</a></span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="starthourutc_nodejs">
<a href="#starthourutc_nodejs" style="color: inherit; text-decoration: inherit;">start<wbr>Hour<wbr>Utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenancewindow_nodejs">
<a href="#maintenancewindow_nodejs" style="color: inherit; text-decoration: inherit;">maintenance<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="day_of_week_python">
<a href="#day_of_week_python" style="color: inherit; text-decoration: inherit;">day_<wbr>of_<wbr>week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#dayofweek">Day<wbr>Of<wbr>Week</a></span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="start_hour_utc_python">
<a href="#start_hour_utc_python" style="color: inherit; text-decoration: inherit;">start_<wbr>hour_<wbr>utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenance_window_python">
<a href="#maintenance_window_python" style="color: inherit; text-decoration: inherit;">maintenance_<wbr>window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

<h4 id="scheduleentryresponse">Schedule<wbr>Entry<wbr>Response</h4>

{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="dayofweek_csharp">
<a href="#dayofweek_csharp" style="color: inherit; text-decoration: inherit;">Day<wbr>Of<wbr>Week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="starthourutc_csharp">
<a href="#starthourutc_csharp" style="color: inherit; text-decoration: inherit;">Start<wbr>Hour<wbr>Utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenancewindow_csharp">
<a href="#maintenancewindow_csharp" style="color: inherit; text-decoration: inherit;">Maintenance<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="dayofweek_go">
<a href="#dayofweek_go" style="color: inherit; text-decoration: inherit;">Day<wbr>Of<wbr>Week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="starthourutc_go">
<a href="#starthourutc_go" style="color: inherit; text-decoration: inherit;">Start<wbr>Hour<wbr>Utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenancewindow_go">
<a href="#maintenancewindow_go" style="color: inherit; text-decoration: inherit;">Maintenance<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="dayofweek_nodejs">
<a href="#dayofweek_nodejs" style="color: inherit; text-decoration: inherit;">day<wbr>Of<wbr>Week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="starthourutc_nodejs">
<a href="#starthourutc_nodejs" style="color: inherit; text-decoration: inherit;">start<wbr>Hour<wbr>Utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenancewindow_nodejs">
<a href="#maintenancewindow_nodejs" style="color: inherit; text-decoration: inherit;">maintenance<wbr>Window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="day_of_week_python">
<a href="#day_of_week_python" style="color: inherit; text-decoration: inherit;">day_<wbr>of_<wbr>week</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Day of the week when a cache can be patched.{{% /md %}}</dd>
    <dt class="property-required"
            title="Required">
        <span id="start_hour_utc_python">
<a href="#start_hour_utc_python" style="color: inherit; text-decoration: inherit;">start_<wbr>hour_<wbr>utc</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Start hour after which cache patching can start.{{% /md %}}</dd>
    <dt class="property-optional"
            title="Optional">
        <span id="maintenance_window_python">
<a href="#maintenance_window_python" style="color: inherit; text-decoration: inherit;">maintenance_<wbr>window</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ISO8601 timespan specifying how much time cache patching can take. {{% /md %}}</dd>
</dl>
{{% /choosable %}}
## Import


An existing resource can be imported using its type token, name, and identifier, e.g.

```sh
$ pulumi import azure-native:cache:PatchSchedule default /subscriptions/subid/resourceGroups/rg1/providers/Microsoft.Cache/Redis/cache1/patchSchedules/default 
```




<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>
