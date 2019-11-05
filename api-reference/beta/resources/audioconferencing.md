---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонной линии для собрания по сети.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c392eb82be9e0f8c30353f18b393589b51649a3e
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969216"
---
# <a name="audioconferencing-resource-type"></a>Тип ресурса АудиоконференЦинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
