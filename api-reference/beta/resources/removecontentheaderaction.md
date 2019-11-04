---
title: Тип ресурса Ремовеконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 99f3b77607b34cb68cdef3fa9fc5658ed06b52ec
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938943"
---
# <a name="removecontentheaderaction-resource-type"></a><span data-ttu-id="54a9d-103">Тип ресурса Ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="54a9d-103">removeContentHeaderAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54a9d-104">Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="54a9d-104">Represents an action that specifies the details on the content header to be removed from the information, if applicable.</span></span> <span data-ttu-id="54a9d-105">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтенсеадерактион** , если заголовок будет удален в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="54a9d-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentHeaderAction** if the header is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="54a9d-106">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента.</span><span class="sxs-lookup"><span data-stu-id="54a9d-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span>

## <a name="properties"></a><span data-ttu-id="54a9d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54a9d-107">Properties</span></span>

| <span data-ttu-id="54a9d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54a9d-108">Property</span></span>       | <span data-ttu-id="54a9d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54a9d-109">Type</span></span>              | <span data-ttu-id="54a9d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54a9d-110">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="54a9d-111">уиелементнамес</span><span class="sxs-lookup"><span data-stu-id="54a9d-111">uiElementNames</span></span> | <span data-ttu-id="54a9d-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="54a9d-112">String collection</span></span> | <span data-ttu-id="54a9d-113">Имя элемента пользовательского интерфейса заголовка, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="54a9d-113">The name of the UI element of the header to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54a9d-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54a9d-114">JSON representation</span></span>

<span data-ttu-id="54a9d-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54a9d-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentHeaderAction",
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
  "description": "removeContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->