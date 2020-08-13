---
title: Тип ресурса Ремовеконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 907113e20b5e4257a672190433efd055a628c17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521154"
---
# <a name="removecontentheaderaction-resource-type"></a><span data-ttu-id="fe80d-103">Тип ресурса Ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="fe80d-103">removeContentHeaderAction resource type</span></span>

<span data-ttu-id="fe80d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe80d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe80d-105">Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="fe80d-105">Represents an action that specifies the details on the content header to be removed from the information, if applicable.</span></span> <span data-ttu-id="fe80d-106">API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтенсеадерактион** , если заголовок будет удален в результате обновления или удаления метки.</span><span class="sxs-lookup"><span data-stu-id="fe80d-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentHeaderAction** if the header is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="fe80d-107">Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента.</span><span class="sxs-lookup"><span data-stu-id="fe80d-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span>

## <a name="properties"></a><span data-ttu-id="fe80d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe80d-108">Properties</span></span>

| <span data-ttu-id="fe80d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe80d-109">Property</span></span>       | <span data-ttu-id="fe80d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fe80d-110">Type</span></span>              | <span data-ttu-id="fe80d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe80d-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="fe80d-112">уиелементнамес</span><span class="sxs-lookup"><span data-stu-id="fe80d-112">uiElementNames</span></span> | <span data-ttu-id="fe80d-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe80d-113">String collection</span></span> | <span data-ttu-id="fe80d-114">Имя элемента пользовательского интерфейса заголовка, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="fe80d-114">The name of the UI element of the header to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe80d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe80d-115">JSON representation</span></span>

<span data-ttu-id="fe80d-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe80d-116">The following is a JSON representation of the resource.</span></span>

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