---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642760"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="3e0c7-103">Тип ресурса resourceReference</span><span class="sxs-lookup"><span data-stu-id="3e0c7-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e0c7-104">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="3e0c7-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e0c7-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e0c7-105">JSON representation</span></span>

<span data-ttu-id="3e0c7-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e0c7-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="3e0c7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e0c7-107">Properties</span></span>

| <span data-ttu-id="3e0c7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e0c7-108">Property</span></span>      | <span data-ttu-id="3e0c7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3e0c7-109">Type</span></span>      | <span data-ttu-id="3e0c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e0c7-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="3e0c7-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="3e0c7-111">webUrl</span></span>        | <span data-ttu-id="3e0c7-112">String</span><span class="sxs-lookup"><span data-stu-id="3e0c7-112">String</span></span>    | <span data-ttu-id="3e0c7-113">URL-адрес, приводя к указанного элемента.</span><span class="sxs-lookup"><span data-stu-id="3e0c7-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="3e0c7-114">id</span><span class="sxs-lookup"><span data-stu-id="3e0c7-114">id</span></span>            | <span data-ttu-id="3e0c7-115">String</span><span class="sxs-lookup"><span data-stu-id="3e0c7-115">String</span></span>    | <span data-ttu-id="3e0c7-116">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="3e0c7-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="3e0c7-117">type</span><span class="sxs-lookup"><span data-stu-id="3e0c7-117">type</span></span>          | <span data-ttu-id="3e0c7-118">String</span><span class="sxs-lookup"><span data-stu-id="3e0c7-118">String</span></span>    | <span data-ttu-id="3e0c7-119">Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem»</span><span class="sxs-lookup"><span data-stu-id="3e0c7-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
