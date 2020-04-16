
---
title: "LocallySignedCert"
block_external_search_index: true
---






## Create a LocallySignedCert Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/tls/#LocallySignedCert">LocallySignedCert</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/tls/#LocallySignedCertArgs">LocallySignedCertArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">LocallySignedCert</span><span class="p">(resource_name, opts=None, </span>allowed_uses=None<span class="p">, </span>ca_cert_pem=None<span class="p">, </span>ca_key_algorithm=None<span class="p">, </span>ca_private_key_pem=None<span class="p">, </span>cert_request_pem=None<span class="p">, </span>early_renewal_hours=None<span class="p">, </span>is_ca_certificate=None<span class="p">, </span>set_subject_key_id=None<span class="p">, </span>validity_period_hours=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewLocallySignedCert<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-tls/sdk/go/tls/?tab=doc#LocallySignedCertArgs">LocallySignedCertArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-tls/sdk/go/tls/?tab=doc#LocallySignedCert">LocallySignedCert</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Tls/Pulumi.Tls.LocallySignedCert.html">LocallySignedCert</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Tls/Pulumi.Tls.LocallySignedCertArgs.html">LocallySignedCertArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Allowed<wbr>Uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ca<wbr>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ca<wbr>Key<wbr>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ca<wbr>Private<wbr>Key<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cert<wbr>Request<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Validity<wbr>Period<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Early<wbr>Renewal<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Ca<wbr>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Set<wbr>Subject<wbr>Key<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Allowed<wbr>Uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ca<wbr>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ca<wbr>Key<wbr>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Ca<wbr>Private<wbr>Key<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cert<wbr>Request<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Validity<wbr>Period<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Early<wbr>Renewal<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Ca<wbr>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Set<wbr>Subject<wbr>Key<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>allowed<wbr>Uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ca<wbr>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ca<wbr>Key<wbr>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ca<wbr>Private<wbr>Key<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cert<wbr>Request<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>validity<wbr>Period<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>early<wbr>Renewal<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is<wbr>Ca<wbr>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>set<wbr>Subject<wbr>Key<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>allowed_<wbr>uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ca_<wbr>cert_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ca_<wbr>key_<wbr>algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>ca_<wbr>private_<wbr>key_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cert_<wbr>request_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>validity_<wbr>period_<wbr>hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>early_<wbr>renewal_<wbr>hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is_<wbr>ca_<wbr>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>set_<wbr>subject_<wbr>key_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## LocallySignedCert Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ready<wbr>For<wbr>Renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Validity<wbr>End<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Validity<wbr>Start<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Ready<wbr>For<wbr>Renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Validity<wbr>End<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Validity<wbr>Start<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ready<wbr>For<wbr>Renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>validity<wbr>End<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>validity<wbr>Start<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>cert_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>ready_<wbr>for_<wbr>renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>validity_<wbr>end_<wbr>time</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>validity_<wbr>start_<wbr>time</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing LocallySignedCert Resource

Get an existing LocallySignedCert resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/tls/#LocallySignedCertState">LocallySignedCertState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/tls/#LocallySignedCert">LocallySignedCert</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>allowed_uses=None<span class="p">, </span>ca_cert_pem=None<span class="p">, </span>ca_key_algorithm=None<span class="p">, </span>ca_private_key_pem=None<span class="p">, </span>cert_pem=None<span class="p">, </span>cert_request_pem=None<span class="p">, </span>early_renewal_hours=None<span class="p">, </span>is_ca_certificate=None<span class="p">, </span>ready_for_renewal=None<span class="p">, </span>set_subject_key_id=None<span class="p">, </span>validity_end_time=None<span class="p">, </span>validity_period_hours=None<span class="p">, </span>validity_start_time=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetLocallySignedCert<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-tls/sdk/go/tls/?tab=doc#LocallySignedCertState">LocallySignedCertState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-tls/sdk/go/tls/?tab=doc#LocallySignedCert">LocallySignedCert</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Tls/Pulumi.Tls.LocallySignedCert.html">LocallySignedCert</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Tls/Pulumi.Tls..LocallySignedCertState.html">LocallySignedCertState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Allowed<wbr>Uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">List&lt;string&gt;</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ca<wbr>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ca<wbr>Key<wbr>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ca<wbr>Private<wbr>Key<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cert<wbr>Request<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Early<wbr>Renewal<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Ca<wbr>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ready<wbr>For<wbr>Renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Set<wbr>Subject<wbr>Key<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Validity<wbr>End<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Validity<wbr>Period<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Validity<wbr>Start<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Allowed<wbr>Uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ca<wbr>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ca<wbr>Key<wbr>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ca<wbr>Private<wbr>Key<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cert<wbr>Request<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Early<wbr>Renewal<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Is<wbr>Ca<wbr>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ready<wbr>For<wbr>Renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Set<wbr>Subject<wbr>Key<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Validity<wbr>End<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Validity<wbr>Period<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Validity<wbr>Start<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>allowed<wbr>Uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ca<wbr>Cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ca<wbr>Key<wbr>Algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ca<wbr>Private<wbr>Key<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cert<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cert<wbr>Request<wbr>Pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>early<wbr>Renewal<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is<wbr>Ca<wbr>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ready<wbr>For<wbr>Renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>set<wbr>Subject<wbr>Key<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>validity<wbr>End<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>validity<wbr>Period<wbr>Hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>validity<wbr>Start<wbr>Time</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>allowed_<wbr>uses</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}List of keywords each describing a use that is permitted
for the issued certificate. The valid keywords are listed below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ca_<wbr>cert_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}PEM-encoded certificate data for the CA.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ca_<wbr>key_<wbr>algorithm</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the algorithm for the key provided
in `ca_private_key_pem`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ca_<wbr>private_<wbr>key_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}PEM-encoded private key data for the CA.
This can be read from a separate file using the ``file`` interpolation
function.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cert_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The certificate data in PEM format.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cert_<wbr>request_<wbr>pem</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}PEM-encoded request certificate data.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>early_<wbr>renewal_<wbr>hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Number of hours before the certificates expiry when a new certificate will be generated
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>is_<wbr>ca_<wbr>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Boolean controlling whether the CA flag will be set in the
generated certificate. Defaults to `false`, meaning that the certificate does not represent
a certificate authority.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ready_<wbr>for_<wbr>renewal</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>set_<wbr>subject_<wbr>key_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If `true`, the certificate will include
the subject key identifier. Defaults to `false`, in which case the subject
key identifier is not set at all.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>validity_<wbr>end_<wbr>time</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The time until which the certificate is invalid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>validity_<wbr>period_<wbr>hours</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The number of hours after initial issuing that the
certificate will become invalid.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>validity_<wbr>start_<wbr>time</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The time after which the certificate is valid, as an
[RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}











<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-tls">https://github.com/pulumi/pulumi-tls</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
