---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
localization_priority: Normal
ms.openlocfilehash: 3257e54744ef14a94a0570ae45afd271c1514bb0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825601"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="68903-103">Тип ресурса teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="68903-103">teamFunSettings resource type</span></span>



<span data-ttu-id="68903-104">Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="68903-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="68903-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="68903-105">Properties</span></span>
| <span data-ttu-id="68903-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="68903-106">Property</span></span>     | <span data-ttu-id="68903-107">Тип</span><span class="sxs-lookup"><span data-stu-id="68903-107">Type</span></span>   |<span data-ttu-id="68903-108">Описание</span><span class="sxs-lookup"><span data-stu-id="68903-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68903-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="68903-109">allowGiphy</span></span>|<span data-ttu-id="68903-110">Логический</span><span class="sxs-lookup"><span data-stu-id="68903-110">Boolean</span></span>|<span data-ttu-id="68903-111">Если присвоено значение true, позволяет использовать Giphy.</span><span class="sxs-lookup"><span data-stu-id="68903-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="68903-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="68903-112">giphyContentRating</span></span>|<span data-ttu-id="68903-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="68903-113">String (enum)</span></span>|<span data-ttu-id="68903-114">Оценка контента Giphy.</span><span class="sxs-lookup"><span data-stu-id="68903-114">Giphy content rating.</span></span> <span data-ttu-id="68903-115">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="68903-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="68903-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="68903-116">allowStickersAndMemes</span></span>|<span data-ttu-id="68903-117">Логический</span><span class="sxs-lookup"><span data-stu-id="68903-117">Boolean</span></span>|<span data-ttu-id="68903-118">Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.</span><span class="sxs-lookup"><span data-stu-id="68903-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="68903-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="68903-119">allowCustomMemes</span></span>|<span data-ttu-id="68903-120">Логический</span><span class="sxs-lookup"><span data-stu-id="68903-120">Boolean</span></span>|<span data-ttu-id="68903-121">Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.</span><span class="sxs-lookup"><span data-stu-id="68903-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68903-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68903-122">JSON representation</span></span>

<span data-ttu-id="68903-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68903-123">The following is a JSON representation of the resource.</span></span>

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
