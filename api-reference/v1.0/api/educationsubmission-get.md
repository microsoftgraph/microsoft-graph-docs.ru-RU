---
title: Get educationSubmission
description: 'Извлечение определенной отправки. Объект отправки представляет работу учащегося для назначения. Ресурсы, связанные с отправкой, представляют эту работу. Увидеть и изменить представление может только учащийся, за который назначена отправка. Учитель или приложение с разрешениями на приложения имеют полный доступ ко всем отправкам. '
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fe05dce0628d8829184fd6e60b4bcff7bd23b207
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526002"
---
# <a name="get-educationsubmission"></a>Get educationSubmission

Пространство имен: microsoft.graph

Извлечение определенной [отправки.](../resources/educationsubmission.md)

Объект **отправки** представляет работу студента для [назначения.](../resources/educationassignment.md) Ресурсы, связанные с **отправкой,** представляют эту работу.

Только **назначенное** Учащемуся может видеть и изменять **отправку.** Учитель или приложение с разрешениями на приложения имеют полный доступ ко всем **отправкам.**

Оценка и отзывы от преподавателя являются частью [образованияOutcome,](../resources/educationoutcome.md) связанного с этим объектом. Добавить или изменить оценки и отзывы могут только преподаватели или приложения с разрешениями приложений. Учащиеся не будут видеть оценку или отзывы до тех пор, пока **назначение** не будет выпущено.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Приложение | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{class-id}/assignments/{assignment-id}/submissions/{submission-id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

Ниже параметров для этого метода: , , и , который `$expand` включает все предыдущие `outcomes` `resources` `submittedResources` `*` параметры. Подробные сведения см. в разделе Примеры.

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не поставляем тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [educationSubmission](../resources/educationsubmission.md) в тексте ответа.

## <a name="examples"></a>Примеры
### <a name="example-1-get-submission"></a>Пример 1. Отправка
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions/869369de-3e5a-89eb-6f2d-83cd88f860b5
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationsubmission-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечания:** Объект отклика, показанный здесь, может быть сокращен для чтения. 
>
>Если [setUpResourcesFolder](educationsubmission-setupResourcesFolder.md) еще не был вызван на этот ресурс [educationSubmission,](../resources/educationsubmission.md) свойство **resourcesFolderUrl** `null` является .

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions/$entity",
    "status": "returned",
    "submittedDateTime": "2021-11-10T00:57:17.0495233Z",
    "unsubmittedDateTime": null,
    "returnedDateTime": "2021-11-10T01:03:25.7812455Z",
    "resourcesFolderUrl": null,
    "id": "869369de-3e5a-89eb-6f2d-83cd88f860b5",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "723e2402-f503-4825-a4d5-5143fbe6f53d"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "723e2402-f503-4825-a4d5-5143fbe6f53d",
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
            "id": "afc58f1f-7c9e-4770-a448-e53ba43463a5",
            "displayName": null
        }
    }
}
```

### <a name="example-2-get-submission-with-expand-options"></a>Пример 2. Получить отправку с помощью $expand параметров
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_submission_expand"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions/869369de-3e5a-89eb-6f2d-83cd88f860b5?$expand=*
```

#### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 4492

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions(outcomes(),resources(),submittedResources())/$entity",
    "status": "returned",
    "submittedDateTime": "2021-11-10T00:57:17.0495233Z",
    "unsubmittedDateTime": null,
    "returnedDateTime": "2021-11-10T01:03:25.7812455Z",
    "resourcesFolderUrl": null,
    "id": "869369de-3e5a-89eb-6f2d-83cd88f860b5",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "723e2402-f503-4825-a4d5-5143fbe6f53d"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "723e2402-f503-4825-a4d5-5143fbe6f53d",
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
            "id": "afc58f1f-7c9e-4770-a448-e53ba43463a5",
            "displayName": null
        }
    },
    "outcomes@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions('869369de-3e5a-89eb-6f2d-83cd88f860b5')/outcomes",
    "outcomes": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "lastModifiedDateTime": null,
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "lastModifiedBy": null,
            "feedback": null,
            "publishedFeedback": null
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "lastModifiedDateTime": null,
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "lastModifiedBy": null,
            "points": null,
            "publishedPoints": null
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "lastModifiedDateTime": "2021-11-10T01:03:25.7712076Z",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            },
            "rubricQualityFeedback": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "feedback": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "feedback": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "feedback": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "feedback": null
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "columnId": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "columnId": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "columnId": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "columnId": null
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "feedback": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "feedback": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "feedback": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "feedback": null
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "a660004a-608d-4cd2-a6dc-4f43812444ee",
                    "columnId": null
                },
                {
                    "qualityId": "2c5ae75d-d347-426b-be2c-cfc81a6f0b32",
                    "columnId": null
                },
                {
                    "qualityId": "32fdea06-5cbb-4881-9093-96e59f59b8b8",
                    "columnId": null
                },
                {
                    "qualityId": "66137bd8-b9c2-40e1-a360-40b7ee75eaef",
                    "columnId": null
                }
            ]
        }
    ],
    "resources@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions('869369de-3e5a-89eb-6f2d-83cd88f860b5')/resources",
    "resources": [],
    "submittedResources@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('59069eb2-2a09-4d90-bb19-2089cc69d613')/assignments('80da1069-a635-4913-813f-d775a5470a8f')/submissions('869369de-3e5a-89eb-6f2d-83cd88f860b5')/submittedResources",
    "submittedResources": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
