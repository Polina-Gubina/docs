# Asynchronous Job Query<a name="EN-US_TOPIC_0022473688"></a>

## Function<a name="section6534076917543"></a>

This API is an extension one. It is used to query the execution status of an asynchronous job, for example, an image exporting job.

## URI<a name="section5323664117543"></a>

GET /v1/\{project\_id\}/jobs/\{job\_id\}

[Table 1](#table4357530317543)  lists the parameters in the URI.

**Table  1**  Parameter description

<a name="table4357530317543"></a>
<table><thead align="left"><tr id="row4437355317543"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.4.1.1"><p id="p3748803717543"><a name="p3748803717543"></a><a name="p3748803717543"></a><strong id="b24725868162658"><a name="b24725868162658"></a><a name="b24725868162658"></a>Parameter</strong></p>
</th>
<th class="cellrowborder" valign="top" width="29.349999999999998%" id="mcps1.2.4.1.2"><p id="p1663218617543"><a name="p1663218617543"></a><a name="p1663218617543"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="49.220000000000006%" id="mcps1.2.4.1.3"><p id="p502984817543"><a name="p502984817543"></a><a name="p502984817543"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row476451817543"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.4.1.1 "><p id="p5038164417543"><a name="p5038164417543"></a><a name="p5038164417543"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p5438136317543"><a name="p5438136317543"></a><a name="p5438136317543"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="49.220000000000006%" headers="mcps1.2.4.1.3 "><p id="p4281427417543"><a name="p4281427417543"></a><a name="p4281427417543"></a>Specifies the project ID.</p>
</td>
</tr>
<tr id="row4978415317543"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.4.1.1 "><p id="p598456817543"><a name="p598456817543"></a><a name="p598456817543"></a>job_id</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p1498798817543"><a name="p1498798817543"></a><a name="p1498798817543"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="49.220000000000006%" headers="mcps1.2.4.1.3 "><p id="p606747617543"><a name="p606747617543"></a><a name="p606747617543"></a>Specifies the asynchronous job ID.</p>
</td>
</tr>
</tbody>
</table>

## Request<a name="section5460728517543"></a>

-   Request parameters

    None

-   Example request

    ```
    GET /v1/ac234de25c6741d2b1273da49eea1b9e/jobs/ff8080814dbd65d7014dbe0d84db0013
    ```


## Response<a name="section5889951917543"></a>

-   Response parameters

    <a name="table528379811520"></a>
    <table><thead align="left"><tr id="row1392930311520"><th class="cellrowborder" valign="top" width="19.470000000000002%" id="mcps1.1.4.1.1"><p id="p5453179311520"><a name="p5453179311520"></a><a name="p5453179311520"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.56%" id="mcps1.1.4.1.2"><p id="p574394205922"><a name="p574394205922"></a><a name="p574394205922"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="54.97%" id="mcps1.1.4.1.3"><p id="p5499914011520"><a name="p5499914011520"></a><a name="p5499914011520"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2574533511520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p499736211520"><a name="p499736211520"></a><a name="p499736211520"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p46525967205922"><a name="p46525967205922"></a><a name="p46525967205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p213318211520"><a name="p213318211520"></a><a name="p213318211520"></a>Specifies the job status. The value can be:</p>
    <p id="p1919864211520"><a name="p1919864211520"></a><a name="p1919864211520"></a><strong id="b39049298151716"><a name="b39049298151716"></a><a name="b39049298151716"></a>SUCCESS</strong>: The job is successfully executed.</p>
    <p id="p3857005011520"><a name="p3857005011520"></a><a name="p3857005011520"></a><strong id="b55570798151716"><a name="b55570798151716"></a><a name="b55570798151716"></a>FAIL</strong>: The job failed to be executed.</p>
    <p id="p1158613711520"><a name="p1158613711520"></a><a name="p1158613711520"></a><strong id="b3103968151716"><a name="b3103968151716"></a><a name="b3103968151716"></a>RUNNING</strong>: The job is in progress.</p>
    <p id="p3716637511520"><a name="p3716637511520"></a><a name="p3716637511520"></a><strong id="b39990109151716"><a name="b39990109151716"></a><a name="b39990109151716"></a>INIT</strong>: The job is being initialized.</p>
    </td>
    </tr>
    <tr id="row6606192511520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p4941574211520"><a name="p4941574211520"></a><a name="p4941574211520"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p10506968205922"><a name="p10506968205922"></a><a name="p10506968205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p4325217111520"><a name="p4325217111520"></a><a name="p4325217111520"></a>Specifies the task ID.</p>
    </td>
    </tr>
    <tr id="row5372522511520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p5677596811520"><a name="p5677596811520"></a><a name="p5677596811520"></a>job_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p45758078205922"><a name="p45758078205922"></a><a name="p45758078205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p3545068711520"><a name="p3545068711520"></a><a name="p3545068711520"></a>Specifies the job type.</p>
    </td>
    </tr>
    <tr id="row5062073411520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p663876511520"><a name="p663876511520"></a><a name="p663876511520"></a>begin_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p15416808205922"><a name="p15416808205922"></a><a name="p15416808205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p86908111520"><a name="p86908111520"></a><a name="p86908111520"></a>Specifies the start time of the job. The value is in UTC format. </p>
    </td>
    </tr>
    <tr id="row782172911520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p2958027411520"><a name="p2958027411520"></a><a name="p2958027411520"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p40801918205922"><a name="p40801918205922"></a><a name="p40801918205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p4719198811520"><a name="p4719198811520"></a><a name="p4719198811520"></a>Specifies the end time of the job. The value is in UTC format. </p>
    </td>
    </tr>
    <tr id="row2207471011520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p4322112411520"><a name="p4322112411520"></a><a name="p4322112411520"></a>error_code</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p16621098205922"><a name="p16621098205922"></a><a name="p16621098205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p1125016611520"><a name="p1125016611520"></a><a name="p1125016611520"></a>Specifies the error code.</p>
    </td>
    </tr>
    <tr id="row3414263711520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p1409017611520"><a name="p1409017611520"></a><a name="p1409017611520"></a>fail_reason</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p4131665205922"><a name="p4131665205922"></a><a name="p4131665205922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p45364511520"><a name="p45364511520"></a><a name="p45364511520"></a>Specifies the cause of the failure.</p>
    </td>
    </tr>
    <tr id="row408280811520"><td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.1.4.1.1 "><p id="p6227201211520"><a name="p6227201211520"></a><a name="p6227201211520"></a>entities</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.56%" headers="mcps1.1.4.1.2 "><p id="p66229469205922"><a name="p66229469205922"></a><a name="p66229469205922"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.97%" headers="mcps1.1.4.1.3 "><p id="p1086820511520"><a name="p1086820511520"></a><a name="p1086820511520"></a>Specifies the custom attributes of the job. If a job is properly executed, an image ID is returned. If an exception occurs on the job, an error code and associated information are returned. </p>
    </td>
    </tr>
    </tbody>
    </table>


-   Example response

    ```
    STATUS CODE 200
    ```

    ```
    {
        "status": "SUCCESS",
        "entities": {
            "image_id": "e9e91bff-14b6-4a0b-8377-4ed0813e3360"
        },
        "job_id": "ff8080814dbd65d7014dbe0d84db0013",
        "job_type": "createImageByInstance",
        "begin_time": "04-Jun-2015 18:11:06:586",
        "end_time": "",
        "error_code": null,
        "fail_reason": null
    }
    ```


## Returned Values<a name="section3678893217543"></a>

-   Normal

    200

-   Abnormal

    <a name="table395981717657"></a>
    <table><thead align="left"><tr id="row1597872817657"><th class="cellrowborder" valign="top" width="46.54%" id="mcps1.1.3.1.1"><p id="p1920862517657"><a name="p1920862517657"></a><a name="p1920862517657"></a><strong id="b68331162733"><a name="b68331162733"></a><a name="b68331162733"></a>Returned Value</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="53.459999999999994%" id="mcps1.1.3.1.2"><p id="p1239479817657"><a name="p1239479817657"></a><a name="p1239479817657"></a><strong id="b60746752162737"><a name="b60746752162737"></a><a name="b60746752162737"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row6445460017657"><td class="cellrowborder" valign="top" width="46.54%" headers="mcps1.1.3.1.1 "><p id="p5344010217657"><a name="p5344010217657"></a><a name="p5344010217657"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.459999999999994%" headers="mcps1.1.3.1.2 "><p id="p3368100917657"><a name="p3368100917657"></a><a name="p3368100917657"></a>Request error.</p>
    </td>
    </tr>
    <tr id="row3469362617657"><td class="cellrowborder" valign="top" width="46.54%" headers="mcps1.1.3.1.1 "><p id="p5872033917657"><a name="p5872033917657"></a><a name="p5872033917657"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.459999999999994%" headers="mcps1.1.3.1.2 "><p id="p5872698817657"><a name="p5872698817657"></a><a name="p5872698817657"></a>Authentication failed.</p>
    </td>
    </tr>
    <tr id="row5878084417657"><td class="cellrowborder" valign="top" width="46.54%" headers="mcps1.1.3.1.1 "><p id="p6362789617657"><a name="p6362789617657"></a><a name="p6362789617657"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.459999999999994%" headers="mcps1.1.3.1.2 "><p id="p5358597717657"><a name="p5358597717657"></a><a name="p5358597717657"></a>You do not have the rights to perform the operation.</p>
    </td>
    </tr>
    <tr id="row1251175317657"><td class="cellrowborder" valign="top" width="46.54%" headers="mcps1.1.3.1.1 "><p id="p681909217657"><a name="p681909217657"></a><a name="p681909217657"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.459999999999994%" headers="mcps1.1.3.1.2 "><p id="p1547559217657"><a name="p1547559217657"></a><a name="p1547559217657"></a>Internal service error.</p>
    </td>
    </tr>
    <tr id="row506260017657"><td class="cellrowborder" valign="top" width="46.54%" headers="mcps1.1.3.1.1 "><p id="p741745117657"><a name="p741745117657"></a><a name="p741745117657"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.459999999999994%" headers="mcps1.1.3.1.2 "><p id="p6394266717657"><a name="p6394266717657"></a><a name="p6394266717657"></a>The service is unavailable.</p>
    </td>
    </tr>
    </tbody>
    </table>


