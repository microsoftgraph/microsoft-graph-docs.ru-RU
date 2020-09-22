---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7087457ac68c98b40b1c89dc4b99b13ae85d46b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094010"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="cebeb-103">Тип ресурса Теаммемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="cebeb-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="cebeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebeb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="cebeb-105">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).</span><span class="sxs-lookup"><span data-stu-id="cebeb-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cebeb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cebeb-106">Properties</span></span>
| <span data-ttu-id="cebeb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cebeb-107">Property</span></span>     | <span data-ttu-id="cebeb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cebeb-108">Type</span></span>   |<span data-ttu-id="cebeb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cebeb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cebeb-110">алловкреатеприватечаннелс</span><span class="sxs-lookup"><span data-stu-id="cebeb-110">allowCreatePrivateChannels</span></span>|<span data-ttu-id="cebeb-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebeb-111">Boolean</span></span>|<span data-ttu-id="cebeb-112">Если задано значение true, участники могут добавлять и обновлять частные каналы.</span><span class="sxs-lookup"><span data-stu-id="cebeb-112">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="cebeb-113">алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="cebeb-113">allowCreateUpdateChannels</span></span>|<span data-ttu-id="cebeb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebeb-114">Boolean</span></span>|<span data-ttu-id="cebeb-115">Если задано значение true, участники могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="cebeb-115">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="cebeb-116">алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="cebeb-116">allowDeleteChannels</span></span>|<span data-ttu-id="cebeb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebeb-117">Boolean</span></span>|<span data-ttu-id="cebeb-118">Если задано значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="cebeb-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="cebeb-119">алловаддремовеаппс</span><span class="sxs-lookup"><span data-stu-id="cebeb-119">allowAddRemoveApps</span></span>|<span data-ttu-id="cebeb-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebeb-120">Boolean</span></span>|<span data-ttu-id="cebeb-121">Если задано значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="cebeb-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="cebeb-122">алловкреатеупдатеремоветабс</span><span class="sxs-lookup"><span data-stu-id="cebeb-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="cebeb-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebeb-123">Boolean</span></span>|<span data-ttu-id="cebeb-124">Если задано значение true, члены могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="cebeb-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="cebeb-125">алловкреатеупдатеремовеконнекторс</span><span class="sxs-lookup"><span data-stu-id="cebeb-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="cebeb-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebeb-126">Boolean</span></span>|<span data-ttu-id="cebeb-127">Если задано значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="cebeb-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cebeb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cebeb-128">JSON representation</span></span>

<span data-ttu-id="cebeb-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cebeb-129">The following is a JSON representation of the resource.</span></span>

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

