---
title: тип ресурсов protectDoNotForwardAction
description: Информирует приложение о применении защиты Do Not Forward.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a68771ea278ba8a904c032a86732b2b190eeeb43
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941773"
---
# <a name="protectdonotforwardaction-resource-type"></a>тип ресурсов protectDoNotForwardAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информирует приложение о применении защиты Do Not Forward. **protectionDoNotForwardAction** может быть возвращена с помощью [оценкиApplication](../api/informationprotectionlabel-evaluateapplication.md) или [evaluateClassificationResults,](../api/informationprotectionlabel-evaluateclassificationresults.md) если результированная метка настроена для применения защиты [Do Not Forward.](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails) Потребляемому приложению необходимо использовать клиентскую библиотеку для применения защиты с помощью Azure Information Protection.

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