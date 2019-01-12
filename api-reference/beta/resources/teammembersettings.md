---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3854481e89f04fa727b77c6b4f8699c62a16d739
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978251"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="c4839-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="c4839-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="c4839-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4839-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4839-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4839-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4839-106">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="c4839-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c4839-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4839-107">Properties</span></span>
| <span data-ttu-id="c4839-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4839-108">Property</span></span>     | <span data-ttu-id="c4839-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c4839-109">Type</span></span>   |<span data-ttu-id="c4839-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4839-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4839-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="c4839-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="c4839-112">Логический</span><span class="sxs-lookup"><span data-stu-id="c4839-112">Boolean</span></span>|<span data-ttu-id="c4839-113">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="c4839-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="c4839-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="c4839-114">allowDeleteChannels</span></span>|<span data-ttu-id="c4839-115">Логический</span><span class="sxs-lookup"><span data-stu-id="c4839-115">Boolean</span></span>|<span data-ttu-id="c4839-116">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="c4839-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="c4839-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="c4839-117">allowAddRemoveApps</span></span>|<span data-ttu-id="c4839-118">Логический</span><span class="sxs-lookup"><span data-stu-id="c4839-118">Boolean</span></span>|<span data-ttu-id="c4839-119">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="c4839-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="c4839-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="c4839-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="c4839-121">Логический</span><span class="sxs-lookup"><span data-stu-id="c4839-121">Boolean</span></span>|<span data-ttu-id="c4839-122">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="c4839-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="c4839-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="c4839-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="c4839-124">Логический</span><span class="sxs-lookup"><span data-stu-id="c4839-124">Boolean</span></span>|<span data-ttu-id="c4839-125">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="c4839-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4839-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4839-126">JSON representation</span></span>

<span data-ttu-id="c4839-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4839-127">The following is a JSON representation of the resource.</span></span>

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
