---
title: тип ресурса conditionalAccessSGrantControls
description: Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6bd2c8dbcd6a57b9f97d810e5691cb2c705c67d2cf322a7b3d26369aa57489dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223636"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>тип ресурса conditionalAccessSGrantControls

Пространство имен: microsoft.graph

Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | String | Определяет связь элементов управления грантами. Возможные значения: `AND` , `OR` . |
| builtInControls | коллекция conditionalAccessGrantControl | Список значений встроенных элементов управления, необходимых политике. Возможные значения: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` . |
| customAuthenticationFactors | Коллекция строк | Список пользовательских ID-элементов элементов управления, необходимых политике. Дополнительные сведения см. в [специальном элементе управления.](/azure/active-directory/conditional-access/controls) |
| termsOfUse | Коллекция String | Список [условий использования](/graph/api/resources/agreement) ID, необходимых политике. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Особые соображения при использовании `passwordChange` в качестве управления

При использовании управления рассмотрим `passwordChange` следующее: 

- `passwordChange` должны сопровождаться `mfa` с помощью `AND` оператора. Это сочетание гарантирует, что пароль будет обновляться безопасным способом.
- `passwordChange` необходимо использовать в политике, содержащей `userRiskLevels` . Это предназначено для того, чтобы включить сценарии, в которых пользователи должны использовать безопасный пароль изменения для сброса риска пользователя.
- Политика должна быть ориентирована `all` на приложения, а не исключать любые приложения.
- Политика не может содержать любое другое условие, кроме `users` `applications` , и `userRiskLevels` .

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
