---
title: тип ресурса justifyAction
description: Указывает, что для указанной операции требуется обоснование.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1db6a91987fd1345ca6a1503dfbd51e3178e9b89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950319"
---
# <a name="justifyaction-resource-type"></a><span data-ttu-id="9224b-103">тип ресурса justifyAction</span><span class="sxs-lookup"><span data-stu-id="9224b-103">justifyAction resource type</span></span>

<span data-ttu-id="9224b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9224b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9224b-105">Указывает, что для указанной операции требуется обоснование.</span><span class="sxs-lookup"><span data-stu-id="9224b-105">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="9224b-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) API may return **justifyAction**.</span><span class="sxs-lookup"><span data-stu-id="9224b-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="9224b-107">Обоснование предоставляется с [помощью метокOptions](../resources/labelingoptions.md).</span><span class="sxs-lookup"><span data-stu-id="9224b-107">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="9224b-108">Предыдущий вызов должен быть повторен, но с свойством **downgradeJustification** **меткиOptions,** за набором с сообщением об оправдании, предоставляемым с помощью пользовательского ввода или логики приложения.</span><span class="sxs-lookup"><span data-stu-id="9224b-108">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="9224b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9224b-109">Properties</span></span>

<span data-ttu-id="9224b-110">Нет</span><span class="sxs-lookup"><span data-stu-id="9224b-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9224b-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9224b-111">JSON representation</span></span>

<span data-ttu-id="9224b-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9224b-112">The following is a JSON representation of the resource.</span></span>

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

