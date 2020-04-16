
---
title: "SingleValueChart"
block_external_search_index: true
---



This chart type displays a single number in a large font, representing the current value of a single metric on a plot line.

If the time period is in the past, the number represents the value of the metric near the end of the time period.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as signalfx from "@pulumi/signalfx";

const mysvchart0 = new signalfx.SingleValueChart("mysvchart0", {
    colorBy: "Dimension",
    description: "Very cool Single Value Chart",
    isTimestampHidden: true,
    maxDelay: 2,
    maxPrecision: 2,
    programText: `myfilters = filter("cluster_name", "prod") and filter("role", "search")
data("cpu.total.idle", filter=myfilters).publish()
`,
    refreshInterval: 1,
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-signalfx/blob/master/website/docs/r/single_value_chart.html.markdown.



## Create a SingleValueChart Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/signalfx/#SingleValueChart">SingleValueChart</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/signalfx/#SingleValueChartArgs">SingleValueChartArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">SingleValueChart</span><span class="p">(resource_name, opts=None, </span>color_by=None<span class="p">, </span>color_scales=None<span class="p">, </span>description=None<span class="p">, </span>is_timestamp_hidden=None<span class="p">, </span>max_delay=None<span class="p">, </span>max_precision=None<span class="p">, </span>name=None<span class="p">, </span>program_text=None<span class="p">, </span>refresh_interval=None<span class="p">, </span>secondary_visualization=None<span class="p">, </span>show_spark_line=None<span class="p">, </span>unit_prefix=None<span class="p">, </span>viz_options=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewSingleValueChart<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChartArgs">SingleValueChartArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChart">SingleValueChart</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Signalfx/Pulumi.Signalfx.SingleValueChart.html">SingleValueChart</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Signalfx/Pulumi.SignalFx.SingleValueChartArgs.html">SingleValueChartArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Program<wbr>Text</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>Scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">List&lt;Pulumi.<wbr>Signal<wbr>Fx.<wbr>Inputs.<wbr>Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Timestamp<wbr>Hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Refresh<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Secondary<wbr>Visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Show<wbr>Spark<wbr>Line</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Unit<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Viz<wbr>Options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">List&lt;Pulumi.<wbr>Signal<wbr>Fx.<wbr>Inputs.<wbr>Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Program<wbr>Text</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>Scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">[]Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Timestamp<wbr>Hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Refresh<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Secondary<wbr>Visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Show<wbr>Spark<wbr>Line</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Unit<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Viz<wbr>Options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">[]Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>program<wbr>Text</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color<wbr>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color<wbr>Scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale[]</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is<wbr>Timestamp<wbr>Hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>refresh<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>secondary<wbr>Visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>show<wbr>Spark<wbr>Line</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>unit<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>viz<wbr>Options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option[]</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>program_<wbr>text</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color_<wbr>by</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color_<wbr>scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">List[Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale]</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is_<wbr>timestamp_<wbr>hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>refresh_<wbr>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>secondary_<wbr>visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>show_<wbr>spark_<wbr>line</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>unit_<wbr>prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>viz_<wbr>options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">List[Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option]</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## SingleValueChart Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>url</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing SingleValueChart Resource

Get an existing SingleValueChart resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/signalfx/#SingleValueChartState">SingleValueChartState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/signalfx/#SingleValueChart">SingleValueChart</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>color_by=None<span class="p">, </span>color_scales=None<span class="p">, </span>description=None<span class="p">, </span>is_timestamp_hidden=None<span class="p">, </span>max_delay=None<span class="p">, </span>max_precision=None<span class="p">, </span>name=None<span class="p">, </span>program_text=None<span class="p">, </span>refresh_interval=None<span class="p">, </span>secondary_visualization=None<span class="p">, </span>show_spark_line=None<span class="p">, </span>unit_prefix=None<span class="p">, </span>url=None<span class="p">, </span>viz_options=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetSingleValueChart<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChartState">SingleValueChartState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChart">SingleValueChart</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Signalfx/Pulumi.Signalfx.SingleValueChart.html">SingleValueChart</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Signalfx/Pulumi.Signalfx..SingleValueChartState.html">SingleValueChartState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Color<wbr>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>Scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">List&lt;Pulumi.<wbr>Signal<wbr>Fx.<wbr>Inputs.<wbr>Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Timestamp<wbr>Hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Program<wbr>Text</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Refresh<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Secondary<wbr>Visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Show<wbr>Spark<wbr>Line</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Unit<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Viz<wbr>Options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">List&lt;Pulumi.<wbr>Signal<wbr>Fx.<wbr>Inputs.<wbr>Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color<wbr>Scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">[]Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Timestamp<wbr>Hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Max<wbr>Precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Program<wbr>Text</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Refresh<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Secondary<wbr>Visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Show<wbr>Spark<wbr>Line</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Unit<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Viz<wbr>Options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">[]Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>color<wbr>By</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color<wbr>Scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale[]</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is<wbr>Timestamp<wbr>Hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max<wbr>Precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>program<wbr>Text</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>refresh<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>secondary<wbr>Visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>show<wbr>Spark<wbr>Line</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>unit<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>viz<wbr>Options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option[]</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>color_<wbr>by</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Must be `"Dimension"`, `"Scale"` or `"Metric"`. `"Dimension"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color_<wbr>scales</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartcolorscale">List[Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale]</a></span>
    </dt>
    <dd>{{% md %}}Single color range including both the color to display for that range and the borders of the range. Example: `[{ gt = 60, color = "blue" }, { lte = 60, color = "yellow" }]`. Look at this [link](https://docs.signalfx.com/en/latest/charts/chart-options-tab.html).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Description of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is_<wbr>timestamp_<wbr>hidden</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to hide the timestamp in the chart. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>delay</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How long (in seconds) to wait for late datapoints
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>max_<wbr>precision</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The maximum precision to for value displayed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>program_<wbr>text</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Signalflow program text for the chart. More info [in the SignalFx docs](https://developers.signalfx.com/signalflow_analytics/signalflow_overview.html#_signalflow_programming_language).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>refresh_<wbr>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How often (in seconds) to refresh the value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>secondary_<wbr>visualization</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The type of secondary visualization. Can be `None`, `Radial`, `Linear`, or `Sparkline`. If unset, the SignalFx default is used (`None`).
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>show_<wbr>spark_<wbr>line</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Whether to show a trend line below the current value. `false` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>unit_<wbr>prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Must be `"Metric"` or `"Binary"`. `"Metric"` by default.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>url</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}URL of the chart
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>viz_<wbr>options</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#singlevaluechartvizoption">List[Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option]</a></span>
    </dt>
    <dd>{{% md %}}Plot-level customization options, associated with a publish statement.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Single<wbr>Value<wbr>Chart<wbr>Color<wbr>Scale</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/signalfx/types/input/#SingleValueChartColorScale">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/signalfx/types/output/#SingleValueChartColorScale">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChartColorScaleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChartColorScaleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Color</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Gt</span>
        <span class="property-indicator"></span>
        <span class="property-type">double</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold non-inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Gte</span>
        <span class="property-indicator"></span>
        <span class="property-type">double</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Lt</span>
        <span class="property-indicator"></span>
        <span class="property-type">double</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold non-inculsive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Lte</span>
        <span class="property-indicator"></span>
        <span class="property-type">double</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold inclusive value for this range.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Color</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Gt</span>
        <span class="property-indicator"></span>
        <span class="property-type">float64</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold non-inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Gte</span>
        <span class="property-indicator"></span>
        <span class="property-type">float64</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Lt</span>
        <span class="property-indicator"></span>
        <span class="property-type">float64</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold non-inculsive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Lte</span>
        <span class="property-indicator"></span>
        <span class="property-type">float64</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold inclusive value for this range.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>color</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>gt</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold non-inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>gte</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>lt</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold non-inculsive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>lte</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold inclusive value for this range.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>color</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>gt</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold non-inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>gte</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Indicates the lower threshold inclusive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>lt</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold non-inculsive value for this range.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>lte</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Indicates the upper threshold inclusive value for this range.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Single<wbr>Value<wbr>Chart<wbr>Viz<wbr>Option</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/signalfx/types/input/#SingleValueChartVizOption">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/signalfx/types/output/#SingleValueChartVizOption">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChartVizOptionArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/go/signalfx/?tab=doc#SingleValueChartVizOptionOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Label</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Label used in the publish statement that displays the plot (metric time series data) you want to customize.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Display<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value<wbr>Suffix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value<wbr>Unit</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
* `value_prefix`, `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Label</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Label used in the publish statement that displays the plot (metric time series data) you want to customize.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Color</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Display<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value<wbr>Suffix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value<wbr>Unit</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
* `value_prefix`, `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>label</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Label used in the publish statement that displays the plot (metric time series data) you want to customize.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>display<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value<wbr>Suffix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value<wbr>Unit</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
* `value_prefix`, `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>label</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Label used in the publish statement that displays the plot (metric time series data) you want to customize.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>color</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>display<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value<wbr>Suffix</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value<wbr>Unit</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
* `value_prefix`, `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-signalfx">https://github.com/pulumi/pulumi-signalfx</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
