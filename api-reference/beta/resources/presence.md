---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 257167fe5b7d417751771650f8e5f03b3dd66296
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107692"
---
# <a name="presence-resource-type"></a><span data-ttu-id="7881e-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="7881e-103">presence resource type</span></span>

<span data-ttu-id="7881e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7881e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7881e-105">Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.</span><span class="sxs-lookup"><span data-stu-id="7881e-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="7881e-106">**Примечание:** В настоящее время этот ресурс поддерживается только для Microsoft Teams пользователей.</span><span class="sxs-lookup"><span data-stu-id="7881e-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="7881e-107">Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="7881e-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="7881e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7881e-108">Methods</span></span>

| <span data-ttu-id="7881e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7881e-109">Method</span></span>                                                                               | <span data-ttu-id="7881e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7881e-110">Return Type</span></span>                                     | <span data-ttu-id="7881e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7881e-111">Description</span></span>                                      |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :----------------------------------------------- |
| [<span data-ttu-id="7881e-112">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="7881e-112">Get presence</span></span>](../api/presence-get.md)                                               | [<span data-ttu-id="7881e-113">presence</span><span class="sxs-lookup"><span data-stu-id="7881e-113">presence</span></span>](../resources/presence.md)            | <span data-ttu-id="7881e-114">Получите сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="7881e-114">Get a user's presence information.</span></span>               |
| [<span data-ttu-id="7881e-115">Наличие нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="7881e-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md) | <span data-ttu-id="7881e-116">[Коллекция присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="7881e-116">[presence](../resources/presence.md) collection</span></span> | <span data-ttu-id="7881e-117">Получите сведения о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="7881e-117">Get the presence information for multiple users.</span></span> |
| [<span data-ttu-id="7881e-118">Настройка присутствия</span><span class="sxs-lookup"><span data-stu-id="7881e-118">Set presence</span></span>](../api/presence-setpresence.md)                                               |                                                 | <span data-ttu-id="7881e-119">Установите сеанс присутствия приложения для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7881e-119">Set an application's presence session for a user.</span></span>           |
| [<span data-ttu-id="7881e-120">Четкое присутствие</span><span class="sxs-lookup"><span data-stu-id="7881e-120">Clear presence</span></span>](../api/presence-clearpresence.md)                                           |                                                 | <span data-ttu-id="7881e-121">Очистить сеанс присутствия приложения для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7881e-121">Clear an application's presence session for a user.</span></span>         |

## <a name="properties"></a><span data-ttu-id="7881e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="7881e-122">Properties</span></span>

| <span data-ttu-id="7881e-123">Связь</span><span class="sxs-lookup"><span data-stu-id="7881e-123">Relationship</span></span>        | <span data-ttu-id="7881e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7881e-124">Type</span></span>                                          | <span data-ttu-id="7881e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7881e-125">Description</span></span>                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7881e-126">id</span><span class="sxs-lookup"><span data-stu-id="7881e-126">id</span></span>                  | <span data-ttu-id="7881e-127">string</span><span class="sxs-lookup"><span data-stu-id="7881e-127">string</span></span>                                        | <span data-ttu-id="7881e-128">ID объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="7881e-128">The user object id</span></span>                                                                                                                                                                                                                                                                             |
| <span data-ttu-id="7881e-129">availability</span><span class="sxs-lookup"><span data-stu-id="7881e-129">availability</span></span>        | <span data-ttu-id="7881e-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7881e-130">string collection</span></span>                             | <span data-ttu-id="7881e-131">Базовые сведения о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="7881e-131">The base presence information for a user.</span></span> <span data-ttu-id="7881e-132">Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="7881e-132">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>                                                                                                           |
| <span data-ttu-id="7881e-133">действие</span><span class="sxs-lookup"><span data-stu-id="7881e-133">activity</span></span>            | <span data-ttu-id="7881e-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7881e-134">string collection</span></span>                             | <span data-ttu-id="7881e-135">Дополнительные сведения о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="7881e-135">The supplemental information to a user's availability.</span></span> <span data-ttu-id="7881e-136">Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="7881e-136">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span> |
| <span data-ttu-id="7881e-137">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="7881e-137">outOfOfficeSettings</span></span> | [<span data-ttu-id="7881e-138">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="7881e-138">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="7881e-139">Параметры вне офиса для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7881e-139">The out of office settings for a user.</span></span>                                                                                                                                                                                                                                                         |

><span data-ttu-id="7881e-140">**Примечание:** Дополнительные данные о различных состояниях присутствия см. в [Teams.](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="7881e-140">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="7881e-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="7881e-141">Relationships</span></span>

<span data-ttu-id="7881e-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7881e-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7881e-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7881e-143">JSON representation</span></span>

<span data-ttu-id="7881e-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7881e-144">The following is a JSON representation of the resource.</span></span>

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
