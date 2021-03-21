---
title: removeWatermarkAction resource type
description: Представляет действие, которое указывает сведения о водяном знаке контента, который должен быть удален из сведений, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2a2365b2c9bc1080db9b6bf58b2035d88832881a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960357"
---
# <a name="removewatermarkaction-resource-type"></a><span data-ttu-id="85619-103">removeWatermarkAction resource type</span><span class="sxs-lookup"><span data-stu-id="85619-103">removeWatermarkAction resource type</span></span>

<span data-ttu-id="85619-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85619-105">Представляет действие, которое указывает сведения о водяном знаке контента, который должен быть удален из сведений, если это применимо.</span><span class="sxs-lookup"><span data-stu-id="85619-105">Represents an action that specifies the details on the content watermark to be removed from the information, if applicable.</span></span> <span data-ttu-id="85619-106">[ОценкаApplication,](../api/informationprotectionlabel-evaluateapplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут возвращать **removeWatermarkAction,** если водяной знак будет удален в результате обновления или удаления метки. [](../api/informationprotectionlabel-evaluateremoval.md)</span><span class="sxs-lookup"><span data-stu-id="85619-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeWatermarkAction** if the watermark is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="85619-107">Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый водяной знак контента.</span><span class="sxs-lookup"><span data-stu-id="85619-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content watermark.</span></span>

## <a name="properties"></a><span data-ttu-id="85619-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85619-108">Properties</span></span>

| <span data-ttu-id="85619-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85619-109">Property</span></span>       | <span data-ttu-id="85619-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85619-110">Type</span></span>              | <span data-ttu-id="85619-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85619-111">Description</span></span>                           |
| :------------- | :---------------- | :------------------------------------ |
| <span data-ttu-id="85619-112">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="85619-112">uiElementNames</span></span> | <span data-ttu-id="85619-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="85619-113">String collection</span></span> | <span data-ttu-id="85619-114">Имя элемента пользовательского интерфейса подножки, который следует удалить.</span><span class="sxs-lookup"><span data-stu-id="85619-114">The name of the UI element of footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85619-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85619-115">JSON representation</span></span>

<span data-ttu-id="85619-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85619-116">The following is a JSON representation of the resource.</span></span>

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

