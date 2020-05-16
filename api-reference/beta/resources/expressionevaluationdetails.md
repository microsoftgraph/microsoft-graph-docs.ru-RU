---
title: Тип ресурса Експрессионевалуатиондетаилс
description: Представляет сведения о выражении, сведения о результатах и свойствах.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 347e356bda19228ea8b3738b5bf8b72f57da95f7
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272850"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="4d7d6-103">Тип ресурса Експрессионевалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="4d7d6-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="4d7d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d7d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d7d6-105">Представляет сведения о выражении, сведения о результатах и свойствах.</span><span class="sxs-lookup"><span data-stu-id="4d7d6-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="4d7d6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d7d6-106">Properties</span></span>

| <span data-ttu-id="4d7d6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d7d6-107">Property</span></span>     | <span data-ttu-id="4d7d6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d7d6-108">Type</span></span>        | <span data-ttu-id="4d7d6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d7d6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4d7d6-110">выражение</span><span class="sxs-lookup"><span data-stu-id="4d7d6-110">expression</span></span> | <span data-ttu-id="4d7d6-111">String</span><span class="sxs-lookup"><span data-stu-id="4d7d6-111">String</span></span> | <span data-ttu-id="4d7d6-112">Представляет выражение, которое было оценено.</span><span class="sxs-lookup"><span data-stu-id="4d7d6-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="4d7d6-113">експрессионевалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="4d7d6-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="4d7d6-114">Коллекция Експрессионевалуатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="4d7d6-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="4d7d6-115">Представляет сведения об оценке выражения.</span><span class="sxs-lookup"><span data-stu-id="4d7d6-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="4d7d6-116">експрессионресулт</span><span class="sxs-lookup"><span data-stu-id="4d7d6-116">expressionResult</span></span> | <span data-ttu-id="4d7d6-117">Логический</span><span class="sxs-lookup"><span data-stu-id="4d7d6-117">Boolean</span></span> | <span data-ttu-id="4d7d6-118">Представляет значение результата текущего выражения.</span><span class="sxs-lookup"><span data-stu-id="4d7d6-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="4d7d6-119">пропертитоевалуате</span><span class="sxs-lookup"><span data-stu-id="4d7d6-119">propertyToEvaluate</span></span> | [<span data-ttu-id="4d7d6-120">пропертитоевалуате</span><span class="sxs-lookup"><span data-stu-id="4d7d6-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="4d7d6-121">Определяет имя свойства и значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="4d7d6-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d7d6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d7d6-122">JSON representation</span></span>

<span data-ttu-id="4d7d6-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d7d6-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
