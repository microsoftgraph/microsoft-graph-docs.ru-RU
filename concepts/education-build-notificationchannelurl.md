---
title: Указание канала по умолчанию для уведомлений о назначениях для образовательных учреждений
description: Используйте API для образования в Microsoft Graph, чтобы указать канал Microsoft Teams по умолчанию для отправки уведомлений о назначении.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 392cfaeef8f4491204dcd6a1cba992ce7f07a092
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440910"
---
# <a name="specify-the-default-channel-for-education-assignment-notifications-using-the-microsoft-graph-api"></a>Укажите канал по умолчанию для уведомлений о назначениях для образовательных учреждений с помощью microsoft API Graph

В этой статье описывается, как использовать API образования в Microsoft Graph, чтобы указать канал Microsoft Teams по умолчанию для отправки уведомлений о **назначении**. Указание канала по умолчанию включает в себя создание свойства **строки notificationChannelUrl** для [educationAssignment](/graph/api/resources/educationassignment). Значение по умолчанию для этого свойства — `null`..

## <a name="prerequisites"></a>Предварительные условия

Перед созданием свойства определите соответствующую команду для назначения и имя канала.

Чтобы определить команду для назначения, в меню слева в Teams щелкните **Teams** и выберите соответствующую команду.

![Снимок экрана: команда, выбранная в элементе навигации Teams](./images/notificationchannel-team.png)

Определите соответствующий канал в выбранной команде.

![Снимок экрана: канал, выбранный в команде](./images/notificationchannel-channel.png)

## <a name="build-the-notificationchannelurl-property-value"></a>Создание значения свойства notificationChannelUrl

Ниже описано, как создать значение свойства.

### <a name="step-1---get-the-team-id-based-on-your-team-name"></a>Шаг 1. Получение идентификатора команды на основе имени команды
Чтобы найти идентификатор команды, выполните запрос GET с именем команды. Если у вас уже есть идентификатор команды, пропустите этот шаг.

#### <a name="request"></a>Запрос

Ниже показан пример запроса.

```http
GET https://graph.microsoft.com/v1.0/teams?$filter=displayName eq 'English Fall ''21'
```

#### <a name="response"></a>Отклик

Ниже показан пример отклика.

```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams",
    "@odata.count": 1,
    "value": [
        {
            "id": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "createdDateTime": null,
            "displayName": "English Fall '21",
            "description": "English Fall '21",
            "internalId": null,
            "classification": null,
            "specialization": null,
            "visibility": null,
            "webUrl": null,
            "isArchived": null,
            "isMembershipLimitedToOwners": null,
            "memberSettings": null,
            "guestSettings": null,
            "messagingSettings": null,
            "funSettings": null,
            "discoverySettings": null
        }
    ]
}
```

### <a name="step-2---get-the-channel-id-based-on-channel-name-and-team-id"></a>Шаг 2. Получение идентификатора канала на основе имени канала и идентификатора команды
Выполните запрос GET с идентификатором команды, полученным на предыдущем шаге, и именем канала. Пропустите этот шаг, если у вас уже есть идентификатор канала.

#### <a name="request"></a>Запрос

Ниже показан пример запроса.

```http
GET https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels?$filter=displayName eq 'General'
```

#### <a name="response"></a>Отклик

Ниже показан пример отклика.

```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('72a7baec-c3e9-4213-a850-f62de0adad5f')/channels",
    "@odata.count": 1,
    "value": [
        {
            "id": "19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2",
            "createdDateTime": "2021-08-25T12:33:49.124Z",
            "displayName": "General",
            "description": "English Fall '21",
            "isFavoriteByDefault": null,
            "email": "",
            "webUrl": "https://teams.microsoft.com/l/channel/19%3Ajb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1%40thread.tacv2/General?groupId=72a7baec-c3e9-4213-a850-f62de0adad5f&tenantId=b6338c92-533e-4f6d-a327-994263712399",
            "membershipType": "standard"
        }
    ]
}
```

### <a name="step-3---construct-the-value-for-the-notificationchannelurl-property"></a>Шаг 3. Создание значения для свойства notificationChannelUrl
Создайте значение свойства **notificationChannelUrl** в следующем формате: 

> `https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}` 

Замените `{team-id}` заполнители `{channel-id}` значениями, описанными в следующей таблице.

| Заполнитель | Описание | Пример |
|:--|:--|:--|
| `{team-id}` | Идентификатор команды из ответа на шаге 1. Это команда, которой принадлежит текущее назначение. | 72a7baec-c3e9-4213-a850-f62de0adad5f |
| `{channel-id}` | Идентификатор элемента из текста ответа, полученного на шаге 2. | 19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2 |

В следующем примере показан **notificationChannelUrl** на основе этого формата.

```http
https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2
```

### <a name="step-4---assign-the-value-to-the-notificationchannelurl-property-for-the-assignment"></a>Шаг 4. Назначение значения свойству notificationChannelUrl для назначения

Вы успешно создали URL-адрес, и теперь нужно назначить значение свойству. Эту операцию можно выполнить, обновив ресурсы **educationAssignment** или **educationAssignmentDefaults** .

#### <a name="example-1-update-an-educationassignment"></a>Пример 1. Обновление объекта educationAssignment

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
PATCH https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39
Content-type: application/json

{
    "displayName": "Property update",
    "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments/$entity",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Property update",
    "closeDateTime": null,
    "dueDateTime": "2021-09-10T00:00:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:57:14.6088791Z",
    "lastModifiedDateTime": "2021-09-04T15:01:35.3361649Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2",
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%224679bc1b-90c5-45af-ae1a-d5357672ed39%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addToCalendarAction": "studentsAndPublisher",
    "addedStudentAction": "none",
    "id": "4679bc1b-90c5-45af-ae1a-d5357672ed39",
    "instructions": {
        "content": "Read chapter 5 and write your review",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 50
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
    },
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    }
}
```

#### <a name="example-2-update-educationassignmentdefaults"></a>Пример 2. Обновление educationAssignmentDefaults

##### <a name="request"></a>Запрос

``` http
PATCH https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentDefaults
Content-Type: application/json

{
  "addToCalendarAction": "studentsOnly",
  "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

##### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "addedStudentAction": "assignIfOpen",
  "addToCalendarAction": "studentsOnly",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

## <a name="see-also"></a>См. также

* [Обновление educationAssignmentDefaults](/graph/api/educationassignmentdefaults-update)
* [Обновление educationAssignment](/graph/api/educationassignment-update)
