---
title: Тип ресурса conditionalAccessGrantControls
description: Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6d8717c1ca8fcd9113b8aeacb5a4a1cefce8df8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130475"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Тип ресурса conditionalAccessGrantControls

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | Строка | Определяет отношение элементов управления предоставлением. Возможные значения: `AND` , `OR` . |
| builtInControls | Коллекция объектов string | Список значений встроенных элементов управления, необходимых для политики. Возможные значения: `block` , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` . `passwordChange` |
| customAuthenticationFactors | Коллекция объектов string | Список пользовательских ИД элементов управления, необходимых для политики. Узнайте больше о настраиваемом элементе управления здесь: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview |
| termsOfUse | Коллекция объектов string | Список [условий использования,](agreement.md) необходимых для политики. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Особые соображения при использовании `passwordChange` в качестве управления

При использовании этого управления учитывайте `passwordChange` следующее: 

- `passwordChange` должен сопровождаться `mfa` с помощью `AND` оператора. Это сочетание гарантирует безопасное обновление пароля.
- `passwordChange` должен использоваться в политике, содержащей `userRiskLevels` . Это позволяет пользователям использовать безопасный пароль для сброса рисков пользователей.
- Политика должна быть нацелена `all` на приложения и не исключать их.
- Политика не может содержать другие условия.

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


