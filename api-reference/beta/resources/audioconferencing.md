---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977509"
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
