---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c1485bbc43588b8144cbe1cc7cb189f9b8c9fdc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863780"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="3ab58-103">Тип ресурса Теаммемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="3ab58-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="3ab58-104">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).</span><span class="sxs-lookup"><span data-stu-id="3ab58-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ab58-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ab58-105">Properties</span></span>
| <span data-ttu-id="3ab58-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ab58-106">Property</span></span>     | <span data-ttu-id="3ab58-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3ab58-107">Type</span></span>   |<span data-ttu-id="3ab58-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ab58-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ab58-109">алловкреатеприватечаннелс</span><span class="sxs-lookup"><span data-stu-id="3ab58-109">allowCreatePrivateChannels</span></span>|<span data-ttu-id="3ab58-110">Логический</span><span class="sxs-lookup"><span data-stu-id="3ab58-110">Boolean</span></span>|<span data-ttu-id="3ab58-111">Если задано значение true, участники могут добавлять и обновлять частные каналы.</span><span class="sxs-lookup"><span data-stu-id="3ab58-111">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="3ab58-112">алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="3ab58-112">allowCreateUpdateChannels</span></span>|<span data-ttu-id="3ab58-113">Логический</span><span class="sxs-lookup"><span data-stu-id="3ab58-113">Boolean</span></span>|<span data-ttu-id="3ab58-114">Если задано значение true, участники могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="3ab58-114">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="3ab58-115">алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="3ab58-115">allowDeleteChannels</span></span>|<span data-ttu-id="3ab58-116">Логический</span><span class="sxs-lookup"><span data-stu-id="3ab58-116">Boolean</span></span>|<span data-ttu-id="3ab58-117">Если задано значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="3ab58-117">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="3ab58-118">алловаддремовеаппс</span><span class="sxs-lookup"><span data-stu-id="3ab58-118">allowAddRemoveApps</span></span>|<span data-ttu-id="3ab58-119">Логический</span><span class="sxs-lookup"><span data-stu-id="3ab58-119">Boolean</span></span>|<span data-ttu-id="3ab58-120">Если задано значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="3ab58-120">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="3ab58-121">алловкреатеупдатеремоветабс</span><span class="sxs-lookup"><span data-stu-id="3ab58-121">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="3ab58-122">Логический</span><span class="sxs-lookup"><span data-stu-id="3ab58-122">Boolean</span></span>|<span data-ttu-id="3ab58-123">Если задано значение true, члены могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="3ab58-123">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="3ab58-124">алловкреатеупдатеремовеконнекторс</span><span class="sxs-lookup"><span data-stu-id="3ab58-124">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="3ab58-125">Логический</span><span class="sxs-lookup"><span data-stu-id="3ab58-125">Boolean</span></span>|<span data-ttu-id="3ab58-126">Если задано значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="3ab58-126">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ab58-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ab58-127">JSON representation</span></span>

<span data-ttu-id="3ab58-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ab58-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreatePrivateChannels": true,
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
