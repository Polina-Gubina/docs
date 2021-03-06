# Querying Snapshot Details<a name="dws_02_0025"></a>

## Function<a name="s89d994cb1803492fb7ab0b764e10efc5"></a>

This API is used to query snapshot details by using the snapshot ID.

## URI<a name="s7407bbbf9740421f9f01edb6677acb7b"></a>

-   URI format

    GET /v1.0/\{project\_id\}/snapshots/\{snapshot\_id\}

-   Parameter description

    **Table  1**  URI parameter description

    <a name="t03cf4133264f4eeaaab4a31d429215f7"></a>
    <table><thead align="left"><tr id="ra40f56bbc733415dbc94e95224e3c8df"><th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.1"><p id="a103a6d2ad01048f197bb0ed6abfbe4c7"><a name="a103a6d2ad01048f197bb0ed6abfbe4c7"></a><a name="a103a6d2ad01048f197bb0ed6abfbe4c7"></a><strong id="b84235270617228"><a name="b84235270617228"></a><a name="b84235270617228"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.2.5.1.2"><p id="aa273af51098f4b73884a23e5e6af5a2e"><a name="aa273af51098f4b73884a23e5e6af5a2e"></a><a name="aa273af51098f4b73884a23e5e6af5a2e"></a><strong id="b6167984116271"><a name="b6167984116271"></a><a name="b6167984116271"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="a2b3ec64214494c5391296825cc730af5"><a name="a2b3ec64214494c5391296825cc730af5"></a><a name="a2b3ec64214494c5391296825cc730af5"></a><strong id="b84235270617235"><a name="b84235270617235"></a><a name="b84235270617235"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.5.1.4"><p id="a176c26c00df5439dbf463a74decabf21"><a name="a176c26c00df5439dbf463a74decabf21"></a><a name="a176c26c00df5439dbf463a74decabf21"></a><strong id="b842352706172443"><a name="b842352706172443"></a><a name="b842352706172443"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r10f89c70109a41b3bad04a491ed4f5fb"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="aae3836ab27c5469a91cc91f7e6b5d227"><a name="aae3836ab27c5469a91cc91f7e6b5d227"></a><a name="aae3836ab27c5469a91cc91f7e6b5d227"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.2 "><p id="a46a358d48fcb4f488efa2de8851c9a43"><a name="a46a358d48fcb4f488efa2de8851c9a43"></a><a name="a46a358d48fcb4f488efa2de8851c9a43"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="ac702291c6f984acfb02da49d2c5896e1"><a name="ac702291c6f984acfb02da49d2c5896e1"></a><a name="ac702291c6f984acfb02da49d2c5896e1"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.5.1.4 "><p id="p1861525155610"><a name="p1861525155610"></a><a name="p1861525155610"></a>Project ID. For details about how to obtain the project ID, see <a href="obtaining-a-project-id.md">Obtaining a Project ID</a>.</p>
    </td>
    </tr>
    <tr id="r6fa9c1b6e62c4257bd4f9a6cc2676086"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="a832201223dd44d51830b8cfa3ca50ae7"><a name="a832201223dd44d51830b8cfa3ca50ae7"></a><a name="a832201223dd44d51830b8cfa3ca50ae7"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.2 "><p id="ab05840a30a4f4e61beca2259c4b889ed"><a name="ab05840a30a4f4e61beca2259c4b889ed"></a><a name="ab05840a30a4f4e61beca2259c4b889ed"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="afc6d8115ff184be09f739b207b2f2a17"><a name="afc6d8115ff184be09f739b207b2f2a17"></a><a name="afc6d8115ff184be09f739b207b2f2a17"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.5.1.4 "><p id="a40c17c2778c24a5abb577474cb6b305a"><a name="a40c17c2778c24a5abb577474cb6b305a"></a><a name="a40c17c2778c24a5abb577474cb6b305a"></a>Snapshot ID</p>
    </td>
    </tr>
    </tbody>
    </table>


## Request<a name="sc41be71f816145c98a3a0cbc0570f81c"></a>

Sample request

```
GET /v1.0/89cd04f168b84af6be287f71730fdb4b/snapshots/b5c45780-1006-49e3-b2d5-b3229975bbc7
```

## Response<a name="sb51fdf6952534594a77e5ca943b4d031"></a>

-   Sample response

    ```
    STATUS CODE 200
    {
        "snapshot": {
            "id": "2a4d0f86-67cd-408a-8b66-017454fb7793",
            "name": "snapshot-1",
            "description": "snapshot description",
            "started": "2016-08-23T03:59:23Z",
            "finished": "2016-08-23T04:01:40Z", 
            "size": 500,
            "status": "AVAILABLE",
            "type": "MANUAL",
            "cluster_id": "4f87d3c4-9e33-482f-b962-e23b30d1a18c"
        }
    }
    ```

-   Parameter description

    **Table  2**  Response parameter description

    <a name="t286df71005a04fc9a3e3bd3b64972842"></a>
    <table><thead align="left"><tr id="r7049a9917fae4de497534fa9eb3bafc7"><th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.1"><p id="a269f59f271c0463f9f00e6986dea722e"><a name="a269f59f271c0463f9f00e6986dea722e"></a><a name="a269f59f271c0463f9f00e6986dea722e"></a><strong id="b837378704"><a name="b837378704"></a><a name="b837378704"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="a57290f6cefdd4799aec005c6d7df117e"><a name="a57290f6cefdd4799aec005c6d7df117e"></a><a name="a57290f6cefdd4799aec005c6d7df117e"></a><strong id="b127747341"><a name="b127747341"></a><a name="b127747341"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="11%" id="mcps1.2.5.1.3"><p id="afd268fcc97c44d5ea561c7f9ebf73103"><a name="afd268fcc97c44d5ea561c7f9ebf73103"></a><a name="afd268fcc97c44d5ea561c7f9ebf73103"></a><strong id="b1723398280"><a name="b1723398280"></a><a name="b1723398280"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="59%" id="mcps1.2.5.1.4"><p id="ac507dcac15b54256ba284f2eb53df8b8"><a name="ac507dcac15b54256ba284f2eb53df8b8"></a><a name="ac507dcac15b54256ba284f2eb53df8b8"></a><strong id="b1027883584"><a name="b1027883584"></a><a name="b1027883584"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r3a8701c6a6f54b439b3493e661020adf"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="a949dcd7ce00c4e28b9998f8cd0a9ed48"><a name="a949dcd7ce00c4e28b9998f8cd0a9ed48"></a><a name="a949dcd7ce00c4e28b9998f8cd0a9ed48"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="af050542890c6472a90174c8ac99aa240"><a name="af050542890c6472a90174c8ac99aa240"></a><a name="af050542890c6472a90174c8ac99aa240"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a9be39c039592450db2af0c42f4618e8f"><a name="a9be39c039592450db2af0c42f4618e8f"></a><a name="a9be39c039592450db2af0c42f4618e8f"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="a32849203a56b4984a5773e3e629ea981"><a name="a32849203a56b4984a5773e3e629ea981"></a><a name="a32849203a56b4984a5773e3e629ea981"></a>Snapshot object</p>
    </td>
    </tr>
    <tr id="r90d399d5d7d14d4199f460d56c4581d8"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="acd6bb391439e483da63b4e7ad6b3deec"><a name="acd6bb391439e483da63b4e7ad6b3deec"></a><a name="acd6bb391439e483da63b4e7ad6b3deec"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a1a346e3dbcf742c6ab8d5ed7983cad63"><a name="a1a346e3dbcf742c6ab8d5ed7983cad63"></a><a name="a1a346e3dbcf742c6ab8d5ed7983cad63"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a2a2635578194442f8d95b6cd9376b3d1"><a name="a2a2635578194442f8d95b6cd9376b3d1"></a><a name="a2a2635578194442f8d95b6cd9376b3d1"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="af842382abb5a4646a7d638742a5b5ca9"><a name="af842382abb5a4646a7d638742a5b5ca9"></a><a name="af842382abb5a4646a7d638742a5b5ca9"></a>Snapshot name</p>
    </td>
    </tr>
    <tr id="en-us_topic_0067625518_row6220102054"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="en-us_topic_0067625518_p503883102054"><a name="en-us_topic_0067625518_p503883102054"></a><a name="en-us_topic_0067625518_p503883102054"></a>Id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="ab79a4b5be3a34cc48a5281e42f07d3ae"><a name="ab79a4b5be3a34cc48a5281e42f07d3ae"></a><a name="ab79a4b5be3a34cc48a5281e42f07d3ae"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a5adefc0d065c4e95a976aa628116dfd2"><a name="a5adefc0d065c4e95a976aa628116dfd2"></a><a name="a5adefc0d065c4e95a976aa628116dfd2"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="a6c3b5cc0b5584fe8ae434538ad34d36a"><a name="a6c3b5cc0b5584fe8ae434538ad34d36a"></a><a name="a6c3b5cc0b5584fe8ae434538ad34d36a"></a>Snapshot ID</p>
    </td>
    </tr>
    <tr id="r484f7517176342aca341b6f52584cd06"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="aaa42bebe4c8141c89e5e9e65805b977e"><a name="aaa42bebe4c8141c89e5e9e65805b977e"></a><a name="aaa42bebe4c8141c89e5e9e65805b977e"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a29e2424c48834b25b5cbee8d4e1461af"><a name="a29e2424c48834b25b5cbee8d4e1461af"></a><a name="a29e2424c48834b25b5cbee8d4e1461af"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a7ab2a43151184e19a10d951096aea13b"><a name="a7ab2a43151184e19a10d951096aea13b"></a><a name="a7ab2a43151184e19a10d951096aea13b"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="a33c9f03d30fe4f989a6e41ff598916bd"><a name="a33c9f03d30fe4f989a6e41ff598916bd"></a><a name="a33c9f03d30fe4f989a6e41ff598916bd"></a>Snapshot description</p>
    </td>
    </tr>
    <tr id="r17a5efa8f2754cf9a4ee96a39f6235cf"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="acdd4bbff6c894d33be42524fd294e34c"><a name="acdd4bbff6c894d33be42524fd294e34c"></a><a name="acdd4bbff6c894d33be42524fd294e34c"></a>started</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a02dcc46e6dff41e8b574b5ada9bab705"><a name="a02dcc46e6dff41e8b574b5ada9bab705"></a><a name="a02dcc46e6dff41e8b574b5ada9bab705"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a664b9a095966401aa809cecc4cf23abb"><a name="a664b9a095966401aa809cecc4cf23abb"></a><a name="a664b9a095966401aa809cecc4cf23abb"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="en-us_topic_0067625518_p992554102054"><a name="en-us_topic_0067625518_p992554102054"></a><a name="en-us_topic_0067625518_p992554102054"></a>Time when a snapshot is being created. The format is <strong id="b842352706102625"><a name="b842352706102625"></a><a name="b842352706102625"></a>ISO8601: YYYY-MM-DDThh:mm:ssZ</strong>.</p>
    </td>
    </tr>
    <tr id="ra8d54ffdb8b04457ad801c1ffd779718"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="aedfb7ceef265473da25b4619b1707c21"><a name="aedfb7ceef265473da25b4619b1707c21"></a><a name="aedfb7ceef265473da25b4619b1707c21"></a>finished</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a329756e755c540748a0e6d08dca5549c"><a name="a329756e755c540748a0e6d08dca5549c"></a><a name="a329756e755c540748a0e6d08dca5549c"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a49f6c3cb18894c41aae82ced20cac177"><a name="a49f6c3cb18894c41aae82ced20cac177"></a><a name="a49f6c3cb18894c41aae82ced20cac177"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="a3107dd758a584216b6ff033c1bd04d56"><a name="a3107dd758a584216b6ff033c1bd04d56"></a><a name="a3107dd758a584216b6ff033c1bd04d56"></a>Time when a snapshot has been created. The format is <strong id="b886692990"><a name="b886692990"></a><a name="b886692990"></a>ISO8601: YYYY-MM-DDThh:mm:ssZ</strong>.</p>
    </td>
    </tr>
    <tr id="r85a5b7aeb0744424908e196af2034f94"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="a46f24c6edc884b80a431c7753ecd80c2"><a name="a46f24c6edc884b80a431c7753ecd80c2"></a><a name="a46f24c6edc884b80a431c7753ecd80c2"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a3ca3c703884243ed8df8c55386348dab"><a name="a3ca3c703884243ed8df8c55386348dab"></a><a name="a3ca3c703884243ed8df8c55386348dab"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a73ffe6b0c374417b944a7eed5967b373"><a name="a73ffe6b0c374417b944a7eed5967b373"></a><a name="a73ffe6b0c374417b944a7eed5967b373"></a>Double</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="a91f90a44a93a4d548d09f93c3def6cb9"><a name="a91f90a44a93a4d548d09f93c3def6cb9"></a><a name="a91f90a44a93a4d548d09f93c3def6cb9"></a>Snapshot size, expressed in GB.</p>
    </td>
    </tr>
    <tr id="re4b1c330c06c429f9446919df6fde239"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="a04054d2531644f83a0d58c4ca10ebc5d"><a name="a04054d2531644f83a0d58c4ca10ebc5d"></a><a name="a04054d2531644f83a0d58c4ca10ebc5d"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a9a11e9e8c2a9445a870c6ba6790ef06d"><a name="a9a11e9e8c2a9445a870c6ba6790ef06d"></a><a name="a9a11e9e8c2a9445a870c6ba6790ef06d"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="afcbbc691158341ffbb51a9e75ca45a71"><a name="afcbbc691158341ffbb51a9e75ca45a71"></a><a name="afcbbc691158341ffbb51a9e75ca45a71"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="adf0b604d9aaf4363a69b5aa2312dc629"><a name="adf0b604d9aaf4363a69b5aa2312dc629"></a><a name="adf0b604d9aaf4363a69b5aa2312dc629"></a>Snapshot status, which can be one of the following:</p>
    <a name="udf0d101452ed491a907d4b00ec92cf88"></a><a name="udf0d101452ed491a907d4b00ec92cf88"></a><ul id="udf0d101452ed491a907d4b00ec92cf88"><li><strong id="b842352706152546"><a name="b842352706152546"></a><a name="b842352706152546"></a>CREATING</strong></li><li><strong id="b335382630162424"><a name="b335382630162424"></a><a name="b335382630162424"></a>AVAILABLE</strong></li><li><strong id="b842352706162411"><a name="b842352706162411"></a><a name="b842352706162411"></a>UNAVAILABLE</strong></li></ul>
    </td>
    </tr>
    <tr id="r2fb09bd79b17477a9f95642b2ddbc046"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="a5dd0fd159f14454bbfc35d61518dc77e"><a name="a5dd0fd159f14454bbfc35d61518dc77e"></a><a name="a5dd0fd159f14454bbfc35d61518dc77e"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="a9adf25345218456bbfa0da59f155d416"><a name="a9adf25345218456bbfa0da59f155d416"></a><a name="a9adf25345218456bbfa0da59f155d416"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a280f7934aabe4b9d873e838e699af9ad"><a name="a280f7934aabe4b9d873e838e699af9ad"></a><a name="a280f7934aabe4b9d873e838e699af9ad"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="a8078aed728754520860cc227e34bfbe7"><a name="a8078aed728754520860cc227e34bfbe7"></a><a name="a8078aed728754520860cc227e34bfbe7"></a>Snapshot creation type. Currently, only <strong id="b842352706103021"><a name="b842352706103021"></a><a name="b842352706103021"></a>MANUAL</strong> is supported.</p>
    </td>
    </tr>
    <tr id="rd0b8a38eb8664d5bb4a6c7d6a1f71fad"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="a685f53e3375746a7ae580a6d64e2685d"><a name="a685f53e3375746a7ae580a6d64e2685d"></a><a name="a685f53e3375746a7ae580a6d64e2685d"></a>cluster_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="af6ed9dc5d1b047eeacb399a06974d5d9"><a name="af6ed9dc5d1b047eeacb399a06974d5d9"></a><a name="af6ed9dc5d1b047eeacb399a06974d5d9"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="11%" headers="mcps1.2.5.1.3 "><p id="a7cc54cc7aecc4940a085592242af3b55"><a name="a7cc54cc7aecc4940a085592242af3b55"></a><a name="a7cc54cc7aecc4940a085592242af3b55"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.5.1.4 "><p id="ad638d5d896084d26a92981a7676003c0"><a name="ad638d5d896084d26a92981a7676003c0"></a><a name="ad638d5d896084d26a92981a7676003c0"></a>ID of the cluster for which a snapshot is created</p>
    </td>
    </tr>
    </tbody>
    </table>


## Returned Value<a name="s0432ac0acf0e4c35952c6e583e5d13a4"></a>

-   Normal

    200

-   Abnormal 

    **Table  3**  Returned value description

    <a name="t381a0ce367d34c508c15bc62556c80f4"></a>
    <table><thead align="left"><tr id="rc705680fb2d44dbea0322e22ce21b85e"><th class="cellrowborder" valign="top" width="46.46%" id="mcps1.2.3.1.1"><p id="a4e92675d7662463086acf80dd01c8299"><a name="a4e92675d7662463086acf80dd01c8299"></a><a name="a4e92675d7662463086acf80dd01c8299"></a><strong id="b842352706103533"><a name="b842352706103533"></a><a name="b842352706103533"></a>Returned Value</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="53.54%" id="mcps1.2.3.1.2"><p id="ae785c47579d34128850726851a808230"><a name="ae785c47579d34128850726851a808230"></a><a name="ae785c47579d34128850726851a808230"></a><strong id="b682285030"><a name="b682285030"></a><a name="b682285030"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r3c21fd4cb9df4b97b4b800659bfbcbed"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="a3cb3e8a40aca472e944ad6981f3e8a48"><a name="a3cb3e8a40aca472e944ad6981f3e8a48"></a><a name="a3cb3e8a40aca472e944ad6981f3e8a48"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="abb6964c16e004d95b78ce00379b65cc0"><a name="abb6964c16e004d95b78ce00379b65cc0"></a><a name="abb6964c16e004d95b78ce00379b65cc0"></a>Request error.</p>
    </td>
    </tr>
    <tr id="r314d45ff59464052ae6c90e8fcc76800"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="a7a241515b87a4bba895c94f9ace0318f"><a name="a7a241515b87a4bba895c94f9ace0318f"></a><a name="a7a241515b87a4bba895c94f9ace0318f"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a590948f2b5484b99830f4e0afc7030f6"><a name="a590948f2b5484b99830f4e0afc7030f6"></a><a name="a590948f2b5484b99830f4e0afc7030f6"></a>Authentication failed.</p>
    </td>
    </tr>
    <tr id="r33a4470852684858b432c23386a051c9"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="aeba1b717f92a44299ddf7e5b92d81821"><a name="aeba1b717f92a44299ddf7e5b92d81821"></a><a name="aeba1b717f92a44299ddf7e5b92d81821"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a62a4fed7d99345468707e253dee3b3f2"><a name="a62a4fed7d99345468707e253dee3b3f2"></a><a name="a62a4fed7d99345468707e253dee3b3f2"></a>You do not have the rights to perform the operation.</p>
    </td>
    </tr>
    <tr id="rf23a577fe6a84045a9addb87bfc2da25"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="a343a5e29aa844df2ba85be45a607f911"><a name="a343a5e29aa844df2ba85be45a607f911"></a><a name="a343a5e29aa844df2ba85be45a607f911"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a6b4ec79bfc1f45678966da755eb28cc7"><a name="a6b4ec79bfc1f45678966da755eb28cc7"></a><a name="a6b4ec79bfc1f45678966da755eb28cc7"></a>The requested resource was not found.</p>
    </td>
    </tr>
    <tr id="rf507ef9a9bc8412fac9ceb00dbdbb364"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="acfaef90a1b4d42209a6e5b1f4ca08086"><a name="acfaef90a1b4d42209a6e5b1f4ca08086"></a><a name="acfaef90a1b4d42209a6e5b1f4ca08086"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="a7b9d99229b044a258e022e746fea6321"><a name="a7b9d99229b044a258e022e746fea6321"></a><a name="a7b9d99229b044a258e022e746fea6321"></a>Internal service error.</p>
    </td>
    </tr>
    <tr id="ra1c6c79a882f4a8db7f0e3426f8d03fb"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.2.3.1.1 "><p id="acb193a6ede6e45ef8969ecb5cea0a1d4"><a name="acb193a6ede6e45ef8969ecb5cea0a1d4"></a><a name="acb193a6ede6e45ef8969ecb5cea0a1d4"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.2.3.1.2 "><p id="ac9a027cbb22f4276bf57e0cf057559f6"><a name="ac9a027cbb22f4276bf57e0cf057559f6"></a><a name="ac9a027cbb22f4276bf57e0cf057559f6"></a>The service is unavailable.</p>
    </td>
    </tr>
    </tbody>
    </table>


