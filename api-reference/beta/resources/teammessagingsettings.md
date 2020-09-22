---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 352fc5bc8a8794a455a84d729bb3b2cea6ad34f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046632"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="55406-103">Тип ресурса Теаммессагингсеттингс</span><span class="sxs-lookup"><span data-stu-id="55406-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="55406-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55406-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55406-105">Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="55406-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="55406-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="55406-106">Properties</span></span>
| <span data-ttu-id="55406-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="55406-107">Property</span></span>     | <span data-ttu-id="55406-108">Тип</span><span class="sxs-lookup"><span data-stu-id="55406-108">Type</span></span>   |<span data-ttu-id="55406-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55406-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55406-110">алловусередитмессажес</span><span class="sxs-lookup"><span data-stu-id="55406-110">allowUserEditMessages</span></span>|<span data-ttu-id="55406-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="55406-111">Boolean</span></span>|<span data-ttu-id="55406-112">Если задано значение true, пользователи могут редактировать сообщения.</span><span class="sxs-lookup"><span data-stu-id="55406-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="55406-113">алловусерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="55406-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="55406-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="55406-114">Boolean</span></span>|<span data-ttu-id="55406-115">Если задано значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="55406-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="55406-116">аллововнерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="55406-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="55406-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="55406-117">Boolean</span></span>|<span data-ttu-id="55406-118">Если задано значение true, владельцы могут удалять любые сообщения.</span><span class="sxs-lookup"><span data-stu-id="55406-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="55406-119">алловтеамментионс</span><span class="sxs-lookup"><span data-stu-id="55406-119">allowTeamMentions</span></span>|<span data-ttu-id="55406-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="55406-120">Boolean</span></span>|<span data-ttu-id="55406-121">Если задано значение true, @team упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="55406-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="55406-122">алловчаннелментионс</span><span class="sxs-lookup"><span data-stu-id="55406-122">allowChannelMentions</span></span>|<span data-ttu-id="55406-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="55406-123">Boolean</span></span>|<span data-ttu-id="55406-124">Если задано значение true, @channel упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="55406-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55406-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55406-125">JSON representation</span></span>

<span data-ttu-id="55406-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55406-126">The following is a JSON representation of the resource.</span></span>

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


