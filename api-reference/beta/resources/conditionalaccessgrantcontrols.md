---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7465ecc3f8e1b99c001fca5d6f43391cf0ef682d
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122506"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Тип ресурса Кондитионалакцессгрантконтролс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | String | Определяет связь элементов управления предоставлением. Возможные значения: `AND` , `OR` . |
| буилтинконтролс | Коллекция String | Список значений встроенных элементов управления, необходимых для политики. Возможные значения: `block` ,,,,, `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` , `passwordChange` . |
| кустомаусентикатионфакторс | Коллекция String | Список идентификаторов настраиваемых элементов управления, необходимых для политики. Дополнительные сведения о настраиваемых элементах управления:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview |
| термсофусе | Коллекция String | Список [условий использования](agreement.md) идентификаторов, необходимых для политики. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Особые рекомендации по использованию `passwordChange` в качестве элемента управления

При использовании `passwordChange` элемента управления учитывайте следующее: 

- `passwordChange`должен сопровождаться `mfa` `AND` оператором. Это сочетание гарантирует, что пароль будет обновлен безопасным способом.
- `passwordChange`должен использоваться в политике, содержащей `userRiskLevels` . Это предназначено для сценариев, в которых пользователям необходимо использовать пароль для безопасного изменения, чтобы сбросить риск для пользователя.
- Политика должна целевить `all` приложения и не исключать какие бы то ни было приложения.
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
