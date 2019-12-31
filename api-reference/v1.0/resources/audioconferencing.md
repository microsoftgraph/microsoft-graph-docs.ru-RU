---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонной линии для собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1c58fb5cbf65b73aed2978fd0b3be45d7d30aec
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913480"
---
# <a name="audioconferencing-resource-type"></a>Тип ресурса АудиоконференЦинг

Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| диалинурл           | String  | URL-адрес веб-страницы, которая содержит сведения о телефонном доступе. |
| конференцеид        | String  | Идентификатор конференции онлайн-собрания.      |
| толлфринумбер      | String  | Бесплатный номер, который подключается к поставщику конференции с аудио.              |
| толлнумбер          | String  | Платный номер, который подключается к поставщику конференции с аудио-и видеоконференциями.                   |

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
  "ConferenceId": "String",
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
