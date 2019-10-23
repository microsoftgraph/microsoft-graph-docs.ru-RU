---
title: Тип ресурса Кондитионалакцесссессионконтролс
description: Представляет сложный тип элементов управления сеанса, который принудительно применяется после входа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 317120eb7c4138d955bf8a35030375180d5a1631
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638549"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>Тип ресурса Кондитионалакцесссессионконтролс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элементы управления сеансом, которые применяются после входа.
Все элементы управления сеансом наследуются от [кондитионалакцесссессионконтрол](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|аппликатионенфорцедрестриктионс|[аппликатионенфорцедрестриктионссессионконтрол](applicationenforcedrestrictionssessioncontrol.md)| Управление сеансами для применения ограничений приложений. Этот элемент управления сеансом поддерживают только Exchange Online и SharePoint Online. |
|клаудаппсекурити|[клаудаппсекуритисессионконтрол](cloudappsecuritysessioncontrol.md)| Управление сеансами для применения Cloud App Security.|
|персистентбровсер|[персистентбровсерсессионконтрол](persistentbrowsersessioncontrol.md)| Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie. Для правильной работы этого элемента управления сеансом необходимо выбрать все приложения. |
|сигнинфрекуенци|[сигнинфрекуенцисессионконтрол](signinfrequencysessioncontrol.md)| Управление сеансами для применения частоты входа.|

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