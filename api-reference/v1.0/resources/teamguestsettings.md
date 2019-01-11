---
title: Тип ресурса teamGuestSettings
description: Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.
localization_priority: Normal
ms.openlocfilehash: f0947101fc8de83d1a56ffa922d9b1e2d79d520f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844879"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="1857d-103">Тип ресурса teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="1857d-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="1857d-104">Параметры для настройки ли гости могут создать, обновить или удалить каналы в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="1857d-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1857d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1857d-105">Properties</span></span>
| <span data-ttu-id="1857d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1857d-106">Property</span></span>     | <span data-ttu-id="1857d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1857d-107">Type</span></span>   |<span data-ttu-id="1857d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1857d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1857d-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="1857d-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="1857d-110">Логический</span><span class="sxs-lookup"><span data-stu-id="1857d-110">Boolean</span></span>|<span data-ttu-id="1857d-111">Если параметр имеет значение true, Гости можно добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="1857d-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="1857d-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="1857d-112">allowDeleteChannels</span></span>|<span data-ttu-id="1857d-113">Логический</span><span class="sxs-lookup"><span data-stu-id="1857d-113">Boolean</span></span>|<span data-ttu-id="1857d-114">Если параметр имеет значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="1857d-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1857d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1857d-115">JSON representation</span></span>

<span data-ttu-id="1857d-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1857d-116">The following is a JSON representation of the resource.</span></span>

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
