
---
title: "PodSecurityPolicyTemplate"
block_external_search_index: true
---






## Create a PodSecurityPolicyTemplate Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#PodSecurityPolicyTemplate">PodSecurityPolicyTemplate</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#PodSecurityPolicyTemplateArgs">PodSecurityPolicyTemplateArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">PodSecurityPolicyTemplate</span><span class="p">(resource_name, opts=None, </span>allow_privilege_escalation=None<span class="p">, </span>allowed_capabilities=None<span class="p">, </span>allowed_csi_drivers=None<span class="p">, </span>allowed_flex_volumes=None<span class="p">, </span>allowed_host_paths=None<span class="p">, </span>allowed_proc_mount_types=None<span class="p">, </span>allowed_unsafe_sysctls=None<span class="p">, </span>annotations=None<span class="p">, </span>default_add_capabilities=None<span class="p">, </span>default_allow_privilege_escalation=None<span class="p">, </span>description=None<span class="p">, </span>forbidden_sysctls=None<span class="p">, </span>fs_group=None<span class="p">, </span>host_ipc=None<span class="p">, </span>host_network=None<span class="p">, </span>host_pid=None<span class="p">, </span>host_ports=None<span class="p">, </span>labels=None<span class="p">, </span>name=None<span class="p">, </span>privileged=None<span class="p">, </span>read_only_root_filesystem=None<span class="p">, </span>required_drop_capabilities=None<span class="p">, </span>run_as_group=None<span class="p">, </span>run_as_user=None<span class="p">, </span>runtime_class=None<span class="p">, </span>se_linux=None<span class="p">, </span>supplemental_group=None<span class="p">, </span>volumes=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewPodSecurityPolicyTemplate<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateArgs">PodSecurityPolicyTemplateArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplate">PodSecurityPolicyTemplate</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.PodSecurityPolicyTemplate.html">PodSecurityPolicyTemplate</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.PodSecurityPolicyTemplateArgs.html">PodSecurityPolicyTemplateArgs</a></span>? <span class="nx">args = null<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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

    <dt class="property-optional"
            title="Optional">
        <span>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Csi<wbr>Drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Flex<wbr>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Host<wbr>Paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Proc<wbr>Mount<wbr>Types</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Unsafe<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Add<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Forbidden<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fs<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Network</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Read<wbr>Only<wbr>Root<wbr>Filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Required<wbr>Drop<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>User</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Runtime<wbr>Class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Se<wbr>Linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Supplemental<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Csi<wbr>Drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Flex<wbr>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Host<wbr>Paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Proc<wbr>Mount<wbr>Types</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Unsafe<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Add<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Forbidden<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fs<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Network</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Read<wbr>Only<wbr>Root<wbr>Filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Required<wbr>Drop<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>User</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Runtime<wbr>Class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Se<wbr>Linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Supplemental<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Csi<wbr>Drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Flex<wbr>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Host<wbr>Paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Proc<wbr>Mount<wbr>Types</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Unsafe<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default<wbr>Add<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default<wbr>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>forbidden<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fs<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Network</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>read<wbr>Only<wbr>Root<wbr>Filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>required<wbr>Drop<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run<wbr>As<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run<wbr>As<wbr>User</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>runtime<wbr>Class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>se<wbr>Linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>supplemental<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>allow_<wbr>privilege_<wbr>escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>csi_<wbr>drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>flex_<wbr>volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>host_<wbr>paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>proc_<wbr>mount_<wbr>types</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>unsafe_<wbr>sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default_<wbr>add_<wbr>capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default_<wbr>allow_<wbr>privilege_<wbr>escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>forbidden_<wbr>sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fs_<wbr>group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>network</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>read_<wbr>only_<wbr>root_<wbr>filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>required_<wbr>drop_<wbr>capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run_<wbr>as_<wbr>group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run_<wbr>as_<wbr>user</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>runtime_<wbr>class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>se_<wbr>linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>supplemental_<wbr>group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Look up an Existing PodSecurityPolicyTemplate Resource

Get an existing PodSecurityPolicyTemplate resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#PodSecurityPolicyTemplateState">PodSecurityPolicyTemplateState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#PodSecurityPolicyTemplate">PodSecurityPolicyTemplate</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>allow_privilege_escalation=None<span class="p">, </span>allowed_capabilities=None<span class="p">, </span>allowed_csi_drivers=None<span class="p">, </span>allowed_flex_volumes=None<span class="p">, </span>allowed_host_paths=None<span class="p">, </span>allowed_proc_mount_types=None<span class="p">, </span>allowed_unsafe_sysctls=None<span class="p">, </span>annotations=None<span class="p">, </span>default_add_capabilities=None<span class="p">, </span>default_allow_privilege_escalation=None<span class="p">, </span>description=None<span class="p">, </span>forbidden_sysctls=None<span class="p">, </span>fs_group=None<span class="p">, </span>host_ipc=None<span class="p">, </span>host_network=None<span class="p">, </span>host_pid=None<span class="p">, </span>host_ports=None<span class="p">, </span>labels=None<span class="p">, </span>name=None<span class="p">, </span>privileged=None<span class="p">, </span>read_only_root_filesystem=None<span class="p">, </span>required_drop_capabilities=None<span class="p">, </span>run_as_group=None<span class="p">, </span>run_as_user=None<span class="p">, </span>runtime_class=None<span class="p">, </span>se_linux=None<span class="p">, </span>supplemental_group=None<span class="p">, </span>volumes=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetPodSecurityPolicyTemplate<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateState">PodSecurityPolicyTemplateState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplate">PodSecurityPolicyTemplate</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.PodSecurityPolicyTemplate.html">PodSecurityPolicyTemplate</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..PodSecurityPolicyTemplateState.html">PodSecurityPolicyTemplateState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Csi<wbr>Drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Flex<wbr>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Host<wbr>Paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Proc<wbr>Mount<wbr>Types</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Unsafe<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Add<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Forbidden<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fs<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Network</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary&lt;string, object&gt;</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Read<wbr>Only<wbr>Root<wbr>Filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Required<wbr>Drop<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>User</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Runtime<wbr>Class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Se<wbr>Linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Supplemental<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Csi<wbr>Drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Flex<wbr>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Host<wbr>Paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Proc<wbr>Mount<wbr>Types</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Unsafe<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Add<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Forbidden<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fs<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Network</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host<wbr>Ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Read<wbr>Only<wbr>Root<wbr>Filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Required<wbr>Drop<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Run<wbr>As<wbr>User</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Runtime<wbr>Class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Se<wbr>Linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Supplemental<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Csi<wbr>Drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Flex<wbr>Volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Host<wbr>Paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Proc<wbr>Mount<wbr>Types</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Unsafe<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default<wbr>Add<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default<wbr>Allow<wbr>Privilege<wbr>Escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>forbidden<wbr>Sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fs<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Network</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host<wbr>Ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>read<wbr>Only<wbr>Root<wbr>Filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>required<wbr>Drop<wbr>Capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run<wbr>As<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run<wbr>As<wbr>User</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>runtime<wbr>Class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>se<wbr>Linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>supplemental<wbr>Group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>allow_<wbr>privilege_<wbr>escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}allowPrivilegeEscalation determines if a pod can request to allow privilege escalation. If unspecified, defaults to
true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>csi_<wbr>drivers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedcsidriver">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>flex_<wbr>volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedflexvolume">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>host_<wbr>paths</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateallowedhostpath">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>proc_<wbr>mount_<wbr>types</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>unsafe_<wbr>sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Annotations for PodSecurityPolicyTemplate object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default_<wbr>add_<wbr>capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default_<wbr>allow_<wbr>privilege_<wbr>escalation</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The PodSecurityPolicyTemplate description (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>forbidden_<wbr>sysctls</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fs_<wbr>group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgroup">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>ipc</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>network</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}hostNetwork determines if the policy allows the use of HostNetwork in the pod spec.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>pid</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host_<wbr>ports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatehostport">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Labels for PodSecurityPolicyTemplate object (map)
* `allow_privilege_escalation` = (Optional)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>privileged</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>read_<wbr>only_<wbr>root_<wbr>filesystem</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>required_<wbr>drop_<wbr>capabilities</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run_<wbr>as_<wbr>group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgroup">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>run_<wbr>as_<wbr>user</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuser">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>runtime_<wbr>class</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateruntimeclass">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>se_<wbr>linux</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinux">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>supplemental_<wbr>group</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgroup">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>volumes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Csi<wbr>Driver</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateAllowedCsiDriver">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateAllowedCsiDriver">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateAllowedCsiDriverArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateAllowedCsiDriverOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the PodSecurityPolicyTemplate (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Flex<wbr>Volume</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateAllowedFlexVolume">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateAllowedFlexVolume">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateAllowedFlexVolumeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateAllowedFlexVolumeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Driver</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Driver</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>driver</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>driver</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Allowed<wbr>Host<wbr>Path</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateAllowedHostPath">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateAllowedHostPath">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateAllowedHostPathArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateAllowedHostPathOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Path<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Read<wbr>Only</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Path<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Read<wbr>Only</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>path<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>read<wbr>Only</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>path<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>read<wbr>Only</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateFsGroup">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateFsGroup">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateFsGroupArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateFsGroupOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgrouprange">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Range<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgrouprange">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Range</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgrouprange">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Range[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatefsgrouprange">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Range]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Fs<wbr>Group<wbr>Range</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateFsGroupRange">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateFsGroupRange">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateFsGroupRangeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateFsGroupRangeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Host<wbr>Port</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateHostPort">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateHostPort">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateHostPortArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateHostPortOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateRunAsGroup">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateRunAsGroup">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsGroupArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsGroupOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgrouprange">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Range<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgrouprange">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Range</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgrouprange">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Range[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasgrouprange">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Range]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>Group<wbr>Range</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateRunAsGroupRange">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateRunAsGroupRange">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsGroupRangeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsGroupRangeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateRunAsUser">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateRunAsUser">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsUserArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsUserOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuserrange">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Range<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuserrange">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Range</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuserrange">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Range[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplaterunasuserrange">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Range]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Run<wbr>As<wbr>User<wbr>Range</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateRunAsUserRange">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateRunAsUserRange">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsUserRangeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRunAsUserRangeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Runtime<wbr>Class</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateRuntimeClass">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateRuntimeClass">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRuntimeClassArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateRuntimeClassOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Allowed<wbr>Runtime<wbr>Class<wbr>Names</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Runtime<wbr>Class<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Allowed<wbr>Runtime<wbr>Class<wbr>Names</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Default<wbr>Runtime<wbr>Class<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>allowed<wbr>Runtime<wbr>Class<wbr>Names</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default<wbr>Runtime<wbr>Class<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>allowed<wbr>Runtime<wbr>Class<wbr>Names</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>default<wbr>Runtime<wbr>Class<wbr>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateSeLinux">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateSeLinux">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSeLinuxArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSeLinuxOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Se<wbr>Linux<wbr>Option</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinuxselinuxoption">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Se<wbr>Linux<wbr>Option<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Se<wbr>Linux<wbr>Option</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinuxselinuxoption">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Se<wbr>Linux<wbr>Option</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>se<wbr>Linux<wbr>Option</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinuxselinuxoption">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Se<wbr>Linux<wbr>Option</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>se<wbr>Linux<wbr>Option</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplateselinuxselinuxoption">Dict[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Se<wbr>Linux<wbr>Option]</a></span>
    </dt>
    <dd>{{% md %}}(list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Se<wbr>Linux<wbr>Se<wbr>Linux<wbr>Option</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateSeLinuxSeLinuxOption">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateSeLinuxSeLinuxOption">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSeLinuxSeLinuxOptionArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSeLinuxSeLinuxOptionOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Level</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Role</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Level</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Role</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>level</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>role</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>level</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>role</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateSupplementalGroup">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateSupplementalGroup">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSupplementalGroupArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSupplementalGroupOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgrouprange">List&lt;Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Range<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgrouprange">[]Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Range</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgrouprange">Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Range[]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>ranges</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#podsecuritypolicytemplatesupplementalgrouprange">List[Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Range]</a></span>
    </dt>
    <dd>{{% md %}}(list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}(string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Pod<wbr>Security<wbr>Policy<wbr>Template<wbr>Supplemental<wbr>Group<wbr>Range</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#PodSecurityPolicyTemplateSupplementalGroupRange">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#PodSecurityPolicyTemplateSupplementalGroupRange">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSupplementalGroupRangeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#PodSecurityPolicyTemplateSupplementalGroupRangeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Max</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Min</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>max</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>min</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}(int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-rancher2">https://github.com/pulumi/pulumi-rancher2</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
