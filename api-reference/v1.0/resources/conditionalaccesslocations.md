---
title: Тип ресурса Кондитионалакцесслокатионс
description: Представляет расположения, включенные в область политики и исключенные из нее.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5378764f36bf5fed858755a475fd85a400a2fed
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384678"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="53042-103">Тип ресурса Кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="53042-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="53042-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53042-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53042-105">Представляет расположения, включенные в область политики и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="53042-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="53042-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53042-106">Properties</span></span>

| <span data-ttu-id="53042-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53042-107">Property</span></span>     | <span data-ttu-id="53042-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53042-108">Type</span></span>        | <span data-ttu-id="53042-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53042-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53042-110">инклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="53042-110">includeLocations</span></span> | <span data-ttu-id="53042-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="53042-111">String collection</span></span> | <span data-ttu-id="53042-112">Идентификаторы расположений в области применения политики, если явно не исключены, `All` или `AllTrusted` .</span><span class="sxs-lookup"><span data-stu-id="53042-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="53042-113">ексклуделокатионс</span><span class="sxs-lookup"><span data-stu-id="53042-113">excludeLocations</span></span> | <span data-ttu-id="53042-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="53042-114">String collection</span></span> | <span data-ttu-id="53042-115">Идентификаторы расположений, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="53042-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53042-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53042-116">JSON representation</span></span>

<span data-ttu-id="53042-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53042-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="53042-118">Связи</span><span class="sxs-lookup"><span data-stu-id="53042-118">Relationships</span></span>

<span data-ttu-id="53042-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="53042-119">None.</span></span>

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
