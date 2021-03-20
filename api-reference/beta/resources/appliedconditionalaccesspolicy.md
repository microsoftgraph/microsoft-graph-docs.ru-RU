---
title: тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ffb91b315772d017ce039237e353df68daa47bfc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952317"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>тип ресурса appliedConditionalAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|условия, удовлетворяемые|conditionalAccessConditions|Относится к условиям политики условного доступа, которые удовлетворены. Возможные значения: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|conditionsNotSatisfied|conditionalAccessConditions|Относится к условиям политики условного доступа, которые не удовлетворены. Возможные значения: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|enforcedGrantControls|Коллекция строк|Относится к средствам управления грантами, которые применяются в политике условного доступа (пример: "Требуется многофакторная проверка подлинности").|
|enforcedSessionControls|Коллекция строк|Относится к средствам управления сеансами, которые применяются в политике условного доступа (пример: "Требуется принудительное управление приложениями").|
|id|Строка|Идентификатор политики условного доступа.|
|result|appliedConditionalAccessPolicyResult| Указывает результат срабатываемой политики ЦС. Возможные значения: , , (Политика не применяется, так как условия политики не были выполнены), (Это связано с политикой в состоянии `success` `failure` `notApplied` `notEnabled` отключена), `unknown` , , , `unknownFutureValue` `reportOnlySuccess` `reportOnlyFailure` , `reportOnlyNotApplied``reportOnlyInterrupted`|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
