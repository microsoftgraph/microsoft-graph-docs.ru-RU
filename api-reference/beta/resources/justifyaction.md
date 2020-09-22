---
title: Тип ресурса Жустифяктион
description: Указывает, что для указанной операции необходимо обоснование.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e26cd675ecb1a3a50c505c019244c60eaee88c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039358"
---
# <a name="justifyaction-resource-type"></a><span data-ttu-id="b22c3-103">Тип ресурса Жустифяктион</span><span class="sxs-lookup"><span data-stu-id="b22c3-103">justifyAction resource type</span></span>

<span data-ttu-id="b22c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b22c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b22c3-105">Указывает, что для указанной операции необходимо обоснование.</span><span class="sxs-lookup"><span data-stu-id="b22c3-105">Indicates that a justification is required for the specified operation.</span></span> <span data-ttu-id="b22c3-106">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateApplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateRemoval.md) могут возвращать **жустифяктион**.</span><span class="sxs-lookup"><span data-stu-id="b22c3-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) APIs may return **justifyAction**.</span></span> <span data-ttu-id="b22c3-107">Обоснование предоставляется с помощью [лабелингоптионс](../resources/labelingoptions.md).</span><span class="sxs-lookup"><span data-stu-id="b22c3-107">Justification is provided via [labelingOptions](../resources/labelingoptions.md).</span></span> <span data-ttu-id="b22c3-108">Предыдущий вызов должен повторяться, но свойство **довнградежустификатион** объекта **лабелингоптионс** Set с сообщением обоснования предоставляется с помощью пользовательского ввода или логики приложения.</span><span class="sxs-lookup"><span data-stu-id="b22c3-108">The previous call should be repeated, but with the **downgradeJustification** property of **labelingOptions** set with a justification message, provided via user input or application logic.</span></span>

## <a name="properties"></a><span data-ttu-id="b22c3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b22c3-109">Properties</span></span>

<span data-ttu-id="b22c3-110">Нет</span><span class="sxs-lookup"><span data-stu-id="b22c3-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b22c3-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b22c3-111">JSON representation</span></span>

<span data-ttu-id="b22c3-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b22c3-112">The following is a JSON representation of the resource.</span></span>

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

