---
title: Тип ресурса teamMemberSettings
description: Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, рабочих групп.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522646"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="ee24e-103">Тип ресурса teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="ee24e-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee24e-104">Параметры для настройки ли члены могут выполнять определенные действия, например, создание каналов и добавьте программы-роботы, в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="ee24e-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee24e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee24e-105">Properties</span></span>
| <span data-ttu-id="ee24e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee24e-106">Property</span></span>     | <span data-ttu-id="ee24e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ee24e-107">Type</span></span>   |<span data-ttu-id="ee24e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ee24e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee24e-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ee24e-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ee24e-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="ee24e-110">Boolean</span></span>|<span data-ttu-id="ee24e-111">Если параметр имеет значение true, участники могли добавлять и обновлять каналов.</span><span class="sxs-lookup"><span data-stu-id="ee24e-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="ee24e-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ee24e-112">allowDeleteChannels</span></span>|<span data-ttu-id="ee24e-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="ee24e-113">Boolean</span></span>|<span data-ttu-id="ee24e-114">Если параметр имеет значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="ee24e-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="ee24e-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="ee24e-115">allowAddRemoveApps</span></span>|<span data-ttu-id="ee24e-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="ee24e-116">Boolean</span></span>|<span data-ttu-id="ee24e-117">Если параметр имеет значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="ee24e-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="ee24e-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="ee24e-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="ee24e-119">Логическое</span><span class="sxs-lookup"><span data-stu-id="ee24e-119">Boolean</span></span>|<span data-ttu-id="ee24e-120">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="ee24e-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="ee24e-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="ee24e-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="ee24e-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="ee24e-122">Boolean</span></span>|<span data-ttu-id="ee24e-123">Если параметр имеет значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="ee24e-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee24e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee24e-124">JSON representation</span></span>

<span data-ttu-id="ee24e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee24e-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teammembersettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
