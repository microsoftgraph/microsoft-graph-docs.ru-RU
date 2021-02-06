---
title: Тип ресурса conditionalAccessLocations
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 153d64d32015fcd6119a4d880bbc786905c39b9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132404"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="67132-103">Тип ресурса conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="67132-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="67132-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67132-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67132-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="67132-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="67132-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="67132-106">Properties</span></span>

| <span data-ttu-id="67132-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="67132-107">Property</span></span>     | <span data-ttu-id="67132-108">Тип</span><span class="sxs-lookup"><span data-stu-id="67132-108">Type</span></span>        | <span data-ttu-id="67132-109">Описание</span><span class="sxs-lookup"><span data-stu-id="67132-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="67132-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="67132-110">includeLocations</span></span> | <span data-ttu-id="67132-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="67132-111">String collection</span></span> | <span data-ttu-id="67132-112">ИД расположения в области политики, если явно не исключены, `All` или `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="67132-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="67132-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="67132-113">excludeLocations</span></span> | <span data-ttu-id="67132-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="67132-114">String collection</span></span> | <span data-ttu-id="67132-115">ИД расположения, исключенные из области действия политики.</span><span class="sxs-lookup"><span data-stu-id="67132-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67132-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67132-116">JSON representation</span></span>

<span data-ttu-id="67132-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67132-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="67132-118">Связи</span><span class="sxs-lookup"><span data-stu-id="67132-118">Relationships</span></span>

<span data-ttu-id="67132-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="67132-119">None.</span></span>

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

