---
title: тип ресурса teamMemberSettings
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dfa463ce47b9724d18f6f13b53ef46a1cb493f4a
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060455"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="1ef4e-103">тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="1ef4e-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="1ef4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef4e-105">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команде.](team.md)</span><span class="sxs-lookup"><span data-stu-id="1ef4e-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1ef4e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ef4e-106">Properties</span></span>
| <span data-ttu-id="1ef4e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ef4e-107">Property</span></span>     | <span data-ttu-id="1ef4e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1ef4e-108">Type</span></span>   |<span data-ttu-id="1ef4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef4e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ef4e-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="1ef4e-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="1ef4e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef4e-111">Boolean</span></span>|<span data-ttu-id="1ef4e-112">Если установлено, что это так, участники могут добавлять и обновлять любые каналы.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-112">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="1ef4e-113">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="1ef4e-113">allowCreatePrivateChannels</span></span>|<span data-ttu-id="1ef4e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef4e-114">Boolean</span></span>|<span data-ttu-id="1ef4e-115">Если установлено, что это так, участники могут добавлять и обновлять частные каналы.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-115">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="1ef4e-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="1ef4e-116">allowDeleteChannels</span></span>|<span data-ttu-id="1ef4e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef4e-117">Boolean</span></span>|<span data-ttu-id="1ef4e-118">Если установлено, что это так, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="1ef4e-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="1ef4e-119">allowAddRemoveApps</span></span>|<span data-ttu-id="1ef4e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef4e-120">Boolean</span></span>|<span data-ttu-id="1ef4e-121">Если установлено, что это так, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="1ef4e-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="1ef4e-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="1ef4e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef4e-123">Boolean</span></span>|<span data-ttu-id="1ef4e-124">Если установлено true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="1ef4e-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="1ef4e-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="1ef4e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef4e-126">Boolean</span></span>|<span data-ttu-id="1ef4e-127">Если установлено верно, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ef4e-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ef4e-128">JSON representation</span></span>

<span data-ttu-id="1ef4e-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ef4e-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowCreatePrivateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


