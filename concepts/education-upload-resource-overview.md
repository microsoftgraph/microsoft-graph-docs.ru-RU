---
title: Отправка файлов для заданий и отправок для образовательных учреждений
description: Узнайте, как отправить файл в задание или ресурс отправки с помощью API для образования в Microsoft Graph.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: f6c3f9a3a35e89ed935105e6320c4f7c652b288f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440875"
---
# <a name="upload-files-for-education-assignments-and-submissions-using-the-microsoft-graph-api"></a>Отправка файлов для образовательных заданий и отправки с помощью microsoft API Graph

Ресурсы являются неотъемлемой частью [назначений и](/graph/api/resources/educationassignment) [отправок для образовательных учреждений](/graph/api/resources/educationsubmission). Преподаватели определяют ресурсы для отправки в папку заданий, а учащиеся — ресурсы для отправки в папку отправки.

В этой статье описывается, как использовать API образования в Microsoft Graph для отправки файлов в папку назначения или отправки.

## <a name="prerequisites"></a>Предварительные условия

Перед отправкой файлов необходимо настроить папку SharePoint, в которую будут отправляться файлы для заданного назначения образования или ресурса отправки.

## <a name="upload-a-resource"></a>Отправка ресурса

API `setUpResourcesFolder` возвращает модель, содержащую **свойство resourcesFolderUrl** .

```http
{
    ...
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GFA"
    ...
}
```

Ниже описано, как отправить ресурс или файл в соответствующую папку ресурсов.

### <a name="step-1---construct-the-upload-url"></a>Шаг 1. Создание URL-адреса отправки
Создайте URL-адрес для отправки содержимого в указанном формате `{resourcesFolderUrl}:/{Name of new file}:/content`. В следующем примере показан URL-адрес отправки, содержащий **свойство resourcesFolderUrl** .

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
```

### <a name="step-2---upload-the-resource-to-sharepoint"></a>Шаг 2. Отправка ресурса в SharePoint
Выполните запрос PUT с URL-адресом отправки, чтобы отправить содержимое.

Содержимое текста запроса должно представлять собой двоичный поток файла, который необходимо отправить.

Дополнительные сведения см. в статье ["Отправка больших файлов с помощью сеанса отправки"](/graph/api/driveitem-createuploadsession).

#### <a name="request"></a>Запрос

Ниже показан пример запроса.

```http
PUT https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2:/MyPictureFile.png:/content
Content-Type: text/plain

Binary data for the file
```

#### <a name="response"></a>Отклик

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

### <a name="step-3---construct-the-value-for-the-fileurl-property"></a>Шаг 3. Создание значения для свойства fileUrl
Создайте значение свойства **fileUrl** в следующем формате: `https://graph.microsoft.com/v1.0/drives/{drive-id}/items/{item-id}` Замените `{drive-id}` заполнители `{item-id}` значениями, описанными в следующей таблице.

| Заполнитель | Описание | Пример |
|:--|:--|:--|
| `{drive-id}` | Идентификатор диска из URL-адреса запроса, используемого на шаге 2. | b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F |
| `{item-id}` | Идентификатор элемента из текста ответа, полученного на шаге 2. | 01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ |

В следующем примере показан **fileUrl** на основе этого формата.

```http
https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJU7DAXTU6XLOJGYWYMTGM5JT5UQ
```

### <a name="step-4---create-educationassignmentresource"></a>Шаг 4. Создание educationAssignmentResource
На этом шаге показано, как отправить ресурс SharePoint в папку ресурсов назначения.

Используйте предыдущий `fileUrl` шаг в тексте запроса для [создания educationAssignmentResource](/graph/api/educationassignment-post-resources).

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик

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

Вы успешно отправили ресурс SharePoint в папку ресурсов назначения (и подключили его к связанному назначению). Чтобы отправить один или несколько рабочих ресурсов учащихся, выполните аналогичные действия.

Дополнительные сведения см [. в разделе Create educationSubmissionResource](/graph/api/educationsubmission-post-resources).
