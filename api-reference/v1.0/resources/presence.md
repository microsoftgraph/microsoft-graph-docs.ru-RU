---
title: Тип ресурса presence
description: Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 1122e14c91a8562757434e4bd36e267ed70790dd
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675963"
---
# <a name="presence-resource-type"></a><span data-ttu-id="85183-103">Тип ресурса presence</span><span class="sxs-lookup"><span data-stu-id="85183-103">presence resource type</span></span>

<span data-ttu-id="85183-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85183-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85183-105">Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.</span><span class="sxs-lookup"><span data-stu-id="85183-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="85183-106">**Примечание.** В настоящее время этот ресурс поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="85183-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="85183-107">Этот ресурс поддерживает подписку на уведомления [об изменениях.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="85183-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="85183-108">Методы</span><span class="sxs-lookup"><span data-stu-id="85183-108">Methods</span></span>

| <span data-ttu-id="85183-109">Метод</span><span class="sxs-lookup"><span data-stu-id="85183-109">Method</span></span>                                                            | <span data-ttu-id="85183-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85183-110">Return Type</span></span>                                       | <span data-ttu-id="85183-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85183-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="85183-112">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="85183-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="85183-113">presence</span><span class="sxs-lookup"><span data-stu-id="85183-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="85183-114">Получите сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="85183-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="85183-115">Получить присутствие нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="85183-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="85183-116">[коллекция presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="85183-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="85183-117">Получите сведения о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="85183-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="85183-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="85183-118">Properties</span></span>

| <span data-ttu-id="85183-119">Связь</span><span class="sxs-lookup"><span data-stu-id="85183-119">Relationship</span></span>        | <span data-ttu-id="85183-120">Тип</span><span class="sxs-lookup"><span data-stu-id="85183-120">Type</span></span>                                                 | <span data-ttu-id="85183-121">Описание</span><span class="sxs-lookup"><span data-stu-id="85183-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="85183-122">id</span><span class="sxs-lookup"><span data-stu-id="85183-122">id</span></span>    |  <span data-ttu-id="85183-123">string</span><span class="sxs-lookup"><span data-stu-id="85183-123">string</span></span>     |  <span data-ttu-id="85183-124">ИД объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="85183-124">The user object id</span></span>   |
|<span data-ttu-id="85183-125">availability</span><span class="sxs-lookup"><span data-stu-id="85183-125">availability</span></span>    |  <span data-ttu-id="85183-126">string collection</span><span class="sxs-lookup"><span data-stu-id="85183-126">string collection</span></span>   |   <span data-ttu-id="85183-127">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="85183-127">The base presence information for a user.</span></span> <span data-ttu-id="85183-128">Возможные значения: `Available` , , , , `AvailableIdle`  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="85183-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="85183-129">activity</span><span class="sxs-lookup"><span data-stu-id="85183-129">activity</span></span>    |  <span data-ttu-id="85183-130">string collection</span><span class="sxs-lookup"><span data-stu-id="85183-130">string collection</span></span>      |    <span data-ttu-id="85183-131">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="85183-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="85183-132">Возможные значения: `Available` , , , , , , `Away` , `BeRightBack` , `Busy` , `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="85183-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`, `InAMeeting`, `Offline`, `OffWork`, `OutOfOffice`, `PresenceUnknown`, `Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="85183-133">**Примечание.** Дополнительные данные о различных состояниях присутствия см. в [записях о присутствии пользователей в Teams.](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="85183-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="85183-134">Связи</span><span class="sxs-lookup"><span data-stu-id="85183-134">Relationships</span></span>

<span data-ttu-id="85183-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="85183-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85183-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="85183-136">JSON representation</span></span>

<span data-ttu-id="85183-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85183-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string"
}
```
