---
title: Обновление outlooktask
description: Изменения для записи свойств задачи Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526888"
---
# <a name="update-outlooktask"></a>Обновление outlooktask

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изменения для записи свойств задачи Outlook.

Свойство **completedDateTime** можно задать с действия **завершения** , или явно операции обновления. При использовании ИСПРАВЛЕНИЯ для значение **completedDateTime**, убедитесь, что вы установите **состояние** `completed` также.

По умолчанию эта операция (и POST, GET и [выполнения](../api/outlooktask-complete.md) операций задач) возвращает свойства, связанные с даты в формате UTC. Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.

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
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Prefer: outlook.timezone | Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок. Необязательный параметр.|

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|AssignedTo|String|Имя пользователя, которому назначена задача.|
|body|[itemBody](../resources/itembody.md)|Основная задача, который обычно содержит сведения о задаче. Обратите внимание на то, что поддерживается только тип HTML-код.|
|categories|Коллекция String|Категории, связанные с задачей.|
|changeKey|String|Версия задачи.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанный часовой пояс, окончания задачи.|
|createdDateTime|DateTimeOffset|Дата и время создания задачи. По умолчанию он не в формате UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства используется формат ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанный часовой пояс, которую требуется завершения задачи.|
|hasAttachments|Логическое|Значение true, если у задачи вложения.|
|importance|string|Важность события. Возможные значения: `low`, `normal`, `high`.|
|isReminderOn|Boolean|Значение true, если оповещение установлено значение Напоминать пользователю задачи.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения задачи. По умолчанию он не в формате UTC. Можно указать пользовательский часовой пояс в заголовке запроса. Значение свойства в формате ISO 8601 и всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|owner|String|Имя человека, создавшего задачу.|
|parentFolderId|String|Уникальный идентификатор родительской папки задач.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Шаблон повторения для задачи.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата и время оповещения напоминание задачи, будет выполнена.|
|sensitivity|string|Указывает уровень конфиденциальности для задачи. Возможные значения: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата в указанном часовом поясе после начала задачи.|
|status|string|Указывает состояние или хода выполнения задачи. Возможные значения: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|String|Краткое описание или название задачи.|

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [outlookTask](../resources/outlooktask.md) объект в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В следующем примере изменяется свойство **dueDateTime** и использует `Prefer: outlook.timezone` заголовка для указания выражения свойств с датами в ответ в Восточное время (ПРИБЛ).
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a>Ответ

Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
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
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
