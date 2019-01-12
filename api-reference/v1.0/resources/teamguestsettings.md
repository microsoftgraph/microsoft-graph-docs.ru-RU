---
title: Тип ресурса teamGuestSettings
description: Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924372"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="643e5-103">Тип ресурса teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="643e5-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="643e5-104">Параметры для настройки ли гости могут создать, обновить или удалить каналы в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="643e5-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="643e5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="643e5-105">Properties</span></span>
| <span data-ttu-id="643e5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="643e5-106">Property</span></span>     | <span data-ttu-id="643e5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="643e5-107">Type</span></span>   |<span data-ttu-id="643e5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="643e5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="643e5-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="643e5-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="643e5-110">Логический</span><span class="sxs-lookup"><span data-stu-id="643e5-110">Boolean</span></span>|<span data-ttu-id="643e5-111">Если параметр имеет значение true, Гости можно добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="643e5-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="643e5-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="643e5-112">allowDeleteChannels</span></span>|<span data-ttu-id="643e5-113">Логический</span><span class="sxs-lookup"><span data-stu-id="643e5-113">Boolean</span></span>|<span data-ttu-id="643e5-114">Если параметр имеет значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="643e5-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="643e5-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="643e5-115">JSON representation</span></span>

<span data-ttu-id="643e5-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="643e5-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
