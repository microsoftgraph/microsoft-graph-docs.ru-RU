---
title: тип ресурса conditionalAccessSessionControls
description: Представляет сложный тип элементов управления сеансами, которые применяются после регистрации.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3750ced7e11c48e9e6cf92e3e6631806bb19883c
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161762"
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
|disableResilienceDefaults|Логическое| Управление сеансами, определяющая, допустимо ли для Azure AD расширение существующих сеансов на основе сведений, собранных до отключения или нет.|
|persistentBrowser|[persistentBrowserSessionControl](persistentbrowsersessioncontrol.md)| Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет. Все приложения должны быть выбраны для правильной работы управления сеансом. |
|signInFrequency|[signInFrequencySessionControl](signinfrequencysessioncontrol.md)| Управление сеансом для обеспечения частоты подписей.|

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
    "signInFrequency",
    "disableResilienceDefaults"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"},
  "disableResilienceDefaults": false
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

