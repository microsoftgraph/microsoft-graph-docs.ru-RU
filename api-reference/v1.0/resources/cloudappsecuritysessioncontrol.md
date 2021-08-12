---
title: тип ресурса cloudAppSecuritySessionControl
description: Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7ba9d84a10ac25275abffd6c922286c010f02a042c5377f3f43b9f26e55be71a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243618"
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
