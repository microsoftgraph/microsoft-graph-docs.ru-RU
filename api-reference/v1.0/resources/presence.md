---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: mkhribech
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: f155db24626420bfb43b225ee67d61ae923b048f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896720"
---
# <a name="presence-resource-type"></a><span data-ttu-id="ae658-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="ae658-103">presence resource type</span></span>

<span data-ttu-id="ae658-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae658-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae658-105">Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae658-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="ae658-106">**Примечание:** В настоящее время этот ресурс поддерживается только для Microsoft Teams пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae658-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="ae658-107">Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="ae658-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="ae658-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ae658-108">Methods</span></span>

| <span data-ttu-id="ae658-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ae658-109">Method</span></span>                                                            | <span data-ttu-id="ae658-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ae658-110">Return Type</span></span>                                       | <span data-ttu-id="ae658-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ae658-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="ae658-112">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="ae658-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="ae658-113">presence</span><span class="sxs-lookup"><span data-stu-id="ae658-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="ae658-114">Получите сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae658-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="ae658-115">Наличие нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="ae658-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="ae658-116">[Коллекция присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="ae658-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="ae658-117">Получите сведения о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae658-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="ae658-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae658-118">Properties</span></span>

| <span data-ttu-id="ae658-119">Связь</span><span class="sxs-lookup"><span data-stu-id="ae658-119">Relationship</span></span>        | <span data-ttu-id="ae658-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ae658-120">Type</span></span>                                                 | <span data-ttu-id="ae658-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ae658-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="ae658-122">id</span><span class="sxs-lookup"><span data-stu-id="ae658-122">id</span></span>    |  <span data-ttu-id="ae658-123">строка</span><span class="sxs-lookup"><span data-stu-id="ae658-123">string</span></span>     |  <span data-ttu-id="ae658-124">ID объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="ae658-124">The user object id</span></span>   |
|<span data-ttu-id="ae658-125">availability</span><span class="sxs-lookup"><span data-stu-id="ae658-125">availability</span></span>    |  <span data-ttu-id="ae658-126">string collection</span><span class="sxs-lookup"><span data-stu-id="ae658-126">string collection</span></span>   |   <span data-ttu-id="ae658-127">Базовые сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae658-127">The base presence information for a user.</span></span> <span data-ttu-id="ae658-128">Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="ae658-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="ae658-129">действие</span><span class="sxs-lookup"><span data-stu-id="ae658-129">activity</span></span>    |  <span data-ttu-id="ae658-130">string collection</span><span class="sxs-lookup"><span data-stu-id="ae658-130">string collection</span></span>      |    <span data-ttu-id="ae658-131">Дополнительные сведения о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae658-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="ae658-132">Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="ae658-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`, `InAMeeting`, `Offline`, `OffWork`, `OutOfOffice`, `PresenceUnknown`, `Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="ae658-133">**Примечание:** Дополнительные данные о различных состояниях присутствия см. в [Teams.](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="ae658-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="ae658-134">Связи</span><span class="sxs-lookup"><span data-stu-id="ae658-134">Relationships</span></span>

<span data-ttu-id="ae658-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae658-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae658-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ae658-136">JSON representation</span></span>

<span data-ttu-id="ae658-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae658-137">The following is a JSON representation of the resource.</span></span>

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
