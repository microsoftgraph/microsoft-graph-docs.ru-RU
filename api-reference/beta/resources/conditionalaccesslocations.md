---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a3b6affa1dccdf9065061bec855fb8a2000d387
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507543"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="2bfbe-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="2bfbe-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="2bfbe-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2bfbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bfbe-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="2bfbe-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="2bfbe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bfbe-106">Properties</span></span>

| <span data-ttu-id="2bfbe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bfbe-107">Property</span></span>     | <span data-ttu-id="2bfbe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2bfbe-108">Type</span></span>        | <span data-ttu-id="2bfbe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2bfbe-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2bfbe-110">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="2bfbe-110">includeLocations</span></span> | <span data-ttu-id="2bfbe-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2bfbe-111">String collection</span></span> | <span data-ttu-id="2bfbe-112">Идентификаторы расположений в области применения политики, если `All`явно не `AllTrusted`исключены, или.</span><span class="sxs-lookup"><span data-stu-id="2bfbe-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="2bfbe-113">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="2bfbe-113">excludeLocations</span></span> | <span data-ttu-id="2bfbe-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2bfbe-114">String collection</span></span> | <span data-ttu-id="2bfbe-115">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="2bfbe-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2bfbe-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bfbe-116">JSON representation</span></span>

<span data-ttu-id="2bfbe-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bfbe-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="2bfbe-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2bfbe-118">Relationships</span></span>

<span data-ttu-id="2bfbe-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2bfbe-119">None.</span></span>

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