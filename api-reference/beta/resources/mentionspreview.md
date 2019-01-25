---
title: Тип ресурса mentionsPreview
description: Представляет сведения об объектах упоминаются в экземпляре ресурсов.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518767"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="ce9cb-103">Тип ресурса mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="ce9cb-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce9cb-104">Представляет сведения о [упомянуть](../resources/mention.md) объекты в экземпляре ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ce9cb-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="ce9cb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce9cb-105">Properties</span></span>
| <span data-ttu-id="ce9cb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce9cb-106">Property</span></span>     | <span data-ttu-id="ce9cb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ce9cb-107">Type</span></span>   |<span data-ttu-id="ce9cb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ce9cb-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce9cb-109">isMentioned</span><span class="sxs-lookup"><span data-stu-id="ce9cb-109">isMentioned</span></span> | <span data-ttu-id="ce9cb-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="ce9cb-110">Boolean</span></span> | <span data-ttu-id="ce9cb-111">Значение true, если пользователь выполнил вход упоминается в экземпляре ресурсов родительского.</span><span class="sxs-lookup"><span data-stu-id="ce9cb-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="ce9cb-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce9cb-112">Read-only.</span></span> <span data-ttu-id="ce9cb-113">Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="ce9cb-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce9cb-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce9cb-114">JSON representation</span></span>

<span data-ttu-id="ce9cb-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce9cb-115">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionspreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
