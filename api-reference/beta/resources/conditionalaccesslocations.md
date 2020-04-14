---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09440c789ae98ae2d5eb46de26f56b32bf0ce578
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413410"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="daa46-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="daa46-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="daa46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daa46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daa46-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="daa46-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="daa46-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="daa46-106">Properties</span></span>

| <span data-ttu-id="daa46-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="daa46-107">Property</span></span>     | <span data-ttu-id="daa46-108">Тип</span><span class="sxs-lookup"><span data-stu-id="daa46-108">Type</span></span>        | <span data-ttu-id="daa46-109">Описание</span><span class="sxs-lookup"><span data-stu-id="daa46-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="daa46-110">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="daa46-110">includeLocations</span></span> | <span data-ttu-id="daa46-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="daa46-111">String collection</span></span> | <span data-ttu-id="daa46-112">Идентификаторы расположений в области применения политики, если `All`явно не `AllTrusted`исключены, или.</span><span class="sxs-lookup"><span data-stu-id="daa46-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="daa46-113">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="daa46-113">excludeLocations</span></span> | <span data-ttu-id="daa46-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="daa46-114">String collection</span></span> | <span data-ttu-id="daa46-115">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="daa46-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="daa46-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daa46-116">JSON representation</span></span>

<span data-ttu-id="daa46-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daa46-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="daa46-118">Связи</span><span class="sxs-lookup"><span data-stu-id="daa46-118">Relationships</span></span>

<span data-ttu-id="daa46-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="daa46-119">None.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->