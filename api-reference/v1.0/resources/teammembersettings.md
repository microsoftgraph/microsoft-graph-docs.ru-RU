---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
localization_priority: Normal
ms.openlocfilehash: 7b63bce5bc298f7d9599d8c6146d7962d319c79f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826070"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="167bd-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="167bd-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="167bd-104">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="167bd-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="167bd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="167bd-105">Properties</span></span>
| <span data-ttu-id="167bd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="167bd-106">Property</span></span>     | <span data-ttu-id="167bd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="167bd-107">Type</span></span>   |<span data-ttu-id="167bd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="167bd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="167bd-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="167bd-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="167bd-110">Логический</span><span class="sxs-lookup"><span data-stu-id="167bd-110">Boolean</span></span>|<span data-ttu-id="167bd-111">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="167bd-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="167bd-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="167bd-112">allowDeleteChannels</span></span>|<span data-ttu-id="167bd-113">Логический</span><span class="sxs-lookup"><span data-stu-id="167bd-113">Boolean</span></span>|<span data-ttu-id="167bd-114">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="167bd-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="167bd-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="167bd-115">allowAddRemoveApps</span></span>|<span data-ttu-id="167bd-116">Логический</span><span class="sxs-lookup"><span data-stu-id="167bd-116">Boolean</span></span>|<span data-ttu-id="167bd-117">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="167bd-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="167bd-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="167bd-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="167bd-119">Логический</span><span class="sxs-lookup"><span data-stu-id="167bd-119">Boolean</span></span>|<span data-ttu-id="167bd-120">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="167bd-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="167bd-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="167bd-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="167bd-122">Логический</span><span class="sxs-lookup"><span data-stu-id="167bd-122">Boolean</span></span>|<span data-ttu-id="167bd-123">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="167bd-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="167bd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="167bd-124">JSON representation</span></span>

<span data-ttu-id="167bd-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="167bd-125">The following is a JSON representation of the resource.</span></span>

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
