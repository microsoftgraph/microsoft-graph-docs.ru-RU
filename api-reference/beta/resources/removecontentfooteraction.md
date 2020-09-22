---
title: Тип ресурса Ремовеконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, который необходимо удалить из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76450b0d6b0f3a532a4e3472d2ce99ead8c933e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073455"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="8f049-103">Тип ресурса Ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="8f049-103">removeContentFooterAction resource type</span></span>

<span data-ttu-id="8f049-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f049-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f049-105">Представляет действие, задающее сведения о нижнем колонтитуле контента, который необходимо удалить из информации, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="8f049-105">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="8f049-106">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateApplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтентфутерактион** , если нижний колонтитул необходимо удалить в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="8f049-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="8f049-107">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, содержащий ранее соответствующий нижний колонтитул контента.</span><span class="sxs-lookup"><span data-stu-id="8f049-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="8f049-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f049-108">Properties</span></span>

| <span data-ttu-id="8f049-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f049-109">Property</span></span>       | <span data-ttu-id="8f049-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8f049-110">Type</span></span>              | <span data-ttu-id="8f049-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f049-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8f049-112">уиелементнамес</span><span class="sxs-lookup"><span data-stu-id="8f049-112">uiElementNames</span></span> | <span data-ttu-id="8f049-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8f049-113">String collection</span></span> | <span data-ttu-id="8f049-114">Имя элемента пользовательского интерфейса нижнего колонтитула, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="8f049-114">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f049-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f049-115">JSON representation</span></span>

<span data-ttu-id="8f049-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f049-116">The following is a JSON representation of the resource.</span></span>

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

