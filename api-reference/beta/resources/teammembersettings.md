---
title: Тип ресурса Теаммемберсеттингс
description: Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять ботов в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558050"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="29f26-103">Тип ресурса Теаммемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="29f26-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f26-104">Параметры для настройки того, могут ли участники выполнять определенные действия, например создавать каналы и добавлять боты в [команду](team.md).</span><span class="sxs-lookup"><span data-stu-id="29f26-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="29f26-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="29f26-105">Properties</span></span>
| <span data-ttu-id="29f26-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="29f26-106">Property</span></span>     | <span data-ttu-id="29f26-107">Тип</span><span class="sxs-lookup"><span data-stu-id="29f26-107">Type</span></span>   |<span data-ttu-id="29f26-108">Описание</span><span class="sxs-lookup"><span data-stu-id="29f26-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f26-109">Алловкреатеупдатечаннелс</span><span class="sxs-lookup"><span data-stu-id="29f26-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="29f26-110">Логический</span><span class="sxs-lookup"><span data-stu-id="29f26-110">Boolean</span></span>|<span data-ttu-id="29f26-111">Если задано значение true, участники могут добавлять и обновлять каналы.</span><span class="sxs-lookup"><span data-stu-id="29f26-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="29f26-112">Алловделетечаннелс</span><span class="sxs-lookup"><span data-stu-id="29f26-112">allowDeleteChannels</span></span>|<span data-ttu-id="29f26-113">Логический</span><span class="sxs-lookup"><span data-stu-id="29f26-113">Boolean</span></span>|<span data-ttu-id="29f26-114">Если задано значение true, участники могут удалять каналы.</span><span class="sxs-lookup"><span data-stu-id="29f26-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="29f26-115">Алловаддремовеаппс</span><span class="sxs-lookup"><span data-stu-id="29f26-115">allowAddRemoveApps</span></span>|<span data-ttu-id="29f26-116">Логический</span><span class="sxs-lookup"><span data-stu-id="29f26-116">Boolean</span></span>|<span data-ttu-id="29f26-117">Если задано значение true, участники могут добавлять и удалять приложения.</span><span class="sxs-lookup"><span data-stu-id="29f26-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="29f26-118">Алловкреатеупдатеремоветабс</span><span class="sxs-lookup"><span data-stu-id="29f26-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="29f26-119">Логический</span><span class="sxs-lookup"><span data-stu-id="29f26-119">Boolean</span></span>|<span data-ttu-id="29f26-120">Если задано значение true, члены могут добавлять, обновлять и удалять вкладки.</span><span class="sxs-lookup"><span data-stu-id="29f26-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="29f26-121">Алловкреатеупдатеремовеконнекторс</span><span class="sxs-lookup"><span data-stu-id="29f26-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="29f26-122">Логический</span><span class="sxs-lookup"><span data-stu-id="29f26-122">Boolean</span></span>|<span data-ttu-id="29f26-123">Если задано значение true, участники могут добавлять, обновлять и удалять соединители.</span><span class="sxs-lookup"><span data-stu-id="29f26-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f26-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29f26-124">JSON representation</span></span>

<span data-ttu-id="29f26-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29f26-125">The following is a JSON representation of the resource.</span></span>

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
