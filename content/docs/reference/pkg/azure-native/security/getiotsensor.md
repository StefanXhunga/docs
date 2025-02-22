
---
title: "getIotSensor"
title_tag: "azure-native.security.getIotSensor"
meta_desc: "Documentation for the azure-native.security.getIotSensor function with examples, input properties, output properties, and supporting types."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

IoT sensor model
API Version: 2020-08-06-preview.




## Using getIotSensor {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getIotSensor<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx">GetIotSensorArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="#result">GetIotSensorResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_iot_sensor(</span><span class="nx">iot_sensor_name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">scope</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetIotSensorResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupIotSensor<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx">LookupIotSensorArgs</span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="#result">LookupIotSensorResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupIotSensor` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetIotSensor </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="#result">GetIotSensorResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx">GetIotSensorArgs</span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:


{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="iotsensorname_csharp">
<a href="#iotsensorname_csharp" style="color: inherit; text-decoration: inherit;">Iot<wbr>Sensor<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the IoT sensor{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="scope_csharp">
<a href="#scope_csharp" style="color: inherit; text-decoration: inherit;">Scope</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Scope of the query (IoT Hub, /providers/Microsoft.Devices/iotHubs/myHub){{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="iotsensorname_go">
<a href="#iotsensorname_go" style="color: inherit; text-decoration: inherit;">Iot<wbr>Sensor<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the IoT sensor{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="scope_go">
<a href="#scope_go" style="color: inherit; text-decoration: inherit;">Scope</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Scope of the query (IoT Hub, /providers/Microsoft.Devices/iotHubs/myHub){{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="iotsensorname_nodejs">
<a href="#iotsensorname_nodejs" style="color: inherit; text-decoration: inherit;">iot<wbr>Sensor<wbr>Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Name of the IoT sensor{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="scope_nodejs">
<a href="#scope_nodejs" style="color: inherit; text-decoration: inherit;">scope</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Scope of the query (IoT Hub, /providers/Microsoft.Devices/iotHubs/myHub){{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="iot_sensor_name_python">
<a href="#iot_sensor_name_python" style="color: inherit; text-decoration: inherit;">iot_<wbr>sensor_<wbr>name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Name of the IoT sensor{{% /md %}}</dd><dt class="property-required"
            title="Required">
        <span id="scope_python">
<a href="#scope_python" style="color: inherit; text-decoration: inherit;">scope</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Scope of the query (IoT Hub, /providers/Microsoft.Devices/iotHubs/myHub){{% /md %}}</dd></dl>
{{% /choosable %}}




## getIotSensor Result {#result}

The following output properties are available:



{{% choosable language csharp %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="connectivitytime_csharp">
<a href="#connectivitytime_csharp" style="color: inherit; text-decoration: inherit;">Connectivity<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Last connectivity time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="creationtime_csharp">
<a href="#creationtime_csharp" style="color: inherit; text-decoration: inherit;">Creation<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Creation time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="dynamiclearning_csharp">
<a href="#dynamiclearning_csharp" style="color: inherit; text-decoration: inherit;">Dynamic<wbr>Learning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Dynamic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learningmode_csharp">
<a href="#learningmode_csharp" style="color: inherit; text-decoration: inherit;">Learning<wbr>Mode</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Learning mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensorstatus_csharp">
<a href="#sensorstatus_csharp" style="color: inherit; text-decoration: inherit;">Sensor<wbr>Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensorversion_csharp">
<a href="#sensorversion_csharp" style="color: inherit; text-decoration: inherit;">Sensor<wbr>Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tistatus_csharp">
<a href="#tistatus_csharp" style="color: inherit; text-decoration: inherit;">Ti<wbr>Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}TI Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tiversion_csharp">
<a href="#tiversion_csharp" style="color: inherit; text-decoration: inherit;">Ti<wbr>Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}TI Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensortype_csharp">
<a href="#sensortype_csharp" style="color: inherit; text-decoration: inherit;">Sensor<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Type of sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tiautomaticupdates_csharp">
<a href="#tiautomaticupdates_csharp" style="color: inherit; text-decoration: inherit;">Ti<wbr>Automatic<wbr>Updates</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}TI Automatic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="zone_csharp">
<a href="#zone_csharp" style="color: inherit; text-decoration: inherit;">Zone</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Zone of the IoT sensor{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language go %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="connectivitytime_go">
<a href="#connectivitytime_go" style="color: inherit; text-decoration: inherit;">Connectivity<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Last connectivity time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="creationtime_go">
<a href="#creationtime_go" style="color: inherit; text-decoration: inherit;">Creation<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Creation time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="dynamiclearning_go">
<a href="#dynamiclearning_go" style="color: inherit; text-decoration: inherit;">Dynamic<wbr>Learning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Dynamic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learningmode_go">
<a href="#learningmode_go" style="color: inherit; text-decoration: inherit;">Learning<wbr>Mode</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Learning mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensorstatus_go">
<a href="#sensorstatus_go" style="color: inherit; text-decoration: inherit;">Sensor<wbr>Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensorversion_go">
<a href="#sensorversion_go" style="color: inherit; text-decoration: inherit;">Sensor<wbr>Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tistatus_go">
<a href="#tistatus_go" style="color: inherit; text-decoration: inherit;">Ti<wbr>Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}TI Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tiversion_go">
<a href="#tiversion_go" style="color: inherit; text-decoration: inherit;">Ti<wbr>Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}TI Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensortype_go">
<a href="#sensortype_go" style="color: inherit; text-decoration: inherit;">Sensor<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Type of sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tiautomaticupdates_go">
<a href="#tiautomaticupdates_go" style="color: inherit; text-decoration: inherit;">Ti<wbr>Automatic<wbr>Updates</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}TI Automatic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="zone_go">
<a href="#zone_go" style="color: inherit; text-decoration: inherit;">Zone</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Zone of the IoT sensor{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language nodejs %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="connectivitytime_nodejs">
<a href="#connectivitytime_nodejs" style="color: inherit; text-decoration: inherit;">connectivity<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Last connectivity time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="creationtime_nodejs">
<a href="#creationtime_nodejs" style="color: inherit; text-decoration: inherit;">creation<wbr>Time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Creation time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="dynamiclearning_nodejs">
<a href="#dynamiclearning_nodejs" style="color: inherit; text-decoration: inherit;">dynamic<wbr>Learning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Dynamic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learningmode_nodejs">
<a href="#learningmode_nodejs" style="color: inherit; text-decoration: inherit;">learning<wbr>Mode</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}Learning mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensorstatus_nodejs">
<a href="#sensorstatus_nodejs" style="color: inherit; text-decoration: inherit;">sensor<wbr>Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensorversion_nodejs">
<a href="#sensorversion_nodejs" style="color: inherit; text-decoration: inherit;">sensor<wbr>Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tistatus_nodejs">
<a href="#tistatus_nodejs" style="color: inherit; text-decoration: inherit;">ti<wbr>Status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}TI Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tiversion_nodejs">
<a href="#tiversion_nodejs" style="color: inherit; text-decoration: inherit;">ti<wbr>Version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}TI Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensortype_nodejs">
<a href="#sensortype_nodejs" style="color: inherit; text-decoration: inherit;">sensor<wbr>Type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Type of sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="tiautomaticupdates_nodejs">
<a href="#tiautomaticupdates_nodejs" style="color: inherit; text-decoration: inherit;">ti<wbr>Automatic<wbr>Updates</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean</span>
    </dt>
    <dd>{{% md %}}TI Automatic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="zone_nodejs">
<a href="#zone_nodejs" style="color: inherit; text-decoration: inherit;">zone</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Zone of the IoT sensor{{% /md %}}</dd></dl>
{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="connectivity_time_python">
<a href="#connectivity_time_python" style="color: inherit; text-decoration: inherit;">connectivity_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Last connectivity time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="creation_time_python">
<a href="#creation_time_python" style="color: inherit; text-decoration: inherit;">creation_<wbr>time</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Creation time of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="dynamic_learning_python">
<a href="#dynamic_learning_python" style="color: inherit; text-decoration: inherit;">dynamic_<wbr>learning</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Dynamic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource Id{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="learning_mode_python">
<a href="#learning_mode_python" style="color: inherit; text-decoration: inherit;">learning_<wbr>mode</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Learning mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource name{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensor_status_python">
<a href="#sensor_status_python" style="color: inherit; text-decoration: inherit;">sensor_<wbr>status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensor_version_python">
<a href="#sensor_version_python" style="color: inherit; text-decoration: inherit;">sensor_<wbr>version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ti_status_python">
<a href="#ti_status_python" style="color: inherit; text-decoration: inherit;">ti_<wbr>status</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}TI Status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ti_version_python">
<a href="#ti_version_python" style="color: inherit; text-decoration: inherit;">ti_<wbr>version</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}TI Version of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource type{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="sensor_type_python">
<a href="#sensor_type_python" style="color: inherit; text-decoration: inherit;">sensor_<wbr>type</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Type of sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="ti_automatic_updates_python">
<a href="#ti_automatic_updates_python" style="color: inherit; text-decoration: inherit;">ti_<wbr>automatic_<wbr>updates</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}TI Automatic mode status of the IoT sensor{{% /md %}}</dd><dt class="property-"
            title="">
        <span id="zone_python">
<a href="#zone_python" style="color: inherit; text-decoration: inherit;">zone</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Zone of the IoT sensor{{% /md %}}</dd></dl>
{{% /choosable %}}





<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure-native">https://github.com/pulumi/pulumi-azure-native</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
</dl>

