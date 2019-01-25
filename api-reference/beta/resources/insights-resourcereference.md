---
title: Тип ресурса resourceReference
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520006"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="93bf4-103">Тип ресурса resourceReference</span><span class="sxs-lookup"><span data-stu-id="93bf4-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93bf4-104">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="93bf4-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="93bf4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93bf4-105">JSON representation</span></span>

<span data-ttu-id="93bf4-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="93bf4-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="93bf4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="93bf4-107">Properties</span></span>

| <span data-ttu-id="93bf4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="93bf4-108">Property</span></span>      | <span data-ttu-id="93bf4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="93bf4-109">Type</span></span>      | <span data-ttu-id="93bf4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93bf4-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="93bf4-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="93bf4-111">webUrl</span></span>        | <span data-ttu-id="93bf4-112">String</span><span class="sxs-lookup"><span data-stu-id="93bf4-112">String</span></span>    | <span data-ttu-id="93bf4-113">URL-адрес, приводя к указанного элемента.</span><span class="sxs-lookup"><span data-stu-id="93bf4-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="93bf4-114">id</span><span class="sxs-lookup"><span data-stu-id="93bf4-114">id</span></span>            | <span data-ttu-id="93bf4-115">String</span><span class="sxs-lookup"><span data-stu-id="93bf4-115">String</span></span>    | <span data-ttu-id="93bf4-116">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="93bf4-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="93bf4-117">type</span><span class="sxs-lookup"><span data-stu-id="93bf4-117">type</span></span>          | <span data-ttu-id="93bf4-118">String</span><span class="sxs-lookup"><span data-stu-id="93bf4-118">String</span></span>    | <span data-ttu-id="93bf4-119">Строковое значение, которое можно использовать для классификации элемента, например, «microsoft.graph.driveItem»</span><span class="sxs-lookup"><span data-stu-id="93bf4-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
