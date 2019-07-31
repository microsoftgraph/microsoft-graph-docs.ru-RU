---
title: Тип ресурса Ментионспревиев
description: Представляет сведения об упоминании объектов в экземпляре ресурса.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5c4604657e18498a85aa8646b5d69db7d74299bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009708"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="ad6d1-103">Тип ресурса Ментионспревиев</span><span class="sxs-lookup"><span data-stu-id="ad6d1-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad6d1-104">Представляет сведения об [упоминании](../resources/mention.md) объектов в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad6d1-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="ad6d1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad6d1-105">Properties</span></span>
| <span data-ttu-id="ad6d1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad6d1-106">Property</span></span>     | <span data-ttu-id="ad6d1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ad6d1-107">Type</span></span>   |<span data-ttu-id="ad6d1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ad6d1-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad6d1-109">Упомянутые</span><span class="sxs-lookup"><span data-stu-id="ad6d1-109">isMentioned</span></span> | <span data-ttu-id="ad6d1-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad6d1-110">Boolean</span></span> | <span data-ttu-id="ad6d1-111">Имеет значение true, если пользователь, вошедшего в систему, упоминается в родительском экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad6d1-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="ad6d1-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad6d1-112">Read-only.</span></span> <span data-ttu-id="ad6d1-113">Поддерживает фильтр.</span><span class="sxs-lookup"><span data-stu-id="ad6d1-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad6d1-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad6d1-114">JSON representation</span></span>

<span data-ttu-id="ad6d1-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad6d1-115">Here is a JSON representation of the resource.</span></span>

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
