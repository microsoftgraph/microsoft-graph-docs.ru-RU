---
title: Тип ресурса Теаммессагингсеттингс
description: Параметры для настройки обмена сообщениями и упоминаний в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 213a8d388b80a4b35d26afc0071445a8ac6095b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519934"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="62ce7-103">Тип ресурса Теаммессагингсеттингс</span><span class="sxs-lookup"><span data-stu-id="62ce7-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="62ce7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62ce7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62ce7-105">Параметры для настройки обмена сообщениями и упоминаний в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="62ce7-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="62ce7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62ce7-106">Properties</span></span>
| <span data-ttu-id="62ce7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62ce7-107">Property</span></span>     | <span data-ttu-id="62ce7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62ce7-108">Type</span></span>   |<span data-ttu-id="62ce7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62ce7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62ce7-110">алловусередитмессажес</span><span class="sxs-lookup"><span data-stu-id="62ce7-110">allowUserEditMessages</span></span>|<span data-ttu-id="62ce7-111">Логическое</span><span class="sxs-lookup"><span data-stu-id="62ce7-111">Boolean</span></span>|<span data-ttu-id="62ce7-112">Если задано значение true, пользователи могут редактировать сообщения.</span><span class="sxs-lookup"><span data-stu-id="62ce7-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="62ce7-113">алловусерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="62ce7-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="62ce7-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="62ce7-114">Boolean</span></span>|<span data-ttu-id="62ce7-115">Если задано значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="62ce7-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="62ce7-116">аллововнерделетемессажес</span><span class="sxs-lookup"><span data-stu-id="62ce7-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="62ce7-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="62ce7-117">Boolean</span></span>|<span data-ttu-id="62ce7-118">Если задано значение true, владельцы могут удалять любые сообщения.</span><span class="sxs-lookup"><span data-stu-id="62ce7-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="62ce7-119">алловтеамментионс</span><span class="sxs-lookup"><span data-stu-id="62ce7-119">allowTeamMentions</span></span>|<span data-ttu-id="62ce7-120">Логическое</span><span class="sxs-lookup"><span data-stu-id="62ce7-120">Boolean</span></span>|<span data-ttu-id="62ce7-121">Если задано значение true, @team упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="62ce7-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="62ce7-122">алловчаннелментионс</span><span class="sxs-lookup"><span data-stu-id="62ce7-122">allowChannelMentions</span></span>|<span data-ttu-id="62ce7-123">Логическое</span><span class="sxs-lookup"><span data-stu-id="62ce7-123">Boolean</span></span>|<span data-ttu-id="62ce7-124">Если задано значение true, @channel упоминаний разрешены.</span><span class="sxs-lookup"><span data-stu-id="62ce7-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62ce7-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62ce7-125">JSON representation</span></span>

<span data-ttu-id="62ce7-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62ce7-126">The following is a JSON representation of the resource.</span></span>

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
