---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: c4b2b2ac4a2f9a11dcd68eee903223f8466ba25d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606883"
---
# <a name="presence-resource-type"></a><span data-ttu-id="4ce99-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="4ce99-103">presence resource type</span></span>

<span data-ttu-id="4ce99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ce99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ce99-105">Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.</span><span class="sxs-lookup"><span data-stu-id="4ce99-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="4ce99-106">**Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4ce99-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="4ce99-107">Этот ресурс поддерживает подписку на [уведомления об изменениях](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="4ce99-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="4ce99-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4ce99-108">Methods</span></span>

| <span data-ttu-id="4ce99-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4ce99-109">Method</span></span>                                                            | <span data-ttu-id="4ce99-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ce99-110">Return Type</span></span>                                       | <span data-ttu-id="4ce99-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce99-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="4ce99-112">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="4ce99-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="4ce99-113">presence</span><span class="sxs-lookup"><span data-stu-id="4ce99-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="4ce99-114">Получение сведений о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ce99-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="4ce99-115">Получение сведений о присутствии нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="4ce99-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="4ce99-116">Коллекция [присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="4ce99-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="4ce99-117">Получение сведений о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="4ce99-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="4ce99-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ce99-118">Properties</span></span>

| <span data-ttu-id="4ce99-119">Связь</span><span class="sxs-lookup"><span data-stu-id="4ce99-119">Relationship</span></span>        | <span data-ttu-id="4ce99-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4ce99-120">Type</span></span>                                                 | <span data-ttu-id="4ce99-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce99-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="4ce99-122">id</span><span class="sxs-lookup"><span data-stu-id="4ce99-122">id</span></span>    |  <span data-ttu-id="4ce99-123">string</span><span class="sxs-lookup"><span data-stu-id="4ce99-123">string</span></span>     |  <span data-ttu-id="4ce99-124">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="4ce99-124">The user object id</span></span>   |
|<span data-ttu-id="4ce99-125">availability</span><span class="sxs-lookup"><span data-stu-id="4ce99-125">availability</span></span>    |  <span data-ttu-id="4ce99-126">string collection</span><span class="sxs-lookup"><span data-stu-id="4ce99-126">string collection</span></span>   |   <span data-ttu-id="4ce99-127">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ce99-127">The base presence information for a user.</span></span> <span data-ttu-id="4ce99-128">Возможные значения:,,,,,,, `Available` `AvailableIdle`  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="4ce99-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="4ce99-129">activity</span><span class="sxs-lookup"><span data-stu-id="4ce99-129">activity</span></span>    |  <span data-ttu-id="4ce99-130">string collection</span><span class="sxs-lookup"><span data-stu-id="4ce99-130">string collection</span></span>      |    <span data-ttu-id="4ce99-131">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ce99-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="4ce99-132">Возможные значения:,,,,,,,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="4ce99-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="4ce99-133">**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="4ce99-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="4ce99-134">Связи</span><span class="sxs-lookup"><span data-stu-id="4ce99-134">Relationships</span></span>

<span data-ttu-id="4ce99-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ce99-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ce99-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ce99-136">JSON representation</span></span>

<span data-ttu-id="4ce99-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ce99-137">The following is a JSON representation of the resource.</span></span>

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
