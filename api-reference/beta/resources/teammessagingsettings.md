---
title: Тип ресурса teamMessagingSettings
description: Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06aca84355a07052dcea316145dfff437eee743b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848260"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="ba305-103">Тип ресурса teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="ba305-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="ba305-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba305-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba305-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba305-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba305-106">Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="ba305-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba305-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba305-107">Properties</span></span>
| <span data-ttu-id="ba305-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba305-108">Property</span></span>     | <span data-ttu-id="ba305-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba305-109">Type</span></span>   |<span data-ttu-id="ba305-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba305-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba305-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="ba305-111">allowUserEditMessages</span></span>|<span data-ttu-id="ba305-112">Логический</span><span class="sxs-lookup"><span data-stu-id="ba305-112">Boolean</span></span>|<span data-ttu-id="ba305-113">Если параметр имеет значение true, пользователи могут изменять свои сообщения;</span><span class="sxs-lookup"><span data-stu-id="ba305-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="ba305-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="ba305-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="ba305-115">Логический</span><span class="sxs-lookup"><span data-stu-id="ba305-115">Boolean</span></span>|<span data-ttu-id="ba305-116">Если параметр имеет значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="ba305-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="ba305-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="ba305-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="ba305-118">Логический</span><span class="sxs-lookup"><span data-stu-id="ba305-118">Boolean</span></span>|<span data-ttu-id="ba305-119">Если параметр имеет значение true, владельцы могут удалять все сообщения.</span><span class="sxs-lookup"><span data-stu-id="ba305-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="ba305-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="ba305-120">allowTeamMentions</span></span>|<span data-ttu-id="ba305-121">Логический</span><span class="sxs-lookup"><span data-stu-id="ba305-121">Boolean</span></span>|<span data-ttu-id="ba305-122">Если задано значение true, допускаются упоминания @team.</span><span class="sxs-lookup"><span data-stu-id="ba305-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="ba305-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="ba305-123">allowChannelMentions</span></span>|<span data-ttu-id="ba305-124">Логический</span><span class="sxs-lookup"><span data-stu-id="ba305-124">Boolean</span></span>|<span data-ttu-id="ba305-125">Если задано значение true, допускаются упоминания @channel.</span><span class="sxs-lookup"><span data-stu-id="ba305-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba305-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba305-126">JSON representation</span></span>

<span data-ttu-id="ba305-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba305-127">The following is a JSON representation of the resource.</span></span>

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
