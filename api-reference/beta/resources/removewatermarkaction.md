---
title: Тип ресурса Ремовеватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34859dedd5e5e740aa776cdf78bb742399523fa2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939273"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="6c196-103">Тип ресурса Ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="6c196-103">removeWatermarkAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c196-104">Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="6c196-104">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="6c196-105">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеватермаркактион** , если водяной знак необходимо удалить в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="6c196-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="6c196-106">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит Подводя содержимого, который использовался ранее.</span><span class="sxs-lookup"><span data-stu-id="6c196-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="6c196-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c196-107">Properties</span></span>

| <span data-ttu-id="6c196-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c196-108">Property</span></span>       | <span data-ttu-id="6c196-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6c196-109">Type</span></span>              | <span data-ttu-id="6c196-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6c196-110">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="6c196-111">уиелементнамес</span><span class="sxs-lookup"><span data-stu-id="6c196-111">uiElementNames</span></span> | <span data-ttu-id="6c196-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6c196-112">String collection</span></span> | <span data-ttu-id="6c196-113">Имя удаляемого элемента пользовательского интерфейса нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="6c196-113">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c196-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c196-114">JSON representation</span></span>

<span data-ttu-id="6c196-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c196-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeWatermarkAction resource",
  "keywords": "",  
  "section": "documentation",
  "tocPath": ""
}-->