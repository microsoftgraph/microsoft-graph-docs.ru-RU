---
title: Тип ресурса Ремовеватермаркактион
description: Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b75a001e7673bbeb1513eaac82555d228d712f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023963"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="fdb9c-103">Тип ресурса Ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="fdb9c-103">removeWatermarkAction resource type</span></span>

<span data-ttu-id="fdb9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdb9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdb9c-105">Представляет действие, задающее сведения о подложке контента, которая будет удалена из информации, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="fdb9c-105">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="fdb9c-106">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеватермаркактион** , если водяной знак необходимо удалить в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="fdb9c-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="fdb9c-107">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит Подводя содержимого, который использовался ранее.</span><span class="sxs-lookup"><span data-stu-id="fdb9c-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="fdb9c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdb9c-108">Properties</span></span>

| <span data-ttu-id="fdb9c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdb9c-109">Property</span></span>       | <span data-ttu-id="fdb9c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fdb9c-110">Type</span></span>              | <span data-ttu-id="fdb9c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fdb9c-111">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="fdb9c-112">уиелементнамес</span><span class="sxs-lookup"><span data-stu-id="fdb9c-112">uiElementNames</span></span> | <span data-ttu-id="fdb9c-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fdb9c-113">String collection</span></span> | <span data-ttu-id="fdb9c-114">Имя удаляемого элемента пользовательского интерфейса нижнего колонтитула.</span><span class="sxs-lookup"><span data-stu-id="fdb9c-114">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fdb9c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdb9c-115">JSON representation</span></span>

<span data-ttu-id="fdb9c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdb9c-116">The following is a JSON representation of the resource.</span></span>

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

