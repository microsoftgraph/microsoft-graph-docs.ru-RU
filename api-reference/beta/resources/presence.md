---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 797ddac8bc582cd5e5d4d51e0e1ad94645c3c1e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521574"
---
# <a name="presence-resource-type"></a><span data-ttu-id="16b05-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="16b05-103">presence resource type</span></span>

<span data-ttu-id="16b05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b05-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16b05-105">Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.</span><span class="sxs-lookup"><span data-stu-id="16b05-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="16b05-106">**Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="16b05-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

## <a name="methods"></a><span data-ttu-id="16b05-107">Методы</span><span class="sxs-lookup"><span data-stu-id="16b05-107">Methods</span></span>

| <span data-ttu-id="16b05-108">Метод</span><span class="sxs-lookup"><span data-stu-id="16b05-108">Method</span></span>                                                            | <span data-ttu-id="16b05-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16b05-109">Return Type</span></span>                                       | <span data-ttu-id="16b05-110">Описание</span><span class="sxs-lookup"><span data-stu-id="16b05-110">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="16b05-111">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="16b05-111">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="16b05-112">presence</span><span class="sxs-lookup"><span data-stu-id="16b05-112">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="16b05-113">Получение сведений о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="16b05-113">Get a user's presence information.</span></span>
| [<span data-ttu-id="16b05-114">Получение сведений о присутствии нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="16b05-114">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="16b05-115">Коллекция [присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="16b05-115">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="16b05-116">Получение сведений о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="16b05-116">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="16b05-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="16b05-117">Properties</span></span>

| <span data-ttu-id="16b05-118">Связь</span><span class="sxs-lookup"><span data-stu-id="16b05-118">Relationship</span></span>        | <span data-ttu-id="16b05-119">Тип</span><span class="sxs-lookup"><span data-stu-id="16b05-119">Type</span></span>                                                 | <span data-ttu-id="16b05-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16b05-120">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="16b05-121">id</span><span class="sxs-lookup"><span data-stu-id="16b05-121">id</span></span>    |  <span data-ttu-id="16b05-122">string</span><span class="sxs-lookup"><span data-stu-id="16b05-122">string</span></span>     |  <span data-ttu-id="16b05-123">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="16b05-123">The user object id</span></span>   |
|<span data-ttu-id="16b05-124">availability</span><span class="sxs-lookup"><span data-stu-id="16b05-124">availability</span></span>    |  <span data-ttu-id="16b05-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="16b05-125">string collection</span></span>   |   <span data-ttu-id="16b05-126">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="16b05-126">The base presence information for a user.</span></span> <span data-ttu-id="16b05-127">Возможные значения: `Available`, `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`,,,, `Offline`,`PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="16b05-127">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="16b05-128">activity</span><span class="sxs-lookup"><span data-stu-id="16b05-128">activity</span></span>    |  <span data-ttu-id="16b05-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="16b05-129">string collection</span></span>      |    <span data-ttu-id="16b05-130">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="16b05-130">The supplemental information to a user's availability.</span></span> <span data-ttu-id="16b05-131">Возможные значения: `Available`, `Away`, `BeRightBack`,`Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `PresenceUnknown``Presenting` `UrgentInterruptionsOnly`,,,,,,,,,,. `Inactive``InAMeeting` `Offline` `OffWork``OutOfOffice`</span><span class="sxs-lookup"><span data-stu-id="16b05-131">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="16b05-132">**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="16b05-132">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="16b05-133">Связи</span><span class="sxs-lookup"><span data-stu-id="16b05-133">Relationships</span></span>

<span data-ttu-id="16b05-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="16b05-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16b05-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="16b05-135">JSON representation</span></span>

<span data-ttu-id="16b05-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16b05-136">The following is a JSON representation of the resource.</span></span>

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
