---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6ffd1dba4a0aafb1364a6d3f1ee673e2381c7178
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954255"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="55209-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="55209-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="55209-104">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="55209-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="55209-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="55209-105">Properties</span></span>
| <span data-ttu-id="55209-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="55209-106">Property</span></span>     | <span data-ttu-id="55209-107">Тип</span><span class="sxs-lookup"><span data-stu-id="55209-107">Type</span></span>   |<span data-ttu-id="55209-108">Описание</span><span class="sxs-lookup"><span data-stu-id="55209-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55209-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="55209-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="55209-110">Логический</span><span class="sxs-lookup"><span data-stu-id="55209-110">Boolean</span></span>|<span data-ttu-id="55209-111">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="55209-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="55209-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="55209-112">allowDeleteChannels</span></span>|<span data-ttu-id="55209-113">Логический</span><span class="sxs-lookup"><span data-stu-id="55209-113">Boolean</span></span>|<span data-ttu-id="55209-114">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="55209-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="55209-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="55209-115">allowAddRemoveApps</span></span>|<span data-ttu-id="55209-116">Логический</span><span class="sxs-lookup"><span data-stu-id="55209-116">Boolean</span></span>|<span data-ttu-id="55209-117">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="55209-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="55209-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="55209-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="55209-119">Логический</span><span class="sxs-lookup"><span data-stu-id="55209-119">Boolean</span></span>|<span data-ttu-id="55209-120">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="55209-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="55209-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="55209-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="55209-122">Логический</span><span class="sxs-lookup"><span data-stu-id="55209-122">Boolean</span></span>|<span data-ttu-id="55209-123">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="55209-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55209-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55209-124">JSON representation</span></span>

<span data-ttu-id="55209-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55209-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
