---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515862"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="4c58b-103">Тип ресурса teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="4c58b-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c58b-104">Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="4c58b-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4c58b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c58b-105">Properties</span></span>
| <span data-ttu-id="4c58b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c58b-106">Property</span></span>     | <span data-ttu-id="4c58b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4c58b-107">Type</span></span>   |<span data-ttu-id="4c58b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4c58b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c58b-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="4c58b-109">allowGiphy</span></span>|<span data-ttu-id="4c58b-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="4c58b-110">Boolean</span></span>|<span data-ttu-id="4c58b-111">Если присвоено значение true, позволяет использовать Giphy.</span><span class="sxs-lookup"><span data-stu-id="4c58b-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="4c58b-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="4c58b-112">giphyContentRating</span></span>|<span data-ttu-id="4c58b-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="4c58b-113">String (enum)</span></span>|<span data-ttu-id="4c58b-114">Оценка контента Giphy.</span><span class="sxs-lookup"><span data-stu-id="4c58b-114">Giphy content rating.</span></span> <span data-ttu-id="4c58b-115">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="4c58b-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="4c58b-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="4c58b-116">allowStickersAndMemes</span></span>|<span data-ttu-id="4c58b-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="4c58b-117">Boolean</span></span>|<span data-ttu-id="4c58b-118">Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.</span><span class="sxs-lookup"><span data-stu-id="4c58b-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="4c58b-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="4c58b-119">allowCustomMemes</span></span>|<span data-ttu-id="4c58b-120">Логическое</span><span class="sxs-lookup"><span data-stu-id="4c58b-120">Boolean</span></span>|<span data-ttu-id="4c58b-121">Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.</span><span class="sxs-lookup"><span data-stu-id="4c58b-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c58b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c58b-122">JSON representation</span></span>

<span data-ttu-id="4c58b-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c58b-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
