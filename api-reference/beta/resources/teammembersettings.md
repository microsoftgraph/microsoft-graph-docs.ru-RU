---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c7c6690eb293581a60cba20d3f3ef63187339c35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007699"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="50910-103">Тип ресурса Теаммемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="50910-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50910-104">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).</span><span class="sxs-lookup"><span data-stu-id="50910-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="50910-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="50910-105">Properties</span></span>
| <span data-ttu-id="50910-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="50910-106">Property</span></span>     | <span data-ttu-id="50910-107">Тип</span><span class="sxs-lookup"><span data-stu-id="50910-107">Type</span></span>   |<span data-ttu-id="50910-108">Описание</span><span class="sxs-lookup"><span data-stu-id="50910-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50910-109">Алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="50910-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="50910-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="50910-110">Boolean</span></span>|<span data-ttu-id="50910-111">Если задано значение true, участники могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="50910-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="50910-112">Алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="50910-112">allowDeleteChannels</span></span>|<span data-ttu-id="50910-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="50910-113">Boolean</span></span>|<span data-ttu-id="50910-114">Если задано значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="50910-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="50910-115">Алловаддремовеаппс</span><span class="sxs-lookup"><span data-stu-id="50910-115">allowAddRemoveApps</span></span>|<span data-ttu-id="50910-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="50910-116">Boolean</span></span>|<span data-ttu-id="50910-117">Если задано значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="50910-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="50910-118">Алловкреатеупдатеремоветабс</span><span class="sxs-lookup"><span data-stu-id="50910-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="50910-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="50910-119">Boolean</span></span>|<span data-ttu-id="50910-120">Если задано значение true, члены могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="50910-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="50910-121">Алловкреатеупдатеремовеконнекторс</span><span class="sxs-lookup"><span data-stu-id="50910-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="50910-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="50910-122">Boolean</span></span>|<span data-ttu-id="50910-123">Если задано значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="50910-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50910-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50910-124">JSON representation</span></span>

<span data-ttu-id="50910-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50910-125">The following is a JSON representation of the resource.</span></span>

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
