---
title: Создание outlookTask
description: Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4de57847638ef98347a7561291d12486468428ee
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869458"
---
# <a name="create-outlooktask"></a>Создание outlookTask

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.

Метод POST всегда игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе.

По умолчанию эта операция (а также операции GET, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC. Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Tasks.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Tasks.ReadWrite    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Prefer: outlook.timezone | Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан. Необязательное свойство.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [OutlookTask](../resources/outlooktask.md) в формате JSON.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В приведенном ниже примере показано использование `Prefer: outlook.timezone` заголовка. Он создает задачу, выражает **startDateTime** и **Дуедатетиме** в восточное стандартное время (EST) и включает `Prefer` заголовку тихоокеанского стандартного времени (PST).
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "assignedTo": "Dana Swope",
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
В тексте запроса добавьте представление объекта [OutlookTask](../resources/outlooktask.md) в формате JSON.
##### <a name="response"></a>Ответ
Метод POST игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе (EST).

Так как `Prefer` заголовок указывает PST-файл, метод POST выражает все свойства, связанные с датами, в ответе в PST-файле. В частности, для свойств **startDateTime** и **дуедатетиме** метод POST преобразовывает полночь в СРЕДСТВе EST в PST-файл и возвращает их в PST-файле в ответе.

Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
