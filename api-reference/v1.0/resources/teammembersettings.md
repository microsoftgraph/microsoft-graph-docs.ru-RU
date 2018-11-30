---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
ms.openlocfilehash: 74d88e1d87c65745fe98da9b1ee21b26824dc4e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027154"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="0db1a-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="0db1a-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="0db1a-104">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="0db1a-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0db1a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0db1a-105">Properties</span></span>
| <span data-ttu-id="0db1a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0db1a-106">Property</span></span>     | <span data-ttu-id="0db1a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0db1a-107">Type</span></span>   |<span data-ttu-id="0db1a-108">Description</span><span class="sxs-lookup"><span data-stu-id="0db1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0db1a-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="0db1a-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="0db1a-110">Логический</span><span class="sxs-lookup"><span data-stu-id="0db1a-110">Boolean</span></span>|<span data-ttu-id="0db1a-111">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="0db1a-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="0db1a-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="0db1a-112">allowDeleteChannels</span></span>|<span data-ttu-id="0db1a-113">Логический</span><span class="sxs-lookup"><span data-stu-id="0db1a-113">Boolean</span></span>|<span data-ttu-id="0db1a-114">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="0db1a-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="0db1a-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="0db1a-115">allowAddRemoveApps</span></span>|<span data-ttu-id="0db1a-116">Логический</span><span class="sxs-lookup"><span data-stu-id="0db1a-116">Boolean</span></span>|<span data-ttu-id="0db1a-117">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="0db1a-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="0db1a-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="0db1a-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="0db1a-119">Логический</span><span class="sxs-lookup"><span data-stu-id="0db1a-119">Boolean</span></span>|<span data-ttu-id="0db1a-120">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="0db1a-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="0db1a-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="0db1a-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="0db1a-122">Логический</span><span class="sxs-lookup"><span data-stu-id="0db1a-122">Boolean</span></span>|<span data-ttu-id="0db1a-123">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="0db1a-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0db1a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0db1a-124">JSON representation</span></span>

<span data-ttu-id="0db1a-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0db1a-125">The following is a JSON representation of the resource.</span></span>

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
