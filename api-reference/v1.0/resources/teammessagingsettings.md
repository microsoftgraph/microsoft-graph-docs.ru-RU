---
title: Тип ресурса teamMessagingSettings
description: Параметры для настройки системы обмена сообщениями и упоминания рабочих групп.
ms.openlocfilehash: 6d1ca12b473f2773d4f56e12405b17e21b0bd0ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025589"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="a9873-103">Тип ресурса teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="a9873-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="a9873-104">Параметры для настройки системы обмена сообщениями и упоминания в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="a9873-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a9873-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9873-105">Properties</span></span>
| <span data-ttu-id="a9873-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9873-106">Property</span></span>     | <span data-ttu-id="a9873-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a9873-107">Type</span></span>   |<span data-ttu-id="a9873-108">Description</span><span class="sxs-lookup"><span data-stu-id="a9873-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9873-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="a9873-109">allowUserEditMessages</span></span>|<span data-ttu-id="a9873-110">Логический</span><span class="sxs-lookup"><span data-stu-id="a9873-110">Boolean</span></span>|<span data-ttu-id="a9873-111">Если параметр имеет значение true, пользователи могут изменять свои сообщения;</span><span class="sxs-lookup"><span data-stu-id="a9873-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="a9873-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="a9873-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="a9873-113">Логический</span><span class="sxs-lookup"><span data-stu-id="a9873-113">Boolean</span></span>|<span data-ttu-id="a9873-114">Если параметр имеет значение true, пользователи могут удалять свои сообщения.</span><span class="sxs-lookup"><span data-stu-id="a9873-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="a9873-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="a9873-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="a9873-116">Логический</span><span class="sxs-lookup"><span data-stu-id="a9873-116">Boolean</span></span>|<span data-ttu-id="a9873-117">Если параметр имеет значение true, владельцы могут удалять все сообщения.</span><span class="sxs-lookup"><span data-stu-id="a9873-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="a9873-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="a9873-118">allowTeamMentions</span></span>|<span data-ttu-id="a9873-119">Логический</span><span class="sxs-lookup"><span data-stu-id="a9873-119">Boolean</span></span>|<span data-ttu-id="a9873-120">Если задано значение true, допускаются упоминания @team.</span><span class="sxs-lookup"><span data-stu-id="a9873-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="a9873-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="a9873-121">allowChannelMentions</span></span>|<span data-ttu-id="a9873-122">Логический</span><span class="sxs-lookup"><span data-stu-id="a9873-122">Boolean</span></span>|<span data-ttu-id="a9873-123">Если задано значение true, допускаются упоминания @channel.</span><span class="sxs-lookup"><span data-stu-id="a9873-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9873-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9873-124">JSON representation</span></span>

<span data-ttu-id="a9873-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9873-125">The following is a JSON representation of the resource.</span></span>

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
