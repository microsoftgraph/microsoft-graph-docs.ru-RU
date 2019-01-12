---
title: 'outlookTask: завершена'
description: 'Завершить задачу Outlook, в котором задается свойство **completedDateTime** текущей дате '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 966f5c2a6d429169cff3bd6746ebb0bace34ad15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979637"
---
# <a name="outlooktask-complete"></a>outlookTask: завершена

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Завершить задачу Outlook, в котором задается свойство **completedDateTime** текущей дате и свойство **состояние** для `completed`.

При завершении задачи в ряде повторяющихся в ответ, коллекция задач будет содержать выполненной задачи в серии и следующую задачу из серии.

Свойство **completedDateTime** представляет дату окончания задачи. Часть времени **completedDateTime** по умолчанию имеет значение полуночи в формате UTC.

По умолчанию эта операция (и операции задачи POST, GET и ИСПРАВЛЕНИЯ) возвращает свойства, связанные с даты в формате UTC. Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.

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
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Prefer: outlook.timezone | Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок. Необязательный параметр.|

## <a name="request-body"></a>Тело запроса

Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [outlookTask](../resources/outlooktask.md) в теле ответа.

## <a name="example"></a>Пример

В следующем примере указывается указанной задачи как завершенные. Указывает Тихоокеанское время (PST) в `Prefer: outlook.timezone` заголовка.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a>Ответ

Ниже приведен пример отклика. **CompletedDateTime** и другие свойства, связанные с даты в ответе выражаются в PST-файлов.

> **Примечание.** Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
    {
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
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
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
