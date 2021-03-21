---
title: removeContentFooterAction resource type
description: Представляет действие, которое указывает сведения на подножке контента, которые будут удалены из сведений, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1e8de130b2ad346e8e1fee2077014eda9e9b94d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962093"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="2b0a6-103">removeContentFooterAction resource type</span><span class="sxs-lookup"><span data-stu-id="2b0a6-103">removeContentFooterAction resource type</span></span>

<span data-ttu-id="2b0a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b0a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b0a6-105">Представляет действие, которое указывает сведения на подножке контента, которые будут удалены из сведений, если это применимо.</span><span class="sxs-lookup"><span data-stu-id="2b0a6-105">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="2b0a6-106">[ОценкаApplication,](../api/informationprotectionlabel-evaluateApplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут возвращать **removeContentFooterAction,** если в результате обновления или удаления метки необходимо удалить подножку. [](../api/informationprotectionlabel-evaluateremoval.md)</span><span class="sxs-lookup"><span data-stu-id="2b0a6-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="2b0a6-107">Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый подножок контента.</span><span class="sxs-lookup"><span data-stu-id="2b0a6-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="2b0a6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b0a6-108">Properties</span></span>

| <span data-ttu-id="2b0a6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b0a6-109">Property</span></span>       | <span data-ttu-id="2b0a6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2b0a6-110">Type</span></span>              | <span data-ttu-id="2b0a6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2b0a6-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="2b0a6-112">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="2b0a6-112">uiElementNames</span></span> | <span data-ttu-id="2b0a6-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2b0a6-113">String collection</span></span> | <span data-ttu-id="2b0a6-114">Имя элемента пользовательского интерфейса необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="2b0a6-114">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b0a6-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b0a6-115">JSON representation</span></span>

<span data-ttu-id="2b0a6-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0a6-116">The following is a JSON representation of the resource.</span></span>

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

