---
title: Обновление системы образования
description: Обновление объекта educationAssigment.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d5a0015ae6c98e2a8a3355f0602027f15751c21e
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941447"
---
# <a name="update-educationassignment"></a>Обновление системы образования

Пространство имен: microsoft.graph

Обновление объекта educationAssigment. 

Выполнить это действие могут только преподаватели. 

Кроме того, запрос на изменение состояния назначения с помощью действия [публикации.](../api/educationassignment-publish.md) Для этого не используйте операцию PATCH.

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
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В теле запроса поставляют только значения полей, которые необходимо обновить. 

Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|addedStudentAction|Строка| Описывает, следует ли распределять назначение среди учащихся, добавленных после даты публикации назначения.|
|allowLateSubmissions|Boolean| Могут ли студенты отправлять отправку после срока.|
|allowStudentsToAddResourcesToSubmission|Boolean| Может ли студент добавлять ресурсы в отправку или нет. Кроме того, указывает, соответствуют ли все ресурсы в представлении списку ресурсов назначения. |
|assignDateTime|DateTimeOffset| Указывает дату публикации назначения для учащихся. |
|assignTo|educationAssignmentRecipient| Студенты, получаювшие назначение.|
|closeDateTime|DateTimeOffset| Дата закрытия назначения для отправки. Это необязательный поле, которое может быть равно нуль, если назначение не позволяет использоватьLateSubmissions или closeDateTime то же самое, что и dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.|
|displayName|Строка| Имя назначения. |
|dueDateTime|DateTimeOffset| Назначение даты должно быть. |
|классификация|educationAssignmentGradeType| Оценка назначения.|
|инструкции|itemBody| Инструкции, которые будут даны учащимся вместе с назначением. |
|notificationChannelUrl|Строка| Канал для связи уведомлений, связанных с назначением. Чтобы изменить URL-адрес, `assignTo` установите значение [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md). URL-адрес канала не может измениться после публикации назначения.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
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


