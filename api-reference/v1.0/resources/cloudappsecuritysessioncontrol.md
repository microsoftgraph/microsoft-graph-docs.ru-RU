---
title: тип ресурса cloudAppSecuritySessionControl
description: Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c52322928b5ef2e2538031ae8c251bc9c1a4caac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962513"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>тип ресурса cloudAppSecuritySessionControl

Пространство имен: microsoft.graph

Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений. Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено ли управление сеансом. |
|cloudAppSecurityType|cloudAppSecuritySessionControlType| Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`. Дополнительные сведения см. в [приложении Deploy Conditional Access App Control для рекомендуемых приложений.](/cloud-app-security/proxy-deployment-aad) |

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
