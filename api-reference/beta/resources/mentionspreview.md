---
title: Тип ресурса Ментионспревиев
description: Представляет сведения об упоминании объектов в экземпляре ресурса.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 516560d2a0a8e498c1a0b31a62d8ca4209724767
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342291"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="60f64-103">Тип ресурса Ментионспревиев</span><span class="sxs-lookup"><span data-stu-id="60f64-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60f64-104">Представляет сведения об [упоминании](../resources/mention.md) объектов в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="60f64-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="60f64-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="60f64-105">Properties</span></span>
| <span data-ttu-id="60f64-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="60f64-106">Property</span></span>     | <span data-ttu-id="60f64-107">Тип</span><span class="sxs-lookup"><span data-stu-id="60f64-107">Type</span></span>   |<span data-ttu-id="60f64-108">Описание</span><span class="sxs-lookup"><span data-stu-id="60f64-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60f64-109">Упомянутые</span><span class="sxs-lookup"><span data-stu-id="60f64-109">isMentioned</span></span> | <span data-ttu-id="60f64-110">Логический</span><span class="sxs-lookup"><span data-stu-id="60f64-110">Boolean</span></span> | <span data-ttu-id="60f64-111">Имеет значение true, если пользователь, вошедшего в систему, упоминается в родительском экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="60f64-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="60f64-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60f64-112">Read-only.</span></span> <span data-ttu-id="60f64-113">Поддерживает фильтр.</span><span class="sxs-lookup"><span data-stu-id="60f64-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60f64-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60f64-114">JSON representation</span></span>

<span data-ttu-id="60f64-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60f64-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
