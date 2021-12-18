---
title: Список назначений пользователя
description: Возвращает список назначений, присвоенных пользователю для всех классов.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5b489ffc2cbe900b90ea4df886cdcd8cf999be5b
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567432"
---
# <a name="list-assignments-of-a-user"></a>Список назначений пользователя

Пространство имен: microsoft.graph

Возвращает список [educationAssignment,](../resources/educationassignment.md) назначенного [для educationUser](../resources/educationuser.md) для [всех классов.](../resources/educationclass.md) 

Этот метод позволяет звонящем находить  все назначения, принадлежащие учащемуся или преподавателю, в одном вызове, а не запрашивать назначения из каждого **класса.**  В **списке** назначений содержится то,  что необходимо для получения подробных сведений о назначении из пространства **имен** класса. Используйте методы, определенные для **назначения** для всех остальных операций.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                                         |
| Application                            | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All |

Для вызова конечной точки `/me` требуется вход пользователя и, следовательно, делегированное разрешение. Разрешения приложений не поддерживаются при использовании конечной точки `/me`.

`/users/{user-id}`Конечная точка работает с делегированием разрешений и разрешений приложений.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments
GET /education/users/{user-id}/assignments
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры `$submissions` `$categories` [запроса oData и OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-the-assignments-of-the-logged-in-user"></a>Пример 1. Получить назначения в журнале пользователя

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_me_assignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/education/me/assignments
```
---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/me/assignments",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 3.1",
            "closeDateTime": "2021-11-19T07:59:00Z",
            "dueDateTime": "2021-11-19T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": false,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:56:21.1575202Z",
            "lastModifiedDateTime": "2021-11-17T16:00:30.0523446Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "published",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%223b870c07-21fe-47fb-8562-cdd6f2c281d6%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "3b870c07-21fe-47fb-8562-cdd6f2c281d6",
            "instructions": null,
            "grading": null,
            "assignTo": null,
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
        },
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 4",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:58:41.5064997Z",
            "lastModifiedDateTime": "2021-11-10T23:58:41.5304842Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "draft",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%2234ab8c17-eaae-4996-9c04-53696934e6ff%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "34ab8c17-eaae-4996-9c04-53696934e6ff",
            "instructions": null,
            "grading": null,
            "assignTo": null,
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
    ]
}
```

### <a name="example-2-get-assignments-of-a-user"></a>Пример 2. Назначение пользователя

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "get_user_assignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/education/users/f3a5344e-dbde-48b0-be24-b5b62a243836/assignments
```
---


#### <a name="response"></a>Отклик

Если пользователь пытается запросить другой пользовательский код, чем его собственный, этот метод возвращает `403 Forbidden` код ответа.

Свойства `instructions` `assignedDateTime` , и всегда будут `assignTo` отображать `resourcesFolderUrl` `webUrl` null.

Ниже приведен пример ответа. 

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/users('f3a5344e-dbde-48b0-be24-b5b62a243836')/assignments",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 3.1",
            "closeDateTime": "2021-11-19T07:59:00Z",
            "dueDateTime": "2021-11-19T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": false,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:56:21.1575202Z",
            "lastModifiedDateTime": "2021-11-17T16:00:30.0523446Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "published",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%223b870c07-21fe-47fb-8562-cdd6f2c281d6%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "3b870c07-21fe-47fb-8562-cdd6f2c281d6",
            "instructions": null,
            "grading": null,
            "assignTo": null,
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
        },
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 4",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:58:41.5064997Z",
            "lastModifiedDateTime": "2021-11-10T23:58:41.5304842Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "draft",
            "notificationChannelUrl": null,
            "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%2234ab8c17-eaae-4996-9c04-53696934e6ff%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "34ab8c17-eaae-4996-9c04-53696934e6ff",
            "instructions": null,
            "grading": null,
            "assignTo": null,
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
    ]
}
```

### <a name="example-3-get-user-assignments-with-expand-submissions"></a>Пример 3. Получить назначения пользователей с расширением отправки

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "get_user_assignments_expand_submissions"
}-->

```http
GET https://graph.microsoft.com/v1.0/education/users/80cefd93-8d88-40e2-b5d3-67898383e226/assignments?expand=submissions
```
---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

> **Примечание:** Он будет расширять представления, если у пользователя есть роль ученика, и будет нулевую для роли учителя.


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/users('80cefd93-8d88-40e2-b5d3-67898383e226')/assignments(submissions())",
    "value": [
        {
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Reading test 09.03 #4",
            "closeDateTime": null,
            "dueDateTime": "2021-09-07T00:00:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-09-13T19:18:35.2587894Z",
            "lastModifiedDateTime": "2021-09-13T19:19:56.6381405Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "assigned",
            "notificationChannelUrl": null,
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "id": "1618dfb0-3ff2-4edf-8d5c-b8f81df00e80",
            "instructions": null,
            "assignTo": null,
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 50
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
                    "id": "AAAAAAAA-0123-4567-89AB-1B4BB48C3119",
                    "displayName": null
                }
            },
            "submissions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/users('80cefd93-8d88-40e2-b5d3-67898383e226')/assignments('1618dfb0-3ff2-4edf-8d5c-b8f81df00e80')/submissions",
            "submissions": [
                {
                    "status": "working",
                    "submittedDateTime": null,
                    "unsubmittedDateTime": null,
                    "returnedDateTime": null,
                    "reassignedDateTime": null,
                    "resourcesFolderUrl": null,
                    "id": "da443246-384d-673b-32db-bdba9d7f2b51",
                    "recipient": {
                        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
                        "userId": "80cefd93-8d88-40e2-b5d3-67898383e226"
                    },
                    "submittedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
                            "displayName": null
                        }
                    },
                    "unsubmittedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": null,
                            "displayName": null
                        }
                    },
                    "returnedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": null,
                            "displayName": null
                        }
                    },
                    "reassignedBy": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": null,
                            "displayName": null
                        }
                    }
                }
            ]
        }
    ]
}        
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
