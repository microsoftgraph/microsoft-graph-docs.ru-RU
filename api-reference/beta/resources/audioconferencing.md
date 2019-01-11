---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9bd8343f29a797a24044f02aa2a00bd098c35007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843626"
---
# <a name="audioconferencing-resource-type"></a>Тип ресурса audioConferencing

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | Строка  | URL-адрес, доступном веб-страницу, которая содержит данные для подключения. |
| leaderPasscode      | Строка  | Ведущий сотрудник, пароль для подключения к поставщику конференции звук.      |
| participantPasscode | Строка  | Участников пароль, необходимый для подключения к поставщику конференции звук. |
| tollFreeNumber      | Строка  | Бесплатный номер для подключения к поставщику конференции звук.              |
| tollNumber          | Строка  | Бесплатный номер для подключения к поставщику конференции звук.                   |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
