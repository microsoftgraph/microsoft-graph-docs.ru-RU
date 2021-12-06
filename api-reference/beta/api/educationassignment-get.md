---
title: Get educationAssignment
description: Получите свойства и связи назначения.
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0124c7d22170a4337fc2053f0352b1afb3d9b630
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978422"
---
# <a name="get-educationassignment"></a>Get educationAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите свойства и связи [назначения.](../resources/educationassignment.md) 

Учащиеся могут видеть только назначения, которые им назначены; преподаватели и приложения с разрешениями на приложения могут видеть все назначения в классе.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не поставляем тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и `200 OK` объект [educationAssignment](../resources/educationassignment.md) в тексте ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request", 
  "sampleKeys":["f4a941ff-9da6-4707-ba5b-0eae93cad0b4","3c77de7f-539b-49e1-9c96-1274f2f0ee3b"],
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/3c77de7f-539b-49e1-9c96-1274f2f0ee3b
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('f4a941ff-9da6-4707-ba5b-0eae93cad0b4')/assignments/$entity",
    "classId": "f4a941ff-9da6-4707-ba5b-0eae93cad0b4",
    "displayName": "07.30 SubmissionsUploadResource Word2",
    "closeDateTime": null,
    "dueDateTime": "2021-08-01T06:59:00Z",
    "assignDateTime": null,
    "assignedDateTime": "2021-07-30T16:01:32.5518042Z",
    "allowLateSubmissions": true,
    "resourcesFolderUrl": "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeU6BLWBcGc_R6UgCKyYyTin/items/016XPCQECCTNQDGB5U4RCZFBXZBV5ZX24X",
    "createdDateTime": "2021-07-30T16:00:52.1918016Z",
    "lastModifiedDateTime": "2021-07-30T19:39:09.6384593Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "assigned",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7b%22subEntityId%22%3a%22%7b%5c%22version%5c%22%3a%5c%221.0%5c%22%2c%5c%22config%5c%22%3a%7b%5c%22classes%5c%22%3a%5b%7b%5c%22id%5c%22%3a%5c%22f4a941ff-9da6-4707-ba5b-0eae93cad0b4%5c%22%2c%5c%22displayName%5c%22%3anull%2c%5c%22assignmentIds%5c%22%3a%5b%5c%223c77de7f-539b-49e1-9c96-1274f2f0ee3b%5c%22%5d%7d%5d%7d%2c%5c%22action%5c%22%3a%5c%22navigate%5c%22%2c%5c%22view%5c%22%3a%5c%22assignment-viewer%5c%22%7d%22%2c%22channelId%22%3anull%7d",
    "addToCalendarAction": "none",
    "addedStudentAction": "none",
    "id": "3c77de7f-539b-49e1-9c96-1274f2f0ee3b",
    "instructions": {
        "content": "<div style=\"font-family: inherit; font-size: inherit; color: inherit;\">upload a word document</div>",
        "contentType": "html"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 10
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
