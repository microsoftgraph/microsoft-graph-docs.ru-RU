---
title: Тип ресурса Чатмессажеполицивиолатионполицитип
description: Представляет свойства подсказки политики для объекта Чатмессажеполицивиолатион. Подсказки политики предоставляют отправителю сведения о нарушении политики.
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ccc3680f5b0365e1f54e9b82743b6906750b272
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223959"
---
# <a name="chatmessagepolicytip-resource-type"></a>Тип ресурса Чатмессажеполицитип

Представляет свойства подсказки политики для объекта [чатмессажеполицивиолатион](chatmessagepolicyviolation.md) . Подсказки политики предоставляют отправителю сведения о нарушении политики.
Подсказка политики обычно задается с помощью приложения защиты от потери данных (DLP), которое отслеживает сообщения, содержащие данные, которые не предполагается отправлять пользователям.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|комплианцеурл|string|URL-адрес, который пользователь может посетить для чтения сведений о политиках защиты от потери данных в Организации. (IE, политики о том, что пользователи не должны говорить в беседах)|
|женералтекст|string|Пояснительный текст, отображаемый отправителю сообщения.|
|матчедкондитиондескриптионс|Коллекция строк|Список ненужных данных в сообщении, обнаруженном приложением защиты от потери данных. Каждое приложение DLP определяет собственные условия, например "номер кредитной карты" и "номер социального страхования".|

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
