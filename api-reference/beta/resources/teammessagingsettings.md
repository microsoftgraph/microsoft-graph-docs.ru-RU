---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a89ed35c820338cde7b3f22a7345c860b1a4427
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964531"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="1ea21-103">Тип ресурса Теаммессагингсеттингс</span><span class="sxs-lookup"><span data-stu-id="1ea21-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ea21-104">Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="1ea21-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1ea21-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ea21-105">Properties</span></span>
| <span data-ttu-id="1ea21-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ea21-106">Property</span></span>     | <span data-ttu-id="1ea21-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1ea21-107">Type</span></span>   |<span data-ttu-id="1ea21-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1ea21-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ea21-109">Алловусередитмессажес</span><span class="sxs-lookup"><span data-stu-id="1ea21-109">allowUserEditMessages</span></span>|<span data-ttu-id="1ea21-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ea21-110">Boolean</span></span>|<span data-ttu-id="1ea21-111">Если задано значение true, пользователи могут редактировать сообщения.</span><span class="sxs-lookup"><span data-stu-id="1ea21-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="1ea21-112">Алловусерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="1ea21-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="1ea21-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ea21-113">Boolean</span></span>|<span data-ttu-id="1ea21-114">Если задано значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="1ea21-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="1ea21-115">Аллововнерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="1ea21-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="1ea21-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ea21-116">Boolean</span></span>|<span data-ttu-id="1ea21-117">Если задано значение true, владельцы могут удалять любые сообщения.</span><span class="sxs-lookup"><span data-stu-id="1ea21-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="1ea21-118">Алловтеамментионс</span><span class="sxs-lookup"><span data-stu-id="1ea21-118">allowTeamMentions</span></span>|<span data-ttu-id="1ea21-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ea21-119">Boolean</span></span>|<span data-ttu-id="1ea21-120">Если задано значение true, @team упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="1ea21-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="1ea21-121">Алловчаннелментионс</span><span class="sxs-lookup"><span data-stu-id="1ea21-121">allowChannelMentions</span></span>|<span data-ttu-id="1ea21-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ea21-122">Boolean</span></span>|<span data-ttu-id="1ea21-123">Если задано значение true, @channel упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="1ea21-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ea21-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ea21-124">JSON representation</span></span>

<span data-ttu-id="1ea21-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ea21-125">The following is a JSON representation of the resource.</span></span>

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
