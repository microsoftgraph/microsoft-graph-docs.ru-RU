---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 27ef5062e84f20dc1dbf6be11020f421871fbc09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033840"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="449e7-103">Тип ресурса Теаммессагингсеттингс</span><span class="sxs-lookup"><span data-stu-id="449e7-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="449e7-104">Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="449e7-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="449e7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="449e7-105">Properties</span></span>
| <span data-ttu-id="449e7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="449e7-106">Property</span></span>     | <span data-ttu-id="449e7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="449e7-107">Type</span></span>   |<span data-ttu-id="449e7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="449e7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="449e7-109">Алловусередитмессажес</span><span class="sxs-lookup"><span data-stu-id="449e7-109">allowUserEditMessages</span></span>|<span data-ttu-id="449e7-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="449e7-110">Boolean</span></span>|<span data-ttu-id="449e7-111">Если задано значение true, пользователи могут редактировать сообщения.</span><span class="sxs-lookup"><span data-stu-id="449e7-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="449e7-112">Алловусерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="449e7-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="449e7-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="449e7-113">Boolean</span></span>|<span data-ttu-id="449e7-114">Если задано значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="449e7-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="449e7-115">Аллововнерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="449e7-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="449e7-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="449e7-116">Boolean</span></span>|<span data-ttu-id="449e7-117">Если задано значение true, владельцы могут удалять любые сообщения.</span><span class="sxs-lookup"><span data-stu-id="449e7-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="449e7-118">Алловтеамментионс</span><span class="sxs-lookup"><span data-stu-id="449e7-118">allowTeamMentions</span></span>|<span data-ttu-id="449e7-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="449e7-119">Boolean</span></span>|<span data-ttu-id="449e7-120">Если задано значение true, @team упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="449e7-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="449e7-121">Алловчаннелментионс</span><span class="sxs-lookup"><span data-stu-id="449e7-121">allowChannelMentions</span></span>|<span data-ttu-id="449e7-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="449e7-122">Boolean</span></span>|<span data-ttu-id="449e7-123">Если задано значение true, @channel упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="449e7-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="449e7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="449e7-124">JSON representation</span></span>

<span data-ttu-id="449e7-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="449e7-125">The following is a JSON representation of the resource.</span></span>

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
