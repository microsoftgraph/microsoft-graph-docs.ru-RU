---
title: тип ресурса chatMembersNotificationRecipient
description: Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из участников чата.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3743d9d37e934cd61f699febfcc148afb8e84e98
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211398"
---
# <a name="chatmembersnotificationrecipient-resource-type"></a><span data-ttu-id="dfb7b-104">тип ресурса chatMembersNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="dfb7b-104">chatMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="dfb7b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfb7b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfb7b-106">Представляет получателя уведомления, отправленного в канале Microsoft Teams действий.</span><span class="sxs-lookup"><span data-stu-id="dfb7b-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="dfb7b-107">Получатель состоит из участников чата.</span><span class="sxs-lookup"><span data-stu-id="dfb7b-107">The recipient consists of the chat members.</span></span>

<span data-ttu-id="dfb7b-108">Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="dfb7b-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dfb7b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfb7b-109">Properties</span></span>
|<span data-ttu-id="dfb7b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfb7b-110">Property</span></span>|<span data-ttu-id="dfb7b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dfb7b-111">Type</span></span>|<span data-ttu-id="dfb7b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dfb7b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb7b-113">chatId</span><span class="sxs-lookup"><span data-stu-id="dfb7b-113">chatId</span></span>|<span data-ttu-id="dfb7b-114">String</span><span class="sxs-lookup"><span data-stu-id="dfb7b-114">String</span></span>|<span data-ttu-id="dfb7b-115">Идентификатор чата.</span><span class="sxs-lookup"><span data-stu-id="dfb7b-115">The chat's identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb7b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="dfb7b-116">Relationships</span></span>
<span data-ttu-id="dfb7b-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dfb7b-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb7b-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dfb7b-118">JSON representation</span></span>
<span data-ttu-id="dfb7b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfb7b-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.chatMembersNotificationRecipient",
  "chatId": "String"
}
```

