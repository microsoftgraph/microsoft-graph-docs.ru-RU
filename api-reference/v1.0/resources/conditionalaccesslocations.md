---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b4cdf4fbd1b81d4a4376983a424c2579376a76d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018902"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="c7408-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="c7408-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="c7408-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7408-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7408-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="c7408-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="c7408-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7408-106">Properties</span></span>

| <span data-ttu-id="c7408-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7408-107">Property</span></span>     | <span data-ttu-id="c7408-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c7408-108">Type</span></span>        | <span data-ttu-id="c7408-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c7408-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c7408-110">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="c7408-110">includeLocations</span></span> | <span data-ttu-id="c7408-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c7408-111">String collection</span></span> | <span data-ttu-id="c7408-112">Идентификаторы расположений в области применения политики, если явно не исключены, `All` или `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="c7408-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="c7408-113">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="c7408-113">excludeLocations</span></span> | <span data-ttu-id="c7408-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c7408-114">String collection</span></span> | <span data-ttu-id="c7408-115">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="c7408-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7408-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7408-116">JSON representation</span></span>

<span data-ttu-id="c7408-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7408-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="c7408-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c7408-118">Relationships</span></span>

<span data-ttu-id="c7408-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c7408-119">None.</span></span>

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

