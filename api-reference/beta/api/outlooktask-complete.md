---
title: 'outlookTask: завершено'
description: 'Выполните задачу Outlook, которая устанавливает для свойства **комплетеддатетиме** текущую дату. '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ba271ddb112769187a4944dbee0df324fe8ea1f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017411"
---
# <a name="outlooktask-complete-deprecated"></a>outlookTask: Complete (устарело)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Выполните задачу Outlook, которая устанавливает для свойства **комплетеддатетиме** текущую дату, а свойству **Status** — значение `completed` .

Если вы завершаете задачу в повторяющейся серии, в ответе коллекция задач будет содержать завершенную задачу в ряду и следующую задачу в ряду.

Свойство **комплетеддатетиме** представляет дату завершения задачи. По умолчанию для части времени **комплетеддатетиме** по умолчанию задается полночь UTC.

По умолчанию эта операция (и операции задания POST, GET и PATCH) Возвращает свойства, связанные с датами, в формате UTC. Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.

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
| Prefer: outlook.timezone | Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан. Необязательный параметр.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.

## <a name="example"></a>Пример

В приведенном ниже примере указанная задача отмечается как завершенная. В нем задается тихоокеанское стандартное время (PST) в `Prefer: outlook.timezone` заголовке.

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

### <a name="response"></a>Отклик

Ниже приведен пример отклика. Свойства **комплетеддатетиме** и другие связанные с датами свойства в отклике выражаются в PST-файле.

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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


