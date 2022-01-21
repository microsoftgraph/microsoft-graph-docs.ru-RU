---
title: тип ресурса conditionalAccessSGrantControls
description: Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4148f1b7474c619c1dc614847e0b5772df2397e8
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161636"
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
| customAuthenticationFactors | Коллекция строк | Список пользовательских ID-элементов элементов управления, необходимых политике. Дополнительные информацию о настраиваемом контроле см. в [специальном элементе управления (предварительный просмотр).](/azure/active-directory/conditional-access/controls#custom-controls-preview) |
| termsOfUse | Коллекция строк | Список [условий использования](agreement.md) ID, необходимых политике. |

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


