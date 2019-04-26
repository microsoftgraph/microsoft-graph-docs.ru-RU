---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 33f1930096ff63968db39e06ddec26c53ae8bcc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341724"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="4164e-103">Тип ресурса Теаммемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="4164e-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4164e-104">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).</span><span class="sxs-lookup"><span data-stu-id="4164e-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4164e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4164e-105">Properties</span></span>
| <span data-ttu-id="4164e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4164e-106">Property</span></span>     | <span data-ttu-id="4164e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4164e-107">Type</span></span>   |<span data-ttu-id="4164e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4164e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4164e-109">Алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="4164e-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="4164e-110">Логический</span><span class="sxs-lookup"><span data-stu-id="4164e-110">Boolean</span></span>|<span data-ttu-id="4164e-111">Если задано значение true, участники могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="4164e-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="4164e-112">Алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="4164e-112">allowDeleteChannels</span></span>|<span data-ttu-id="4164e-113">Логический</span><span class="sxs-lookup"><span data-stu-id="4164e-113">Boolean</span></span>|<span data-ttu-id="4164e-114">Если задано значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="4164e-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="4164e-115">Алловаддремовеаппс</span><span class="sxs-lookup"><span data-stu-id="4164e-115">allowAddRemoveApps</span></span>|<span data-ttu-id="4164e-116">Логический</span><span class="sxs-lookup"><span data-stu-id="4164e-116">Boolean</span></span>|<span data-ttu-id="4164e-117">Если задано значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="4164e-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="4164e-118">Алловкреатеупдатеремоветабс</span><span class="sxs-lookup"><span data-stu-id="4164e-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="4164e-119">Логический</span><span class="sxs-lookup"><span data-stu-id="4164e-119">Boolean</span></span>|<span data-ttu-id="4164e-120">Если задано значение true, члены могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="4164e-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="4164e-121">Алловкреатеупдатеремовеконнекторс</span><span class="sxs-lookup"><span data-stu-id="4164e-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="4164e-122">Логический</span><span class="sxs-lookup"><span data-stu-id="4164e-122">Boolean</span></span>|<span data-ttu-id="4164e-123">Если задано значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="4164e-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4164e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4164e-124">JSON representation</span></span>

<span data-ttu-id="4164e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4164e-125">The following is a JSON representation of the resource.</span></span>

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
