---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8a907bc56475634d4c677aa670d398e9ab13ff50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073532"
---
# <a name="presence-resource-type"></a><span data-ttu-id="0d703-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="0d703-103">presence resource type</span></span>

<span data-ttu-id="0d703-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d703-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d703-105">Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.</span><span class="sxs-lookup"><span data-stu-id="0d703-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="0d703-106">**Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0d703-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="0d703-107">Этот ресурс поддерживает подписку на [уведомления об изменениях](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="0d703-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="0d703-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0d703-108">Methods</span></span>

| <span data-ttu-id="0d703-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0d703-109">Method</span></span>                                                            | <span data-ttu-id="0d703-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d703-110">Return Type</span></span>                                       | <span data-ttu-id="0d703-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d703-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="0d703-112">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="0d703-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="0d703-113">presence</span><span class="sxs-lookup"><span data-stu-id="0d703-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="0d703-114">Получение сведений о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d703-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="0d703-115">Получение сведений о присутствии нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="0d703-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="0d703-116">Коллекция [присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="0d703-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="0d703-117">Получение сведений о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="0d703-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="0d703-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d703-118">Properties</span></span>

| <span data-ttu-id="0d703-119">Связь</span><span class="sxs-lookup"><span data-stu-id="0d703-119">Relationship</span></span>        | <span data-ttu-id="0d703-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0d703-120">Type</span></span>                                                 | <span data-ttu-id="0d703-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0d703-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="0d703-122">id</span><span class="sxs-lookup"><span data-stu-id="0d703-122">id</span></span>    |  <span data-ttu-id="0d703-123">string</span><span class="sxs-lookup"><span data-stu-id="0d703-123">string</span></span>     |  <span data-ttu-id="0d703-124">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="0d703-124">The user object id</span></span>   |
|<span data-ttu-id="0d703-125">availability</span><span class="sxs-lookup"><span data-stu-id="0d703-125">availability</span></span>    |  <span data-ttu-id="0d703-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0d703-126">string collection</span></span>   |   <span data-ttu-id="0d703-127">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d703-127">The base presence information for a user.</span></span> <span data-ttu-id="0d703-128">Возможные значения:,,,,,,, `Available` `AvailableIdle`  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="0d703-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="0d703-129">activity</span><span class="sxs-lookup"><span data-stu-id="0d703-129">activity</span></span>    |  <span data-ttu-id="0d703-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0d703-130">string collection</span></span>      |    <span data-ttu-id="0d703-131">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d703-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="0d703-132">Возможные значения:,,,,,,,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="0d703-132">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="0d703-133">**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="0d703-133">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="0d703-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d703-134">Relationships</span></span>

<span data-ttu-id="0d703-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0d703-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d703-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0d703-136">JSON representation</span></span>

<span data-ttu-id="0d703-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d703-137">The following is a JSON representation of the resource.</span></span>

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


