---
title: Обновление educationassignment
description: Обновите объект назначения. Это можно сделать только преподавателей в классе. Обратите внимание на то, что запрос на исправление нельзя использовать для изменения состояния назначения. Используется для изменения состояния назначения действие опубликовать.
ms.openlocfilehash: 8b23b7ac4b971856ed7a96b4991fca2e5220d069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077562"
---
# <a name="update-educationassignment"></a>Обновление educationassignment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновите объект назначения. Это можно сделать только преподавателей в классе. Обратите внимание на то, что запрос на исправление нельзя использовать для изменения состояния назначения. Используется для изменения состояния назначения действие [Опубликовать](../api/educationassignment-publish.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadWriteBasic EduAssignments.ReadWrite  |
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
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|allowLateSubmissions|Логический| Является ли отправленные данные можно отправлять после даты выполнения.|
|allowStudentsToAddResourcesToSubmission|Логический| Является ли студента можно добавить ресурсы для отправки. Указывает, является ли только элементов на отправку поступил из списка назначений ресурсов. |
|assignDateTime|DateTimeOffset| Дата назначения должны быть опубликованы для студентов. |
|assignTo|educationAssignmentRecipient| Студентов, получение назначения.|
|displayName|String| Имя назначения. |
|dueDateTime|DateTimeOffset| Дата назначения должно быть выполнено. |
|Оценка успеваемости|educationAssignmentGradeType| Как будет выражаемым числом назначения.|
|инструкции|itemBody| Инструкции для студентов, а также назначения. |

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [educationAssignment](../resources/educationassignment.md) объекта в теле ответа.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
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
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->