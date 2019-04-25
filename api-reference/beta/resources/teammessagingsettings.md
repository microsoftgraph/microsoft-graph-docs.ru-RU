---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553950"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="b8501-103">Тип ресурса Теаммессагингсеттингс</span><span class="sxs-lookup"><span data-stu-id="b8501-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="b8501-104">Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="b8501-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b8501-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8501-105">Properties</span></span>
| <span data-ttu-id="b8501-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8501-106">Property</span></span>     | <span data-ttu-id="b8501-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b8501-107">Type</span></span>   |<span data-ttu-id="b8501-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b8501-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8501-109">Алловусередитмессажес</span><span class="sxs-lookup"><span data-stu-id="b8501-109">allowUserEditMessages</span></span>|<span data-ttu-id="b8501-110">Логический</span><span class="sxs-lookup"><span data-stu-id="b8501-110">Boolean</span></span>|<span data-ttu-id="b8501-111">Если задано значение true, пользователи могут редактировать сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8501-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="b8501-112">Алловусерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="b8501-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="b8501-113">Логический</span><span class="sxs-lookup"><span data-stu-id="b8501-113">Boolean</span></span>|<span data-ttu-id="b8501-114">Если задано значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8501-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="b8501-115">Аллововнерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="b8501-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="b8501-116">Логический</span><span class="sxs-lookup"><span data-stu-id="b8501-116">Boolean</span></span>|<span data-ttu-id="b8501-117">Если задано значение true, владельцы могут удалять любые сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8501-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="b8501-118">Алловтеамментионс</span><span class="sxs-lookup"><span data-stu-id="b8501-118">allowTeamMentions</span></span>|<span data-ttu-id="b8501-119">Логический</span><span class="sxs-lookup"><span data-stu-id="b8501-119">Boolean</span></span>|<span data-ttu-id="b8501-120">Если задано значение true, @team упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="b8501-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="b8501-121">Алловчаннелментионс</span><span class="sxs-lookup"><span data-stu-id="b8501-121">allowChannelMentions</span></span>|<span data-ttu-id="b8501-122">Логический</span><span class="sxs-lookup"><span data-stu-id="b8501-122">Boolean</span></span>|<span data-ttu-id="b8501-123">Если задано значение true, @channel упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="b8501-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8501-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b8501-124">JSON representation</span></span>

<span data-ttu-id="b8501-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8501-125">The following is a JSON representation of the resource.</span></span>

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
