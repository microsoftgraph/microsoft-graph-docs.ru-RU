---
title: Тип ресурса presence
description: Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: ddbe555df37d232940bb8eadb081be459d0f8562
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796579"
---
# <a name="presence-resource-type"></a><span data-ttu-id="b9f58-103">Тип ресурса presence</span><span class="sxs-lookup"><span data-stu-id="b9f58-103">presence resource type</span></span>

<span data-ttu-id="b9f58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f58-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9f58-105">Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.</span><span class="sxs-lookup"><span data-stu-id="b9f58-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="b9f58-106">**Примечание.** В настоящее время этот ресурс поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b9f58-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="b9f58-107">Этот ресурс поддерживает подписку на уведомления [об изменениях.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="b9f58-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="b9f58-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b9f58-108">Methods</span></span>

| <span data-ttu-id="b9f58-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b9f58-109">Method</span></span>                                                            | <span data-ttu-id="b9f58-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b9f58-110">Return Type</span></span>                                       | <span data-ttu-id="b9f58-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f58-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="b9f58-112">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="b9f58-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="b9f58-113">presence</span><span class="sxs-lookup"><span data-stu-id="b9f58-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="b9f58-114">Получите сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9f58-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="b9f58-115">Получить присутствие нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="b9f58-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="b9f58-116">[коллекция presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="b9f58-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="b9f58-117">Получите сведения о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="b9f58-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="b9f58-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9f58-118">Properties</span></span>

| <span data-ttu-id="b9f58-119">Связь</span><span class="sxs-lookup"><span data-stu-id="b9f58-119">Relationship</span></span>        | <span data-ttu-id="b9f58-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b9f58-120">Type</span></span>                                                 | <span data-ttu-id="b9f58-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f58-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="b9f58-122">id</span><span class="sxs-lookup"><span data-stu-id="b9f58-122">id</span></span>    |  <span data-ttu-id="b9f58-123">string</span><span class="sxs-lookup"><span data-stu-id="b9f58-123">string</span></span>     |  <span data-ttu-id="b9f58-124">ИД объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="b9f58-124">The user object id</span></span>   |
|<span data-ttu-id="b9f58-125">availability</span><span class="sxs-lookup"><span data-stu-id="b9f58-125">availability</span></span>    |  <span data-ttu-id="b9f58-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b9f58-126">string collection</span></span>   |   <span data-ttu-id="b9f58-127">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9f58-127">The base presence information for a user.</span></span> <span data-ttu-id="b9f58-128">Возможные значения: `Available` `AvailableIdle` , , `Away` `BeRightBack` , `Busy` `BusyIdle` `DoNotDisturb` `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="b9f58-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="b9f58-129">действие</span><span class="sxs-lookup"><span data-stu-id="b9f58-129">activity</span></span>    |  <span data-ttu-id="b9f58-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b9f58-130">string collection</span></span>      |    <span data-ttu-id="b9f58-131">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9f58-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="b9f58-132">Возможные значения: `Available` `Away` , `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="b9f58-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |
|<span data-ttu-id="b9f58-133">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="b9f58-133">outOfOfficeSettings</span></span> | [<span data-ttu-id="b9f58-134">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="b9f58-134">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="b9f58-135">Параметры "Нет на месте" для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9f58-135">The out of office settings for a user.</span></span> |

><span data-ttu-id="b9f58-136">**Примечание.** Дополнительные данные о различных состояниях присутствия см. в [записях о присутствии пользователей в Teams.](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="b9f58-136">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="b9f58-137">Связи</span><span class="sxs-lookup"><span data-stu-id="b9f58-137">Relationships</span></span>

<span data-ttu-id="b9f58-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9f58-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9f58-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9f58-139">JSON representation</span></span>

<span data-ttu-id="b9f58-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9f58-140">The following is a JSON representation of the resource.</span></span>

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
   "activity":"string",
   "outOfOfficeSettings":{"@odata.type": "#microsoft.graph.outOfOfficeSettings"}
}
```
