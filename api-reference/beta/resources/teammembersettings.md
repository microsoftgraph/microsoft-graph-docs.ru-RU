---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
localization_priority: Normal
ms.openlocfilehash: 85f8794ea3564174c75f38228f3891bcd264df2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851382"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="ef63b-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="ef63b-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="ef63b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef63b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef63b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef63b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef63b-106">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="ef63b-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ef63b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef63b-107">Properties</span></span>
| <span data-ttu-id="ef63b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef63b-108">Property</span></span>     | <span data-ttu-id="ef63b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef63b-109">Type</span></span>   |<span data-ttu-id="ef63b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef63b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef63b-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ef63b-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ef63b-112">Логический</span><span class="sxs-lookup"><span data-stu-id="ef63b-112">Boolean</span></span>|<span data-ttu-id="ef63b-113">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="ef63b-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="ef63b-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ef63b-114">allowDeleteChannels</span></span>|<span data-ttu-id="ef63b-115">Логический</span><span class="sxs-lookup"><span data-stu-id="ef63b-115">Boolean</span></span>|<span data-ttu-id="ef63b-116">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="ef63b-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="ef63b-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="ef63b-117">allowAddRemoveApps</span></span>|<span data-ttu-id="ef63b-118">Логический</span><span class="sxs-lookup"><span data-stu-id="ef63b-118">Boolean</span></span>|<span data-ttu-id="ef63b-119">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="ef63b-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="ef63b-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="ef63b-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="ef63b-121">Логический</span><span class="sxs-lookup"><span data-stu-id="ef63b-121">Boolean</span></span>|<span data-ttu-id="ef63b-122">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="ef63b-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="ef63b-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="ef63b-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="ef63b-124">Логический</span><span class="sxs-lookup"><span data-stu-id="ef63b-124">Boolean</span></span>|<span data-ttu-id="ef63b-125">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="ef63b-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef63b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef63b-126">JSON representation</span></span>

<span data-ttu-id="ef63b-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef63b-127">The following is a JSON representation of the resource.</span></span>

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
