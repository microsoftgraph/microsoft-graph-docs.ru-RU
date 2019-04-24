---
title: Тип ресурса Ментионспревиев
description: Представляет сведения об упоминании объектов в экземпляре ресурса.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523487"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="27983-103">Тип ресурса Ментионспревиев</span><span class="sxs-lookup"><span data-stu-id="27983-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27983-104">Представляет сведения об [упоминании](../resources/mention.md) объектов в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="27983-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="27983-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="27983-105">Properties</span></span>
| <span data-ttu-id="27983-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="27983-106">Property</span></span>     | <span data-ttu-id="27983-107">Тип</span><span class="sxs-lookup"><span data-stu-id="27983-107">Type</span></span>   |<span data-ttu-id="27983-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27983-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27983-109">Упомянутые</span><span class="sxs-lookup"><span data-stu-id="27983-109">isMentioned</span></span> | <span data-ttu-id="27983-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="27983-110">Boolean</span></span> | <span data-ttu-id="27983-111">Имеет значение true, если пользователь, вошедшего в систему, упоминается в родительском экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="27983-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="27983-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27983-112">Read-only.</span></span> <span data-ttu-id="27983-113">Поддерживает фильтр.</span><span class="sxs-lookup"><span data-stu-id="27983-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27983-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27983-114">JSON representation</span></span>

<span data-ttu-id="27983-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27983-115">Here is a JSON representation of the resource.</span></span>

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
