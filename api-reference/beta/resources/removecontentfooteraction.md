---
title: Тип ресурса Ремовеконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, который необходимо удалить из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62bd0fbefeb9bf246619bc470c5552cd20d174d2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939448"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="eb0a5-103">Тип ресурса Ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="eb0a5-103">removeContentFooterAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb0a5-104">Представляет действие, задающее сведения о нижнем колонтитуле контента, который необходимо удалить из информации, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="eb0a5-104">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="eb0a5-105">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateApplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтентфутерактион** , если нижний колонтитул необходимо удалить в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="eb0a5-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="eb0a5-106">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, содержащий ранее соответствующий нижний колонтитул контента.</span><span class="sxs-lookup"><span data-stu-id="eb0a5-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="eb0a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb0a5-107">Properties</span></span>

| <span data-ttu-id="eb0a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb0a5-108">Property</span></span>       | <span data-ttu-id="eb0a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eb0a5-109">Type</span></span>              | <span data-ttu-id="eb0a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb0a5-110">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="eb0a5-111">уиелементнамес</span><span class="sxs-lookup"><span data-stu-id="eb0a5-111">uiElementNames</span></span> | <span data-ttu-id="eb0a5-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eb0a5-112">String collection</span></span> | <span data-ttu-id="eb0a5-113">Имя элемента пользовательского интерфейса нижнего колонтитула, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="eb0a5-113">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb0a5-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb0a5-114">JSON representation</span></span>

<span data-ttu-id="eb0a5-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb0a5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentFooterAction",
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
  "description": "removeContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->