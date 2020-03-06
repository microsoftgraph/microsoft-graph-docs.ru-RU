---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d75ae8d97d3d2c95cc1779e38346efeea3026f23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533531"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="656d0-103">Тип ресурса Теаммемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="656d0-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="656d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="656d0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="656d0-105">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).</span><span class="sxs-lookup"><span data-stu-id="656d0-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="656d0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="656d0-106">Properties</span></span>
| <span data-ttu-id="656d0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="656d0-107">Property</span></span>     | <span data-ttu-id="656d0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="656d0-108">Type</span></span>   |<span data-ttu-id="656d0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="656d0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="656d0-110">алловкреатеприватечаннелс</span><span class="sxs-lookup"><span data-stu-id="656d0-110">allowCreatePrivateChannels</span></span>|<span data-ttu-id="656d0-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="656d0-111">Boolean</span></span>|<span data-ttu-id="656d0-112">Если задано значение true, участники могут добавлять и обновлять частные каналы.</span><span class="sxs-lookup"><span data-stu-id="656d0-112">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="656d0-113">алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="656d0-113">allowCreateUpdateChannels</span></span>|<span data-ttu-id="656d0-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="656d0-114">Boolean</span></span>|<span data-ttu-id="656d0-115">Если задано значение true, участники могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="656d0-115">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="656d0-116">алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="656d0-116">allowDeleteChannels</span></span>|<span data-ttu-id="656d0-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="656d0-117">Boolean</span></span>|<span data-ttu-id="656d0-118">Если задано значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="656d0-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="656d0-119">алловаддремовеаппс</span><span class="sxs-lookup"><span data-stu-id="656d0-119">allowAddRemoveApps</span></span>|<span data-ttu-id="656d0-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="656d0-120">Boolean</span></span>|<span data-ttu-id="656d0-121">Если задано значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="656d0-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="656d0-122">алловкреатеупдатеремоветабс</span><span class="sxs-lookup"><span data-stu-id="656d0-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="656d0-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="656d0-123">Boolean</span></span>|<span data-ttu-id="656d0-124">Если задано значение true, члены могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="656d0-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="656d0-125">алловкреатеупдатеремовеконнекторс</span><span class="sxs-lookup"><span data-stu-id="656d0-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="656d0-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="656d0-126">Boolean</span></span>|<span data-ttu-id="656d0-127">Если задано значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="656d0-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="656d0-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="656d0-128">JSON representation</span></span>

<span data-ttu-id="656d0-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="656d0-129">The following is a JSON representation of the resource.</span></span>

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
