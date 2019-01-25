---
title: Тип ресурса teamMessagingSettings
description: Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510101"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="5a071-103">Тип ресурса teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="5a071-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a071-104">Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="5a071-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a071-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a071-105">Properties</span></span>
| <span data-ttu-id="5a071-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a071-106">Property</span></span>     | <span data-ttu-id="5a071-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5a071-107">Type</span></span>   |<span data-ttu-id="5a071-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5a071-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a071-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="5a071-109">allowUserEditMessages</span></span>|<span data-ttu-id="5a071-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="5a071-110">Boolean</span></span>|<span data-ttu-id="5a071-111">Если параметр имеет значение true, пользователи могут изменять свои сообщения;</span><span class="sxs-lookup"><span data-stu-id="5a071-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="5a071-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="5a071-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="5a071-113">Логическое</span><span class="sxs-lookup"><span data-stu-id="5a071-113">Boolean</span></span>|<span data-ttu-id="5a071-114">Если параметр имеет значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="5a071-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="5a071-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="5a071-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="5a071-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="5a071-116">Boolean</span></span>|<span data-ttu-id="5a071-117">Если параметр имеет значение true, владельцы могут удалять все сообщения.</span><span class="sxs-lookup"><span data-stu-id="5a071-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="5a071-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="5a071-118">allowTeamMentions</span></span>|<span data-ttu-id="5a071-119">Логическое</span><span class="sxs-lookup"><span data-stu-id="5a071-119">Boolean</span></span>|<span data-ttu-id="5a071-120">Если задано значение true, допускаются упоминания @team.</span><span class="sxs-lookup"><span data-stu-id="5a071-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="5a071-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="5a071-121">allowChannelMentions</span></span>|<span data-ttu-id="5a071-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="5a071-122">Boolean</span></span>|<span data-ttu-id="5a071-123">Если задано значение true, допускаются упоминания @channel.</span><span class="sxs-lookup"><span data-stu-id="5a071-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a071-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a071-124">JSON representation</span></span>

<span data-ttu-id="5a071-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a071-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teammessagingsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
