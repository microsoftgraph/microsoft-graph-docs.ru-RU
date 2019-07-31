---
title: Тип ресурса Теамгуестсеттингс
description: Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d6e10ccde127e2318ad9c2f3015f5d911574513
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964559"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="93216-103">Тип ресурса Теамгуестсеттингс</span><span class="sxs-lookup"><span data-stu-id="93216-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93216-104">Параметры для настройки того, могут ли гости создавать, обновлять или удалять каналы в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="93216-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="93216-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="93216-105">Properties</span></span>
| <span data-ttu-id="93216-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="93216-106">Property</span></span>     | <span data-ttu-id="93216-107">Тип</span><span class="sxs-lookup"><span data-stu-id="93216-107">Type</span></span>   |<span data-ttu-id="93216-108">Описание</span><span class="sxs-lookup"><span data-stu-id="93216-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93216-109">Алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="93216-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="93216-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="93216-110">Boolean</span></span>|<span data-ttu-id="93216-111">Если задано значение true, гости могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="93216-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="93216-112">Алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="93216-112">allowDeleteChannels</span></span>|<span data-ttu-id="93216-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="93216-113">Boolean</span></span>|<span data-ttu-id="93216-114">Если задано значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="93216-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93216-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93216-115">JSON representation</span></span>

<span data-ttu-id="93216-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93216-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
