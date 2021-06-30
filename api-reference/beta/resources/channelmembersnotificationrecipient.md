---
title: тип ресурса channelMembersNotificationRecipient
description: Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из участников канала.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 821d4f2ee41c15cb93cd3d53b9af9cf1e63db97b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211403"
---
# <a name="channelmembersnotificationrecipient-resource-type"></a><span data-ttu-id="abe03-104">тип ресурса channelMembersNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="abe03-104">channelMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="abe03-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abe03-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe03-106">Представляет получателя уведомления, отправленного в канале Microsoft Teams действий.</span><span class="sxs-lookup"><span data-stu-id="abe03-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="abe03-107">Получатель состоит из участников канала.</span><span class="sxs-lookup"><span data-stu-id="abe03-107">The recipient consists of the channel members.</span></span>

<span data-ttu-id="abe03-108">Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="abe03-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="abe03-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="abe03-109">Properties</span></span>
| <span data-ttu-id="abe03-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="abe03-110">Property</span></span>  | <span data-ttu-id="abe03-111">Тип</span><span class="sxs-lookup"><span data-stu-id="abe03-111">Type</span></span>   | <span data-ttu-id="abe03-112">Описание</span><span class="sxs-lookup"><span data-stu-id="abe03-112">Description</span></span>                                            |
| :-------- | :----- | :----------------------------------------------------- |
| <span data-ttu-id="abe03-113">teamId</span><span class="sxs-lookup"><span data-stu-id="abe03-113">teamId</span></span>    | <span data-ttu-id="abe03-114">String</span><span class="sxs-lookup"><span data-stu-id="abe03-114">String</span></span> | <span data-ttu-id="abe03-115">Идентификатор группы, под которым находится канал.</span><span class="sxs-lookup"><span data-stu-id="abe03-115">The team's identifier under which the channel resides.</span></span> |
| <span data-ttu-id="abe03-116">channelId</span><span class="sxs-lookup"><span data-stu-id="abe03-116">channelId</span></span> | <span data-ttu-id="abe03-117">String</span><span class="sxs-lookup"><span data-stu-id="abe03-117">String</span></span> | <span data-ttu-id="abe03-118">Идентификатор канала.</span><span class="sxs-lookup"><span data-stu-id="abe03-118">The channel's identifier.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="abe03-119">Связи</span><span class="sxs-lookup"><span data-stu-id="abe03-119">Relationships</span></span>
<span data-ttu-id="abe03-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="abe03-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="abe03-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="abe03-121">JSON representation</span></span>
<span data-ttu-id="abe03-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abe03-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.channelMembersNotificationRecipient",
  "teamId": "String",
  "channelId": "String"
}
```
