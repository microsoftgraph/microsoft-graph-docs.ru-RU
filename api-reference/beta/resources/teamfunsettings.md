---
title: Тип ресурса teamFunSettings
description: Параметры для настройки использования Giphy, memes и наклейки рабочих групп.
ms.openlocfilehash: e8cf62b88a3afa3e5caf6b9425312d7a26af4d20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075222"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="976d0-103">Тип ресурса teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="976d0-103">teamFunSettings resource type</span></span>

> <span data-ttu-id="976d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="976d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="976d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="976d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="976d0-106">Параметры для настройки использования Giphy, memes и наклейки в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="976d0-106">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="976d0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="976d0-107">Properties</span></span>
| <span data-ttu-id="976d0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="976d0-108">Property</span></span>     | <span data-ttu-id="976d0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="976d0-109">Type</span></span>   |<span data-ttu-id="976d0-110">Description</span><span class="sxs-lookup"><span data-stu-id="976d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="976d0-111">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="976d0-111">allowGiphy</span></span>|<span data-ttu-id="976d0-112">Логический</span><span class="sxs-lookup"><span data-stu-id="976d0-112">Boolean</span></span>|<span data-ttu-id="976d0-113">Если присвоено значение true, позволяет использовать Giphy.</span><span class="sxs-lookup"><span data-stu-id="976d0-113">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="976d0-114">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="976d0-114">giphyContentRating</span></span>|<span data-ttu-id="976d0-115">String (enum)</span><span class="sxs-lookup"><span data-stu-id="976d0-115">String (enum)</span></span>|<span data-ttu-id="976d0-116">Оценка контента Giphy.</span><span class="sxs-lookup"><span data-stu-id="976d0-116">Giphy content rating.</span></span> <span data-ttu-id="976d0-117">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="976d0-117">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="976d0-118">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="976d0-118">allowStickersAndMemes</span></span>|<span data-ttu-id="976d0-119">Логический</span><span class="sxs-lookup"><span data-stu-id="976d0-119">Boolean</span></span>|<span data-ttu-id="976d0-120">Если параметр имеет значение true, позволяет пользователям включают в себя наклейки и memes.</span><span class="sxs-lookup"><span data-stu-id="976d0-120">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="976d0-121">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="976d0-121">allowCustomMemes</span></span>|<span data-ttu-id="976d0-122">Логический</span><span class="sxs-lookup"><span data-stu-id="976d0-122">Boolean</span></span>|<span data-ttu-id="976d0-123">Если задано значение true, предоставляет пользователям возможность включать настраиваемых memes.</span><span class="sxs-lookup"><span data-stu-id="976d0-123">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="976d0-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="976d0-124">JSON representation</span></span>

<span data-ttu-id="976d0-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="976d0-125">The following is a JSON representation of the resource.</span></span>

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
