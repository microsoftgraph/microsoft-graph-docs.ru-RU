---
title: Upload для назначений и представлений для образования с помощью API microsoft Graph
description: Узнайте, как загрузить файл на назначение или ресурс отправки с помощью API образования в Microsoft Graph.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 0d7c60fbb88c6c6eec9f4748f2921a800f20b99e2248d6f6c26cad188591721c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54151797"
---
# <a name="upload-files-for-education-assignments-and-submissions-using-the-microsoft-graph-api"></a>Upload для назначений и представлений для образования с помощью API microsoft Graph

Ресурсы являются неотъемлемой частью [назначений](/graph/api/resources/educationassignment) и подчинений в [области образования.](/graph/api/resources/educationsubmission) Преподаватели определяют ресурсы для отправки в папку назначения, а учащиеся определяют ресурсы для отправки в папку отправки.

В этой статье описывается использование API образования в Microsoft Graph для отправки файлов в папку назначения или отправки.

## <a name="prerequisites"></a>Необходимые условия

Прежде чем загружать файлы, SharePoint папку, в которую можно загрузить файлы [](/graph/api/resources/educationassignment) для данного учебного назначения или ресурса [submisstion.](/graph/api/resources/educationsubmission) 

## <a name="upload-a-resource"></a>Upload ресурс

API `setUpResourcesFolder` возвращает модель, содержаную **свойство resourcesFolderUrl.**

```http
{
    ...
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GFA"
    ...
}
```
Ниже описано, как загрузить ресурс или файл в соответствующую папку ресурса.

### <a name="step-1---construct-the-upload-url"></a>Шаг 1 . Создание URL-адреса отправки
Создайте URL-адрес для отправки контента в этом конкретном `{resourcesFolderUrl}:/{Name of new file}:/content` формате. В следующем примере показан URL-адрес загрузки, содержащий **свойство resourcesFolderUrl.**

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
```

### <a name="step-2---upload-the-resource-to-sharepoint"></a>Шаг 2 — Upload ресурс для SharePoint
Сделайте PUT-запрос с URL-адресом загрузки для отправки контента.

Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.

Дополнительные сведения [см. в Upload больших файлов с сеансом загрузки.](/graph/api/driveitem-createuploadsession)

#### <a name="request-example"></a>Пример запроса
Ниже показан пример запроса.

```http
PUT https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
Content-Type: text/plain

Binary data for the file
```

#### <a name="response-example"></a>Пример ответа
Ниже показан пример отклика.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#drives('b%216SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F')/items/$entity",
    "@microsoft.graph.downloadUrl": "...",
    "createdDateTime": "2021-03-11T18:49:47Z",
    "eTag": "\"{EDD00CE7-B74C-4C3E-BA3E-484CB41EF31D},1\"",
    "id": "01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
    "lastModifiedDateTime": "2021-03-11T18:49:47Z",
    "name": "MyPictureFile.png",
    "webUrl": "https://contososdorg.sharepoint.com/sites/GraphTest/Class%20Files/Assignments/Test%20File%20Distribution/MyPictureFile.png",
    "cTag": "\"c:{EDD00CE7-B74C-4C3E-BA3E-484CB41EF31D},2\"",
    "size": 2302233,
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "email": "t-james@contososd.org",
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": "James"
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "email": "t-james@contososd.org",
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": "James"
        }
    },
    "parentReference": {
        "driveId": "b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F",
        "driveType": "documentLibrary",
        "id": "01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
        "path": "/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/root:/Assignments/Test File Distribution"
    },
    "file": {
        "mimeType": "image/png",
        "hashes": {
            "quickXorHash": "CvYQxN7MCGrIsdrA38c6wWhOu5g="
        }
    },
    "fileSystemInfo": {
        "createdDateTime": "2021-03-11T18:49:47Z",
        "lastModifiedDateTime": "2021-03-11T18:49:47Z"
    },
    "image": {}
}
```

### <a name="step-3---construct-the-value-for-the-fileurl-property"></a>Шаг 3 . Построение значения для свойства fileUrl
Создайте значение для **свойства fileUrl** с помощью следующего формата: `https://graph.microsoft.com/v1.0/drives/{drive-id}/items/{item-id}` . Замените эти значения на значения, описанные `{drive-id}` `{item-id}` в следующей таблице.

| Заполнитель | Описание | Пример |
|:--|:--|:--|
| `{drive-id}` | Drive ID из URL-адреса запроса, используемого в шаге 2. | b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F |
| `{item-id}` | ID элемента из тела ответа, полученного в шаге 2. | 01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ |

В следующем примере показан **файлUrl,** основанный на этом формате.

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ
```

### <a name="step-4---create-educationassignmentresource"></a>Шаг 4 . Создание educationAssignmentResource
На этом шаге показано, как загрузить SharePoint в папку ресурсов назначения.

Используйте `fileUrl` предыдущий шаг в теле запроса, чтобы [создать educationAssignmentResource](/graph/api/educationassignment-post-resources).

#### <a name="request-example"></a>Пример запроса
Ниже показан пример запроса.

```http
POST https://graph.microsoft.com/v1.0/education/classes/b07edbef-7420-4b3d-8f7c-d599cf21e069/assignments/48b80dff-452a-4108-bd85-fa0d84e39d0a/resources
Content-type: application/json

{
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
        "displayName": "Parts of a Sonnet"
    }
}
```

#### <a name="response-example"></a>Пример ответа
Ниже показан пример отклика.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('48b80dff-452a-4108-bd85-fa0d84e39d0a')/resources/$entity",
    "distributeForStudentWork": false,
    "id": "ff1aafe4-ae89-49c3-8366-4b509f640d6a",
    "resource": {
        "@odata.type": "#microsoft.graph.educationFileResource",
        "displayName": "Parts of a Sonnet",
        "createdDateTime": "2021-03-11T18:35:40.6642039Z",
        "lastModifiedDateTime": "2021-03-11T18:35:40.6642039Z",
        "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
                "displayName": null
            }
        }
    }
}
```

Теперь вы успешно загрузили ресурс SharePoint в папку ресурсов назначения (и прикрепили его к связанному назначению). Вы можете выполнять аналогичные действия, чтобы загрузить один или несколько ресурсов работы учащихся. Дополнительные сведения см. в [материале Create educationSubmissionResource](/graph/api/educationsubmission-post-resources).
