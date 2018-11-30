---
title: Тип ресурса teamGuestSettings
description: Параметры для настройки ли гости могут создать, обновить или удалить каналы рабочих групп.
ms.openlocfilehash: 3c59c84e0baa9db580a81eeb72a405ec5097c478
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027063"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="7e27f-103">Тип ресурса teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="7e27f-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="7e27f-104">Параметры для настройки ли гости могут создать, обновить или удалить каналы в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="7e27f-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7e27f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e27f-105">Properties</span></span>
| <span data-ttu-id="7e27f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e27f-106">Property</span></span>     | <span data-ttu-id="7e27f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7e27f-107">Type</span></span>   |<span data-ttu-id="7e27f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7e27f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e27f-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="7e27f-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="7e27f-110">Логический</span><span class="sxs-lookup"><span data-stu-id="7e27f-110">Boolean</span></span>|<span data-ttu-id="7e27f-111">Если параметр имеет значение true, Гости можно добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="7e27f-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="7e27f-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="7e27f-112">allowDeleteChannels</span></span>|<span data-ttu-id="7e27f-113">Логический</span><span class="sxs-lookup"><span data-stu-id="7e27f-113">Boolean</span></span>|<span data-ttu-id="7e27f-114">Если параметр имеет значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="7e27f-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e27f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e27f-115">JSON representation</span></span>

<span data-ttu-id="7e27f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e27f-116">The following is a JSON representation of the resource.</span></span>

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
