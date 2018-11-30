---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
ms.openlocfilehash: fa673e050ab3362ae7b132f30cfc4caf16d96dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075226"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="b5249-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b5249-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="b5249-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5249-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5249-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5249-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5249-106">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="b5249-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b5249-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5249-107">Properties</span></span>
| <span data-ttu-id="b5249-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5249-108">Property</span></span>     | <span data-ttu-id="b5249-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b5249-109">Type</span></span>   |<span data-ttu-id="b5249-110">Description</span><span class="sxs-lookup"><span data-stu-id="b5249-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5249-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="b5249-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="b5249-112">Логический</span><span class="sxs-lookup"><span data-stu-id="b5249-112">Boolean</span></span>|<span data-ttu-id="b5249-113">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="b5249-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="b5249-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="b5249-114">allowDeleteChannels</span></span>|<span data-ttu-id="b5249-115">Логический</span><span class="sxs-lookup"><span data-stu-id="b5249-115">Boolean</span></span>|<span data-ttu-id="b5249-116">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="b5249-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="b5249-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="b5249-117">allowAddRemoveApps</span></span>|<span data-ttu-id="b5249-118">Логический</span><span class="sxs-lookup"><span data-stu-id="b5249-118">Boolean</span></span>|<span data-ttu-id="b5249-119">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="b5249-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="b5249-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="b5249-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="b5249-121">Логический</span><span class="sxs-lookup"><span data-stu-id="b5249-121">Boolean</span></span>|<span data-ttu-id="b5249-122">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="b5249-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="b5249-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="b5249-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="b5249-124">Логический</span><span class="sxs-lookup"><span data-stu-id="b5249-124">Boolean</span></span>|<span data-ttu-id="b5249-125">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="b5249-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5249-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5249-126">JSON representation</span></span>

<span data-ttu-id="b5249-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5249-127">The following is a JSON representation of the resource.</span></span>

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
