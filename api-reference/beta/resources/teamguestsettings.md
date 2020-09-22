---
title: Тип ресурса Теамгуестсеттингс
description: Параметры для настройки того, могут ли гости создавать, изменять или удалять каналы в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 49b50293524b35145cb23d27ab630c64caf2ca43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046661"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="04979-103">Тип ресурса Теамгуестсеттингс</span><span class="sxs-lookup"><span data-stu-id="04979-103">teamGuestSettings resource type</span></span>

<span data-ttu-id="04979-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04979-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04979-105">Параметры для настройки того, могут ли гости создавать, обновлять или удалять каналы в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="04979-105">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04979-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04979-106">Properties</span></span>
| <span data-ttu-id="04979-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="04979-107">Property</span></span>     | <span data-ttu-id="04979-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04979-108">Type</span></span>   |<span data-ttu-id="04979-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04979-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04979-110">алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="04979-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="04979-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="04979-111">Boolean</span></span>|<span data-ttu-id="04979-112">Если задано значение true, гости могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="04979-112">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="04979-113">алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="04979-113">allowDeleteChannels</span></span>|<span data-ttu-id="04979-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="04979-114">Boolean</span></span>|<span data-ttu-id="04979-115">Если задано значение true, гости могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="04979-115">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04979-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04979-116">JSON representation</span></span>

<span data-ttu-id="04979-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04979-117">The following is a JSON representation of the resource.</span></span>

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


