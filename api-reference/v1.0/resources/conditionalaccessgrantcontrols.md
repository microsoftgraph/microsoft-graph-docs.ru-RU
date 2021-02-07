---
title: Тип ресурса conditionalAccessGrantControls
description: Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 99b6d6dc3bd15ea84c4a8507981acd9c8ac2eb6f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130790"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Тип ресурса conditionalAccessGrantControls

Пространство имен: microsoft.graph

Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | String | Определяет отношение элементов управления предоставлением. Возможные значения: `AND` , `OR` . |
| builtInControls | Коллекция String | Список значений встроенных элементов управления, необходимых для политики. Возможные значения: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` . |
| customAuthenticationFactors | Коллекция String | Список пользовательских ИД элементов управления, необходимых для политики. Дополнительные сведения см. в [настраиваемом элементе управления.](/azure/active-directory/conditional-access/controls) |
| termsOfUse | Коллекция String | Список [условий использования,](/graph/api/resources/agreement) необходимых для политики. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Особые соображения при использовании `passwordChange` в качестве управления

При использовании этого управления учитывайте `passwordChange` следующее: 

- `passwordChange` должен сопровождаться `mfa` с помощью `AND` оператора. Это сочетание гарантирует безопасное обновление пароля.
- `passwordChange` должен использоваться в политике, содержащей `userRiskLevels` . Это позволяет пользователям использовать безопасный пароль для сброса рисков пользователей.
- Политика должна быть нацелена `all` на приложения и не исключать их.
- Политика не может содержать другие условия, кроме `users` . `applications` `userRiskLevels`

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
