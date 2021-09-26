---
title: тип ресурса conditionalAccessSGrantControls
description: Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68346c835acb3ad46353fe4a48f6a426861484c8
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763627"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>тип ресурса conditionalAccessSGrantControls

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | Строка | Определяет связь элементов управления грантами. Возможные значения: `AND` , `OR` . |
| builtInControls | коллекция conditionalAccessGrantControl | Список значений встроенных элементов управления, необходимых политике. Возможные значения: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` . |
| customAuthenticationFactors | Коллекция объектов string | Список пользовательских ID-элементов элементов управления, необходимых политике. Дополнительные информацию о настраиваемом контроле см. в [специальном элементе управления (предварительный просмотр).](/azure/active-directory/conditional-access/controls#custom-controls-preview) |
| termsOfUse | Коллекция объектов string | Список [условий использования](agreement.md) ID, необходимых политике. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Особые соображения при использовании `passwordChange` в качестве управления

При использовании управления рассмотрим `passwordChange` следующее: 

- `passwordChange` должны сопровождаться `mfa` с помощью `AND` оператора. Это сочетание гарантирует, что пароль будет обновляться безопасным способом.
- `passwordChange` необходимо использовать в политике, содержащей `userRiskLevels` . Это предназначено для того, чтобы включить сценарии, в которых пользователи должны использовать безопасный пароль изменения для сброса риска пользователя.
- Политика должна быть ориентирована `all` на приложения, а не исключать любые приложения.
- Политика не может содержать любое другое условие.

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


