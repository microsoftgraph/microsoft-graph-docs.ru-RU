---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 48574baf0969077add921d6b4c9d52dd2d5d4906
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913571"
---
# <a name="presence-resource-type"></a><span data-ttu-id="9d5c4-103">Тип ресурса присутствия</span><span class="sxs-lookup"><span data-stu-id="9d5c4-103">presence resource type</span></span>

<span data-ttu-id="9d5c4-104">Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-104">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="9d5c4-105">**Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-105">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

## <a name="methods"></a><span data-ttu-id="9d5c4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9d5c4-106">Methods</span></span>

| <span data-ttu-id="9d5c4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9d5c4-107">Method</span></span>                                                            | <span data-ttu-id="9d5c4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9d5c4-108">Return Type</span></span>                                       | <span data-ttu-id="9d5c4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d5c4-109">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="9d5c4-110">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="9d5c4-110">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="9d5c4-111">presence</span><span class="sxs-lookup"><span data-stu-id="9d5c4-111">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="9d5c4-112">Получение сведений о присутствии пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-112">Get a user's presence information.</span></span>
| [<span data-ttu-id="9d5c4-113">Получение сведений о присутствии нескольких пользователей</span><span class="sxs-lookup"><span data-stu-id="9d5c4-113">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="9d5c4-114">Коллекция [присутствия](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="9d5c4-114">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="9d5c4-115">Получение сведений о присутствии для нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-115">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="9d5c4-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d5c4-116">Properties</span></span>

| <span data-ttu-id="9d5c4-117">Отношение</span><span class="sxs-lookup"><span data-stu-id="9d5c4-117">Relationship</span></span>        | <span data-ttu-id="9d5c4-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9d5c4-118">Type</span></span>                                                 | <span data-ttu-id="9d5c4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9d5c4-119">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="9d5c4-120">id</span><span class="sxs-lookup"><span data-stu-id="9d5c4-120">id</span></span>    |  <span data-ttu-id="9d5c4-121">string</span><span class="sxs-lookup"><span data-stu-id="9d5c4-121">string</span></span>     |  <span data-ttu-id="9d5c4-122">Идентификатор объекта пользователя</span><span class="sxs-lookup"><span data-stu-id="9d5c4-122">The user object id</span></span>   |
|<span data-ttu-id="9d5c4-123">availability</span><span class="sxs-lookup"><span data-stu-id="9d5c4-123">availability</span></span>    |  <span data-ttu-id="9d5c4-124">string collection</span><span class="sxs-lookup"><span data-stu-id="9d5c4-124">string collection</span></span>   |   <span data-ttu-id="9d5c4-125">Базовые сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-125">The base presence information for a user.</span></span> <span data-ttu-id="9d5c4-126">Возможные значения: `Available`, `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`,,,, `Offline`,`PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="9d5c4-126">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="9d5c4-127">activity</span><span class="sxs-lookup"><span data-stu-id="9d5c4-127">activity</span></span>    |  <span data-ttu-id="9d5c4-128">string collection</span><span class="sxs-lookup"><span data-stu-id="9d5c4-128">string collection</span></span>      |    <span data-ttu-id="9d5c4-129">Дополнительная информация о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-129">The supplemental information to a user's availability.</span></span> <span data-ttu-id="9d5c4-130">Возможные значения: `Available`, `Away`, `BeRightBack`,`Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `PresenceUnknown``Presenting` `UrgentInterruptionsOnly`,,,,,,,,,,. `Inactive``InAMeeting` `Offline` `OffWork``OutOfOffice`</span><span class="sxs-lookup"><span data-stu-id="9d5c4-130">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="9d5c4-131">**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="9d5c4-131">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="9d5c4-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="9d5c4-132">Relationships</span></span>

<span data-ttu-id="9d5c4-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d5c4-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9d5c4-134">JSON representation</span></span>

<span data-ttu-id="9d5c4-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d5c4-135">The following is a JSON representation of the resource.</span></span>

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
