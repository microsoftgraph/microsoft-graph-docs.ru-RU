---
title: Тип ресурса Кондитионалакцесссессионконтролс
description: Представляет сложный тип элементов управления сеанса, который принудительно применяется после входа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 13e1bc5b7f042634f1e4d2c9384c88fab5b96b29
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450820"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>Тип ресурса Кондитионалакцесссессионконтролс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элементы управления сеансом, которые применяются после входа.
Все элементы управления сеансом наследуются от [кондитионалакцесссессионконтрол](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|аппликатионенфорцедрестриктионс|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| Управление сеансами для применения ограничений приложений. Этот элемент управления сеансом поддерживают только Exchange Online и SharePoint Online. |
|клаудаппсекурити|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| Управление сеансами для применения Cloud App Security.|
|персистентбровсер|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie. Для правильной работы этого элемента управления сеансом необходимо выбрать все приложения. |
|сигнинфрекуенци|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| Управление сеансами для применения частоты входа.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "applicationEnforcedRestrictions",
    "persistentBrowser",
    "cloudAppSecurity",
    "signInFrequency"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessSessionControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->