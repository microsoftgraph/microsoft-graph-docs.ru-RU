---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонии для Онлинемитинг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1371e80830bf148588f6bda91326b0521fcdda42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328376"
---
# <a name="audioconferencing-resource-type"></a>Тип ресурса АудиоконференЦинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| Диалинурл           | String  | URL-адрес веб-страницы, которая содержит сведения о телефонном доступе. |
| Леадерпасскоде      | String  | Пароль заполнения, необходимый для подключения к поставщику конференции с аудио-и видеоКонференциями.      |
| ПартиЦипантпасскоде | String  | Пароль участника, необходимый для подключения к поставщику конференции с аудио-и видеоКонференциями. |
| Толлфринумбер      | String  | Бесплатный номер для подключения к поставщику конференции с аудио.              |
| Толлнумбер          | String  | Платный номер для подключения к поставщику конференции с аудио-и видеоКонференциями.                   |

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
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
