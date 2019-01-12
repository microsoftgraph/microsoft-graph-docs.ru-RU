---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b4c30afb6d0c10e8f011b779cf257a1627ff7b48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949782"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="6363c-103">Тип ресурса teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="6363c-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="6363c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6363c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6363c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6363c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6363c-106">Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="6363c-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6363c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6363c-107">Properties</span></span>
| <span data-ttu-id="6363c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6363c-108">Property</span></span>     | <span data-ttu-id="6363c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6363c-109">Type</span></span>   |<span data-ttu-id="6363c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6363c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6363c-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="6363c-111">allowGiphy</span></span>|<span data-ttu-id="6363c-112">Логический</span><span class="sxs-lookup"><span data-stu-id="6363c-112">Boolean</span></span>|<span data-ttu-id="6363c-113">Если присвоено значение true, позволяет использовать Giphy.</span><span class="sxs-lookup"><span data-stu-id="6363c-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="6363c-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="6363c-114">giphyContentRating</span></span>|<span data-ttu-id="6363c-115">String (enum)</span><span class="sxs-lookup"><span data-stu-id="6363c-115">String (enum)</span></span>|<span data-ttu-id="6363c-116">Оценка контента Giphy.</span><span class="sxs-lookup"><span data-stu-id="6363c-116">Giphy content rating.</span></span> <span data-ttu-id="6363c-117">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="6363c-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="6363c-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="6363c-118">allowStickersAndMemes</span></span>|<span data-ttu-id="6363c-119">Логический</span><span class="sxs-lookup"><span data-stu-id="6363c-119">Boolean</span></span>|<span data-ttu-id="6363c-120">Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.</span><span class="sxs-lookup"><span data-stu-id="6363c-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="6363c-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="6363c-121">allowCustomMemes</span></span>|<span data-ttu-id="6363c-122">Логический</span><span class="sxs-lookup"><span data-stu-id="6363c-122">Boolean</span></span>|<span data-ttu-id="6363c-123">Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.</span><span class="sxs-lookup"><span data-stu-id="6363c-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6363c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6363c-124">JSON representation</span></span>

<span data-ttu-id="6363c-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6363c-125">The following is a JSON representation of the resource.</span></span>

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
