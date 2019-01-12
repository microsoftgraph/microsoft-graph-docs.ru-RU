---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987673"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="6aa0b-103">Тип ресурса teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="6aa0b-103">teamFunSettings resource type</span></span>



<span data-ttu-id="6aa0b-104">Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="6aa0b-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6aa0b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6aa0b-105">Properties</span></span>
| <span data-ttu-id="6aa0b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aa0b-106">Property</span></span>     | <span data-ttu-id="6aa0b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6aa0b-107">Type</span></span>   |<span data-ttu-id="6aa0b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6aa0b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6aa0b-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="6aa0b-109">allowGiphy</span></span>|<span data-ttu-id="6aa0b-110">Логический</span><span class="sxs-lookup"><span data-stu-id="6aa0b-110">Boolean</span></span>|<span data-ttu-id="6aa0b-111">Если присвоено значение true, позволяет использовать Giphy.</span><span class="sxs-lookup"><span data-stu-id="6aa0b-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="6aa0b-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="6aa0b-112">giphyContentRating</span></span>|<span data-ttu-id="6aa0b-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="6aa0b-113">String (enum)</span></span>|<span data-ttu-id="6aa0b-114">Оценка контента Giphy.</span><span class="sxs-lookup"><span data-stu-id="6aa0b-114">Giphy content rating.</span></span> <span data-ttu-id="6aa0b-115">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="6aa0b-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="6aa0b-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="6aa0b-116">allowStickersAndMemes</span></span>|<span data-ttu-id="6aa0b-117">Логический</span><span class="sxs-lookup"><span data-stu-id="6aa0b-117">Boolean</span></span>|<span data-ttu-id="6aa0b-118">Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.</span><span class="sxs-lookup"><span data-stu-id="6aa0b-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="6aa0b-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="6aa0b-119">allowCustomMemes</span></span>|<span data-ttu-id="6aa0b-120">Логический</span><span class="sxs-lookup"><span data-stu-id="6aa0b-120">Boolean</span></span>|<span data-ttu-id="6aa0b-121">Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.</span><span class="sxs-lookup"><span data-stu-id="6aa0b-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6aa0b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6aa0b-122">JSON representation</span></span>

<span data-ttu-id="6aa0b-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aa0b-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
