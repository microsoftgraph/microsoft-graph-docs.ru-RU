---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: d6f88f23a6c08d5aa757163d4956c104a603e87b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515634"
---
# <a name="presence-resource-type"></a><span data-ttu-id="0c54a-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="0c54a-103">presence resource type</span></span>

<span data-ttu-id="0c54a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c54a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c54a-105">Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c54a-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="0c54a-106">**Примечание:** В настоящее время этот ресурс поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0c54a-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="0c54a-107">Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="0c54a-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="0c54a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0c54a-108">Methods</span></span>

| <span data-ttu-id="0c54a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0c54a-109">Method</span></span>                                                            | <span data-ttu-id="0c54a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c54a-110">Return Type</span></span>                                       | <span data-ttu-id="0c54a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c54a-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="0c54a-112">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="0c54a-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="0c54a-113">presence</span><span class="sxs-lookup"><span data-stu-id="0c54a-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="0c54a-114">Получите сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="0c54a-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="0c54a-115">Наличие нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="0c54a-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="0c54a-116">[Коллекция присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="0c54a-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="0c54a-117">Получите сведения о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c54a-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="0c54a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c54a-118">Properties</span></span>

| <span data-ttu-id="0c54a-119">Связь</span><span class="sxs-lookup"><span data-stu-id="0c54a-119">Relationship</span></span>        | <span data-ttu-id="0c54a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0c54a-120">Type</span></span>                                                 | <span data-ttu-id="0c54a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0c54a-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="0c54a-122">id</span><span class="sxs-lookup"><span data-stu-id="0c54a-122">id</span></span>    |  <span data-ttu-id="0c54a-123">string</span><span class="sxs-lookup"><span data-stu-id="0c54a-123">string</span></span>     |  <span data-ttu-id="0c54a-124">ID объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="0c54a-124">The user object id</span></span>   |
|<span data-ttu-id="0c54a-125">availability</span><span class="sxs-lookup"><span data-stu-id="0c54a-125">availability</span></span>    |  <span data-ttu-id="0c54a-126">string collection</span><span class="sxs-lookup"><span data-stu-id="0c54a-126">string collection</span></span>   |   <span data-ttu-id="0c54a-127">Базовые сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="0c54a-127">The base presence information for a user.</span></span> <span data-ttu-id="0c54a-128">Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="0c54a-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="0c54a-129">действие</span><span class="sxs-lookup"><span data-stu-id="0c54a-129">activity</span></span>    |  <span data-ttu-id="0c54a-130">string collection</span><span class="sxs-lookup"><span data-stu-id="0c54a-130">string collection</span></span>      |    <span data-ttu-id="0c54a-131">Дополнительные сведения о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="0c54a-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="0c54a-132">Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="0c54a-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |
|<span data-ttu-id="0c54a-133">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="0c54a-133">outOfOfficeSettings</span></span> | [<span data-ttu-id="0c54a-134">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="0c54a-134">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="0c54a-135">Параметры вне офиса для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0c54a-135">The out of office settings for a user.</span></span> |

><span data-ttu-id="0c54a-136">**Примечание:** Дополнительные данные о различных состояниях присутствия см. в [записи Присутствия пользователя в Teams.](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="0c54a-136">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="0c54a-137">Связи</span><span class="sxs-lookup"><span data-stu-id="0c54a-137">Relationships</span></span>

<span data-ttu-id="0c54a-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c54a-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c54a-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c54a-139">JSON representation</span></span>

<span data-ttu-id="0c54a-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c54a-140">The following is a JSON representation of the resource.</span></span>

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
