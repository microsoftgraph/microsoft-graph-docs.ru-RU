---
title: Тип ресурса teamMessagingSettings
description: Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: df80fbb828a400e736b2e8c3b73f949fe6bfd1ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878381"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="c1368-103">Тип ресурса teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="c1368-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="c1368-104">Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="c1368-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1368-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1368-105">Properties</span></span>
| <span data-ttu-id="c1368-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1368-106">Property</span></span>     | <span data-ttu-id="c1368-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c1368-107">Type</span></span>   |<span data-ttu-id="c1368-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c1368-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1368-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="c1368-109">allowUserEditMessages</span></span>|<span data-ttu-id="c1368-110">Логический</span><span class="sxs-lookup"><span data-stu-id="c1368-110">Boolean</span></span>|<span data-ttu-id="c1368-111">Если параметр имеет значение true, пользователи могут изменять свои сообщения;</span><span class="sxs-lookup"><span data-stu-id="c1368-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="c1368-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="c1368-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="c1368-113">Логический</span><span class="sxs-lookup"><span data-stu-id="c1368-113">Boolean</span></span>|<span data-ttu-id="c1368-114">Если параметр имеет значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="c1368-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="c1368-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="c1368-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="c1368-116">Логический</span><span class="sxs-lookup"><span data-stu-id="c1368-116">Boolean</span></span>|<span data-ttu-id="c1368-117">Если параметр имеет значение true, владельцы могут удалять все сообщения.</span><span class="sxs-lookup"><span data-stu-id="c1368-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="c1368-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="c1368-118">allowTeamMentions</span></span>|<span data-ttu-id="c1368-119">Логический</span><span class="sxs-lookup"><span data-stu-id="c1368-119">Boolean</span></span>|<span data-ttu-id="c1368-120">Если задано значение true, допускаются упоминания @team.</span><span class="sxs-lookup"><span data-stu-id="c1368-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="c1368-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="c1368-121">allowChannelMentions</span></span>|<span data-ttu-id="c1368-122">Логический</span><span class="sxs-lookup"><span data-stu-id="c1368-122">Boolean</span></span>|<span data-ttu-id="c1368-123">Если задано значение true, допускаются упоминания @channel.</span><span class="sxs-lookup"><span data-stu-id="c1368-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1368-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1368-124">JSON representation</span></span>

<span data-ttu-id="c1368-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1368-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
