---
title: Тип ресурса conditionalAccessLocations
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 670f07e22b2027c74a79eaca505c624c04c19621
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132116"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="57e76-103">Тип ресурса conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="57e76-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="57e76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57e76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57e76-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="57e76-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="57e76-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="57e76-106">Properties</span></span>

| <span data-ttu-id="57e76-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="57e76-107">Property</span></span>     | <span data-ttu-id="57e76-108">Тип</span><span class="sxs-lookup"><span data-stu-id="57e76-108">Type</span></span>        | <span data-ttu-id="57e76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="57e76-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="57e76-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="57e76-110">includeLocations</span></span> | <span data-ttu-id="57e76-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57e76-111">String collection</span></span> | <span data-ttu-id="57e76-112">ИД расположения в области политики, если явно не исключены, `All` или `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="57e76-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="57e76-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="57e76-113">excludeLocations</span></span> | <span data-ttu-id="57e76-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57e76-114">String collection</span></span> | <span data-ttu-id="57e76-115">ИД расположения, исключенные из области действия политики.</span><span class="sxs-lookup"><span data-stu-id="57e76-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57e76-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57e76-116">JSON representation</span></span>

<span data-ttu-id="57e76-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57e76-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="57e76-118">Связи</span><span class="sxs-lookup"><span data-stu-id="57e76-118">Relationships</span></span>

<span data-ttu-id="57e76-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="57e76-119">None.</span></span>

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

