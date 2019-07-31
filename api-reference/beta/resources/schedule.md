---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a404c620b20cfcb69076ecc3bac25f907a12216c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965329"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="27f3c-103">Тип ресурса "Расписание"</span><span class="sxs-lookup"><span data-stu-id="27f3c-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27f3c-104">Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="27f3c-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="27f3c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="27f3c-105">Methods</span></span>

| <span data-ttu-id="27f3c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="27f3c-106">Method</span></span>       | <span data-ttu-id="27f3c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27f3c-107">Return Type</span></span>  |<span data-ttu-id="27f3c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27f3c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27f3c-109">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="27f3c-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="27f3c-110">schedule</span><span class="sxs-lookup"><span data-stu-id="27f3c-110">schedule</span></span>](schedule.md) | <span data-ttu-id="27f3c-111">Создание или замена `schedule`.</span><span class="sxs-lookup"><span data-stu-id="27f3c-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="27f3c-112">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="27f3c-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="27f3c-113">schedule</span><span class="sxs-lookup"><span data-stu-id="27f3c-113">schedule</span></span>](schedule.md) | <span data-ttu-id="27f3c-114">Получение `schedule`.</span><span class="sxs-lookup"><span data-stu-id="27f3c-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="27f3c-115">share</span><span class="sxs-lookup"><span data-stu-id="27f3c-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="27f3c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="27f3c-116">None</span></span> | <span data-ttu-id="27f3c-117">Предоставьте общий `schedule` доступ к диапазону времени с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="27f3c-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="27f3c-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="27f3c-118">Properties</span></span>
|<span data-ttu-id="27f3c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27f3c-119">Name</span></span>                   |<span data-ttu-id="27f3c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="27f3c-120">Type</span></span>           |<span data-ttu-id="27f3c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="27f3c-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="27f3c-122">id</span><span class="sxs-lookup"><span data-stu-id="27f3c-122">id</span></span>                    |`string`  |<span data-ttu-id="27f3c-123">Идентификатор объекта `schedule`.</span><span class="sxs-lookup"><span data-stu-id="27f3c-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="27f3c-124">enabled</span><span class="sxs-lookup"><span data-stu-id="27f3c-124">enabled</span></span>               |`bool`    | <span data-ttu-id="27f3c-125">Указывает, включено ли расписание для группы.</span><span class="sxs-lookup"><span data-stu-id="27f3c-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="27f3c-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="27f3c-126">Required.</span></span>|
| <span data-ttu-id="27f3c-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="27f3c-127">timeZone</span></span>              |`string`  | <span data-ttu-id="27f3c-128">Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных.</span><span class="sxs-lookup"><span data-stu-id="27f3c-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="27f3c-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="27f3c-129">Required.</span></span>|
| <span data-ttu-id="27f3c-130">Провисионстатус</span><span class="sxs-lookup"><span data-stu-id="27f3c-130">provisionStatus</span></span>       |`operationStatus`    | <span data-ttu-id="27f3c-131">Состояние подготовки расписания.</span><span class="sxs-lookup"><span data-stu-id="27f3c-131">The status of the schedule provisioning.</span></span> <span data-ttu-id="27f3c-132">`notStarted`Возможные значения: `running`,, `completed`,. `failed`</span><span class="sxs-lookup"><span data-stu-id="27f3c-132">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="27f3c-133">Провисионстатускоде</span><span class="sxs-lookup"><span data-stu-id="27f3c-133">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="27f3c-134">Дополнительные сведения о том, почему не удалось подготовить расписание.</span><span class="sxs-lookup"><span data-stu-id="27f3c-134">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="27f3c-135">Связи</span><span class="sxs-lookup"><span data-stu-id="27f3c-135">Relationships</span></span>
|<span data-ttu-id="27f3c-136">Имя</span><span class="sxs-lookup"><span data-stu-id="27f3c-136">Name</span></span>                   |<span data-ttu-id="27f3c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="27f3c-137">Type</span></span>           |<span data-ttu-id="27f3c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="27f3c-138">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="27f3c-139">Сдвигает</span><span class="sxs-lookup"><span data-stu-id="27f3c-139">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="27f3c-140">Смены в расписании.</span><span class="sxs-lookup"><span data-stu-id="27f3c-140">The shifts in the schedule.</span></span> |
| <span data-ttu-id="27f3c-141">Тимесофф</span><span class="sxs-lookup"><span data-stu-id="27f3c-141">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="27f3c-142">Экземпляры повременных вызовов в расписании.</span><span class="sxs-lookup"><span data-stu-id="27f3c-142">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="27f3c-143">Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="27f3c-143">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="27f3c-144">Набор причин незапланированного времени.</span><span class="sxs-lookup"><span data-stu-id="27f3c-144">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="27f3c-145">Счедулингграупс</span><span class="sxs-lookup"><span data-stu-id="27f3c-145">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="27f3c-146">Логическая группа пользователей в расписании (обычно по роли).</span><span class="sxs-lookup"><span data-stu-id="27f3c-146">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="27f3c-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27f3c-147">JSON representation</span></span>

<span data-ttu-id="27f3c-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f3c-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
