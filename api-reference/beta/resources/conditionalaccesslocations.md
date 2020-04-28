---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a92d99d7a9e80084b8ec1ce385ce76d1f522b359
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916790"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="c2400-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="c2400-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="c2400-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2400-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2400-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="c2400-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="c2400-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2400-106">Properties</span></span>

| <span data-ttu-id="c2400-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2400-107">Property</span></span>     | <span data-ttu-id="c2400-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c2400-108">Type</span></span>        | <span data-ttu-id="c2400-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c2400-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c2400-110">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="c2400-110">includeLocations</span></span> | <span data-ttu-id="c2400-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c2400-111">String collection</span></span> | <span data-ttu-id="c2400-112">Идентификаторы расположений в области применения политики, если `All`явно не `AllTrusted`исключены, или.</span><span class="sxs-lookup"><span data-stu-id="c2400-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="c2400-113">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="c2400-113">excludeLocations</span></span> | <span data-ttu-id="c2400-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c2400-114">String collection</span></span> | <span data-ttu-id="c2400-115">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="c2400-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2400-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2400-116">JSON representation</span></span>

<span data-ttu-id="c2400-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2400-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="c2400-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c2400-118">Relationships</span></span>

<span data-ttu-id="c2400-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c2400-119">None.</span></span>

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