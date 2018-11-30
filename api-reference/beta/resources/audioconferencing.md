---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
ms.openlocfilehash: dd23c6ade282e081482a8c079491644c663b4054
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077136"
---
# <a name="audioconferencing-resource-type"></a>Тип ресурса audioConferencing

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Description                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | URL-адрес, доступном веб-страницу, которая содержит данные для подключения. |
| leaderPasscode      | String  | Ведущий сотрудник, пароль для подключения к поставщику конференции звук.      |
| participantPasscode | String  | Участников пароль, необходимый для подключения к поставщику конференции звук. |
| tollFreeNumber      | String  | Бесплатный номер для подключения к поставщику конференции звук.              |
| tollNumber          | String  | Бесплатный номер для подключения к поставщику конференции звук.                   |

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
