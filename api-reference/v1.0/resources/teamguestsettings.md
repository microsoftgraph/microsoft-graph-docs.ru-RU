---
title: Тип ресурса Теамгуестсеттингс
description: Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7c5cc116567b0ee2db1b2dd5e28c4749d7c6772c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033868"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="c2996-103">Тип ресурса Теамгуестсеттингс</span><span class="sxs-lookup"><span data-stu-id="c2996-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="c2996-104">Параметры для настройки того, могут ли гости создавать, обновлять или удалять каналы в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="c2996-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c2996-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2996-105">Properties</span></span>
| <span data-ttu-id="c2996-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2996-106">Property</span></span>     | <span data-ttu-id="c2996-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c2996-107">Type</span></span>   |<span data-ttu-id="c2996-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c2996-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2996-109">Алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="c2996-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="c2996-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2996-110">Boolean</span></span>|<span data-ttu-id="c2996-111">Если задано значение true, гости могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="c2996-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="c2996-112">Алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="c2996-112">allowDeleteChannels</span></span>|<span data-ttu-id="c2996-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2996-113">Boolean</span></span>|<span data-ttu-id="c2996-114">Если задано значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="c2996-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2996-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2996-115">JSON representation</span></span>

<span data-ttu-id="c2996-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2996-116">The following is a JSON representation of the resource.</span></span>

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
