---
title: тип ресурса chatMessagePolicyViolationPolicyTip
description: Представляет свойства подсказки политики на объекте chatMessagePolicyViolation. Советы по политике предоставляют отправительу сведения о нарушении политики.
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4373475c4219c05b1bdf7ea741c0ed6526253d234da916e0760a3ed46fee3312
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169664"
---
# <a name="chatmessagepolicytip-resource-type"></a>тип ресурса chatMessagePolicyTip

Представляет свойства подсказки политики на [объекте chatMessagePolicyViolation.](chatmessagepolicyviolation.md) Советы по политике предоставляют отправительу сведения о нарушении политики.
Советы по политике обычно устанавливаются приложением по предотвращению потери данных (DLP), которое следит за сообщениями, которые содержат данные, которые не должны отправлять пользователи.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|complianceUrl|Строка|URL-адрес, который пользователь может посетить, чтобы прочитать о политиках предотвращения потери данных для организации. (т. е. политики о том, что пользователи не должны говорить в чатах)|
|generalText|Строка|Пояснительный текст, показанный отправителю сообщения.|
|matchedConditionDescriptions|string collection|Список неправильных данных в сообщении, обнаруженном приложением для предотвращения потери данных. Каждое приложение DLP определяет свои условия, примеры включают "Номер кредитной карты" и "Номер социального обеспечения".|

## <a name="json-representation"></a>Представление JSON

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
