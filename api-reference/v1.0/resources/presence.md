---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 31e042e59e9ede46c3649ccb623416147b676e06
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606974"
---
# <a name="presence-resource-type"></a><span data-ttu-id="95216-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="95216-103">presence resource type</span></span>

<span data-ttu-id="95216-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95216-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95216-105">Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.</span><span class="sxs-lookup"><span data-stu-id="95216-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="95216-106">**Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="95216-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="95216-107">Этот ресурс поддерживает подписку на [уведомления об изменениях](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="95216-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="95216-108">Методы</span><span class="sxs-lookup"><span data-stu-id="95216-108">Methods</span></span>

| <span data-ttu-id="95216-109">Метод</span><span class="sxs-lookup"><span data-stu-id="95216-109">Method</span></span>                                                            | <span data-ttu-id="95216-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95216-110">Return Type</span></span>                                       | <span data-ttu-id="95216-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95216-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="95216-112">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="95216-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="95216-113">presence</span><span class="sxs-lookup"><span data-stu-id="95216-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="95216-114">Получение сведений о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="95216-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="95216-115">Получение сведений о присутствии нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="95216-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="95216-116">Коллекция [присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="95216-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="95216-117">Получение сведений о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="95216-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="95216-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="95216-118">Properties</span></span>

| <span data-ttu-id="95216-119">Связь</span><span class="sxs-lookup"><span data-stu-id="95216-119">Relationship</span></span>        | <span data-ttu-id="95216-120">Тип</span><span class="sxs-lookup"><span data-stu-id="95216-120">Type</span></span>                                                 | <span data-ttu-id="95216-121">Описание</span><span class="sxs-lookup"><span data-stu-id="95216-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="95216-122">id</span><span class="sxs-lookup"><span data-stu-id="95216-122">id</span></span>    |  <span data-ttu-id="95216-123">string</span><span class="sxs-lookup"><span data-stu-id="95216-123">string</span></span>     |  <span data-ttu-id="95216-124">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="95216-124">The user object id</span></span>   |
|<span data-ttu-id="95216-125">availability</span><span class="sxs-lookup"><span data-stu-id="95216-125">availability</span></span>    |  <span data-ttu-id="95216-126">string collection</span><span class="sxs-lookup"><span data-stu-id="95216-126">string collection</span></span>   |   <span data-ttu-id="95216-127">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="95216-127">The base presence information for a user.</span></span> <span data-ttu-id="95216-128">Возможные значения:,,,,,,, `Available` `AvailableIdle`  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="95216-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="95216-129">activity</span><span class="sxs-lookup"><span data-stu-id="95216-129">activity</span></span>    |  <span data-ttu-id="95216-130">string collection</span><span class="sxs-lookup"><span data-stu-id="95216-130">string collection</span></span>      |    <span data-ttu-id="95216-131">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="95216-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="95216-132">Возможные значения:,,,,,,,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="95216-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="95216-133">**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="95216-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="95216-134">Связи</span><span class="sxs-lookup"><span data-stu-id="95216-134">Relationships</span></span>

<span data-ttu-id="95216-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="95216-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95216-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95216-136">JSON representation</span></span>

<span data-ttu-id="95216-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95216-137">The following is a JSON representation of the resource.</span></span>

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
