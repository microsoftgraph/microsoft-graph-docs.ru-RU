---
title: Обновление системы образования
description: Обновление объекта назначения. Это могут сделать только преподаватели в классе. Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения. Чтобы изменить состояние назначения, используйте действие публикации.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fcaed5b3c73039aeac6c1861a8b1ddcd4e5f19d8
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629207"
---
# <a name="update-educationassignment"></a>Обновление системы образования

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление объекта назначения. Это могут сделать только преподаватели в классе. Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения. Чтобы [изменить](../api/educationassignment-publish.md) состояние назначения, используйте действие публикации.

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
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|addedStudentAction|Строка| Управление поведением учащихся, добавленных после публикации задания.|
|allowLateSubmissions|Логический| Можно ли отправку представлений после даты.|
|allowStudentsToAddResourcesToSubmission|Логический| Может ли учащийся добавлять ресурсы в отправку. Указано, поступили ли из списка ресурсов назначения только элементы, указанные в представлении. |
|assignDateTime|DateTimeOffset| Дата публикации назначения учащимся. |
|assignTo|educationAssignmentRecipient| Студенты, получаювшие назначение.|
|closeDateTime|DateTimeOffset| Дата закрытия назначения для отправки. Это необязательный поле, которое может быть равно нуль, если назначение не позволяет использоватьLateSubmissions или closeDateTime то же самое, что и dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.|
|displayName|Строка| Имя назначения. |
|dueDateTime|DateTimeOffset| Назначение даты должно быть. |
|классификация|educationAssignmentGradeType| Оценка назначения.|
|инструкции|itemBody| Инструкции, которые будут даны учащимся вместе с назначением. |
|notificationChannelUrl|Строка| Канал для публикации уведомления о публикации назначения. Обновление URL-адреса канала не допускается после публикации назначения и допускается только в том случае, если **значение assignTo** является [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
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
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "closeDateTime": "2014-02-11T00:00:00Z",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
}
```

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


