---
title: тип ресурса conditionalAccessSessionControls
description: Представляет сложный тип элементов управления сеансами, которые применяются после регистрации.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a531eb54d7dcb4221cd788a7f615ff006b75a648
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129945"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a>тип ресурса conditionalAccessSessionControls

Пространство имен: microsoft.graph

Представляет элементы управления сеансами, которые применяются после регистрации.
Все элементы управления сеансом [наследуются из conditionalAccesssesionControl.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationEnforcedRestrictions|[applicationEnforcedRestrictionsSessionControl](applicationenforcedrestrictionssessioncontrol.md)| Управление сеансами для применения ограничений приложения. Только Exchange Online и Sharepoint Online поддерживают управление этим сеансом. |
|cloudAppSecurity|[cloudAppSecuritySessionControl](cloudappsecuritysessioncontrol.md)| Управление сеансами для применения безопасности облачных приложений.|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет. Все приложения должны быть выбраны для правильной работы управления сеансом. |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| Управление сеансом для обеспечения частоты подписей.|

## <a name="relationships"></a>Отношения

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

