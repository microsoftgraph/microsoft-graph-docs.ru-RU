---
title: Тип ресурса Чатмессажеполицивиолатионполицитип
description: Представляет свойства подсказки политики для объекта Чатмессажеполицивиолатион. Подсказки политики предоставляют отправителю сведения о нарушении политики.
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7a12afbd3ffb8eac75eb89b5d2bb5095fbd2ae98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082104"
---
# <a name="chatmessagepolicytip-resource-type"></a>Тип ресурса Чатмессажеполицитип

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства подсказки политики для объекта [чатмессажеполицивиолатион](chatmessagepolicyviolation.md) . Подсказки политики предоставляют отправителю сведения о нарушении политики.
Подсказка политики обычно задается с помощью приложения защиты от потери данных (DLP), которое отслеживает сообщения, содержащие данные, которые не предполагается отправлять пользователям.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|комплианцеурл|string|URL-адрес, который пользователь может посетить для чтения сведений о политиках защиты от потери данных в Организации. (IE, политики о том, что пользователи не должны говорить в беседах)|
|женералтекст|string|Пояснительный текст, отображаемый отправителю сообщения.|
|матчедкондитиондескриптионс|Коллекция строк|Список ненужных данных в сообщении, обнаруженном приложением защиты от потери данных. Каждое приложение DLP определяет собственные условия, например "номер кредитной карты" и "номер социального страхования".|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->
```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
