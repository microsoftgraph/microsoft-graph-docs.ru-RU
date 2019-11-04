---
title: Тип ресурса Жустифяктион
description: Указывает, что для указанной операции необходимо обоснование.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bc96062febc15310de6a3b2ed04f96a8cf1e69e5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939315"
---
# <a name="justifyaction-resource-type"></a><span data-ttu-id="3bd0b-103">Тип ресурса Жустифяктион</span><span class="sxs-lookup"><span data-stu-id="3bd0b-103">justifyAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bd0b-104">Указывает, что для указанной операции необходимо обоснование.</span><span class="sxs-lookup"><span data-stu-id="3bd0b-104">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="3bd0b-105">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateApplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateRemoval.md) могут возвращать **жустифяктион**.</span><span class="sxs-lookup"><span data-stu-id="3bd0b-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="3bd0b-106">Обоснование предоставляется с помощью [лабелингоптионс](../resources/labelingoptions.md).</span><span class="sxs-lookup"><span data-stu-id="3bd0b-106">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="3bd0b-107">Предыдущий вызов должен повторяться, но свойство **довнградежустификатион** объекта **лабелингоптионс** Set с сообщением обоснования предоставляется с помощью пользовательского ввода или логики приложения.</span><span class="sxs-lookup"><span data-stu-id="3bd0b-107">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="3bd0b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3bd0b-108">Properties</span></span>

<span data-ttu-id="3bd0b-109">Нет</span><span class="sxs-lookup"><span data-stu-id="3bd0b-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bd0b-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3bd0b-110">JSON representation</span></span>

<span data-ttu-id="3bd0b-111">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bd0b-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.justifyAction",
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
  "description": "justifyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->