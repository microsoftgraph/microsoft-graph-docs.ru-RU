---
title: Обновление системы образования
description: Обновление объекта educationAssigment.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: faca28843e5e9b6c6f4eadea6f9be265ff56bd9e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092366"
---
# <a name="update-educationassignment"></a>Обновление системы образования

Пространство имен: microsoft.graph

Обновление [объекта educationAssignment.](../resources/educationassignment.md) 

Выполнить это действие могут только преподаватели. 

Кроме того, запрос на изменение состояния назначения **с** помощью действия [публикации.](../api/educationassignment-publish.md) Для этого не используйте операцию PATCH.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | Не поддерживается. | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{class-id}/assignments/{assignment-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В теле запроса поставляют только значения полей, которые необходимо обновить. 

Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|addedStudentAction|Строка| Описывает, следует ли распределять назначение среди учащихся, добавленных после даты публикации назначения.|
|addToCalendarAction|educationAddToCalendarOptions|Необязательное поле для управления **поведением** назначения для добавления **назначений** в календари учащихся и преподавателей при **публикации** назначения. Допустимые значения: `none`, `studentsAndPublisher`, `studentsAndTeamOwners`, `unknownFutureValue`, `studentsOnly`. Обратите внимание, что вы должны использовать загон запроса, чтобы получить следующее значение `Prefer: include - unknown -enum-members` (ы) в этом [развиваемом переуме:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `studentsOnly` . Необязательно.|
|allowLateSubmissions|Логическое| Могут ли студенты отправлять отправку после срока.|
|allowStudentsToAddResourcesToSubmission|Логический| Может ли студент добавлять ресурсы в отправку или нет. Кроме того, указывает, соответствуют ли все ресурсы в представлении списку ресурсов назначения. |
|assignDateTime|DateTimeOffset| Указывает дату публикации назначения для учащихся. Невозможно изменить после публикации назначения.|
|assignTo|[educationAssignmentRecipient](../resources/educationassignmentrecipient.md)| Студенты, получаювшие назначение.|
|closeDateTime|DateTimeOffset| Дата закрытия назначения для отправки. Это необязательный поле, которое может быть равно нуль, если назначение не позволяет использоватьLateSubmissions или closeDateTime то же самое, что и dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.|
|displayName|Строка| Имя назначения. |
|dueDateTime|DateTimeOffset| Назначение даты должно быть. |
|классификация|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)| Оценка назначения.|
|инструкции|itemBody| Инструкции, которые будут даны учащимся вместе с назначением. |
|notificationChannelUrl|String| Канал для связи уведомлений, связанных с назначением. Чтобы изменить URL-адрес, `assignTo` установите значение [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md). URL-адрес канала не может измениться после публикации назначения.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","4679bc1b-90c5-45af-ae1a-d5357672ed39"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39
Content-type: application/json

{
    "displayName": "Reading and review test 09.03 #5",
    "instructions": {
        "contentType": "text",
        "content": "Read chapter 5 and write your review"
    },
    "dueDateTime": "2021-09-10T00:00:00Z",
    "addedStudentAction": "none"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-educationassignment-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments/$entity",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Reading and review test 09.03 #5",
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
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%224679bc1b-90c5-45af-ae1a-d5357672ed39%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
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

## <a name="see-also"></a>См. также

* [Состояния, переходы и ограничения для назначений и представлений](/graph/assignments-submissions-states-transition)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


