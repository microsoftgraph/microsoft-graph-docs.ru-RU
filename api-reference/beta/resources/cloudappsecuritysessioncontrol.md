---
title: тип ресурса cloudAppSecuritySessionControl
description: Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 689b065a6156f009d2425a294aaec8e49c4bee93
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60488614"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>тип ресурса cloudAppSecuritySessionControl

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений. Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено ли управление сеансом. |
|cloudAppSecurityType|cloudAppSecuritySessionControlType| Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`. Чтобы узнать больше об этих значениях, разверни управление приложениями условного доступа [для рекомендуемых приложений.](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1--configure-your-idp-to-work-with-cloud-app-security) |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

