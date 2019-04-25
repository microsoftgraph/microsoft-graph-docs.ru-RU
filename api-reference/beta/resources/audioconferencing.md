---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонии для Онлинемитинг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535574"
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

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
