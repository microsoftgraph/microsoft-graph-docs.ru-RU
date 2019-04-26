---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48d9281a032bebd9d65936cbf9effd78416ffc7d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341471"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="13bd5-103">Тип ресурса Теаммессагингсеттингс</span><span class="sxs-lookup"><span data-stu-id="13bd5-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13bd5-104">Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="13bd5-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="13bd5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="13bd5-105">Properties</span></span>
| <span data-ttu-id="13bd5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="13bd5-106">Property</span></span>     | <span data-ttu-id="13bd5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="13bd5-107">Type</span></span>   |<span data-ttu-id="13bd5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="13bd5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13bd5-109">Алловусередитмессажес</span><span class="sxs-lookup"><span data-stu-id="13bd5-109">allowUserEditMessages</span></span>|<span data-ttu-id="13bd5-110">Логический</span><span class="sxs-lookup"><span data-stu-id="13bd5-110">Boolean</span></span>|<span data-ttu-id="13bd5-111">Если задано значение true, пользователи могут редактировать сообщения.</span><span class="sxs-lookup"><span data-stu-id="13bd5-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="13bd5-112">Алловусерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="13bd5-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="13bd5-113">Логический</span><span class="sxs-lookup"><span data-stu-id="13bd5-113">Boolean</span></span>|<span data-ttu-id="13bd5-114">Если задано значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="13bd5-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="13bd5-115">Аллововнерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="13bd5-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="13bd5-116">Логический</span><span class="sxs-lookup"><span data-stu-id="13bd5-116">Boolean</span></span>|<span data-ttu-id="13bd5-117">Если задано значение true, владельцы могут удалять любые сообщения.</span><span class="sxs-lookup"><span data-stu-id="13bd5-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="13bd5-118">Алловтеамментионс</span><span class="sxs-lookup"><span data-stu-id="13bd5-118">allowTeamMentions</span></span>|<span data-ttu-id="13bd5-119">Логический</span><span class="sxs-lookup"><span data-stu-id="13bd5-119">Boolean</span></span>|<span data-ttu-id="13bd5-120">Если задано значение true, @team упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="13bd5-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="13bd5-121">Алловчаннелментионс</span><span class="sxs-lookup"><span data-stu-id="13bd5-121">allowChannelMentions</span></span>|<span data-ttu-id="13bd5-122">Логический</span><span class="sxs-lookup"><span data-stu-id="13bd5-122">Boolean</span></span>|<span data-ttu-id="13bd5-123">Если задано значение true, @channel упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="13bd5-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13bd5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13bd5-124">JSON representation</span></span>

<span data-ttu-id="13bd5-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13bd5-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
