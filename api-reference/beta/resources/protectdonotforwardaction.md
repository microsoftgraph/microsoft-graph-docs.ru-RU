---
title: Тип ресурса Протектдонотфорвардактион
description: Информирует приложение о необходимости защиты от пересылки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d9687460a549438db1c9076bef2184b0b1ee5d3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939189"
---
# <a name="protectdonotforwardaction-resource-type"></a>Тип ресурса Протектдонотфорвардактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информирует приложение о необходимости защиты от пересылки. **протектиондонотфорвардактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если результирующая метка настроена для применения [защиты от пересылки](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails). Приложение, использующее приложение, должно использовать клиентскую библиотеку для применения защиты с помощью Azure Information Protection.

## <a name="properties"></a>Свойства

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectDoNotForwardAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectDoNotForwardAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
