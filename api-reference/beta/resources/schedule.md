---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48b3b5c118a39442469bc6155068664fcebe0ec2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343523"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="0883f-103">Тип ресурса "Расписание"</span><span class="sxs-lookup"><span data-stu-id="0883f-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0883f-104">Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0883f-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="0883f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0883f-105">Methods</span></span>

| <span data-ttu-id="0883f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0883f-106">Method</span></span>       | <span data-ttu-id="0883f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0883f-107">Return Type</span></span>  |<span data-ttu-id="0883f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0883f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0883f-109">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="0883f-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="0883f-110">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="0883f-110">schedule</span></span>](schedule.md) | <span data-ttu-id="0883f-111">Создание или замена `schedule`.</span><span class="sxs-lookup"><span data-stu-id="0883f-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="0883f-112">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="0883f-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="0883f-113">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="0883f-113">schedule</span></span>](schedule.md) | <span data-ttu-id="0883f-114">Получение `schedule`.</span><span class="sxs-lookup"><span data-stu-id="0883f-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="0883f-115">share</span><span class="sxs-lookup"><span data-stu-id="0883f-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="0883f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="0883f-116">None</span></span> | <span data-ttu-id="0883f-117">Предоставьте общий `schedule` доступ к диапазону времени с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="0883f-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="0883f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0883f-118">Properties</span></span>
|<span data-ttu-id="0883f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0883f-119">Name</span></span>                   |<span data-ttu-id="0883f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0883f-120">Type</span></span>           |<span data-ttu-id="0883f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0883f-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0883f-122">id</span><span class="sxs-lookup"><span data-stu-id="0883f-122">id</span></span>                    |`string`  |<span data-ttu-id="0883f-123">Идентификатор объекта `schedule`.</span><span class="sxs-lookup"><span data-stu-id="0883f-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="0883f-124">enabled</span><span class="sxs-lookup"><span data-stu-id="0883f-124">enabled</span></span>               |`bool`    | <span data-ttu-id="0883f-125">Указывает, включено ли расписание для группы.</span><span class="sxs-lookup"><span data-stu-id="0883f-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="0883f-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0883f-126">Required.</span></span>|
| <span data-ttu-id="0883f-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="0883f-127">timeZone</span></span>              |`string`  | <span data-ttu-id="0883f-128">Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных.</span><span class="sxs-lookup"><span data-stu-id="0883f-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="0883f-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0883f-129">Required.</span></span>|
| <span data-ttu-id="0883f-130">Провисионстатус</span><span class="sxs-lookup"><span data-stu-id="0883f-130">provisionStatus</span></span>       |`operationStatus`    | <span data-ttu-id="0883f-131">Состояние подготовки расписания.</span><span class="sxs-lookup"><span data-stu-id="0883f-131">The status of the schedule provisioning.</span></span> <span data-ttu-id="0883f-132">`notStarted`Возможные значения: `running`,, `completed`,. `failed`</span><span class="sxs-lookup"><span data-stu-id="0883f-132">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="0883f-133">Провисионстатускоде</span><span class="sxs-lookup"><span data-stu-id="0883f-133">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="0883f-134">Дополнительные сведения о том, почему не удалось подготовить расписание.</span><span class="sxs-lookup"><span data-stu-id="0883f-134">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="0883f-135">Связи</span><span class="sxs-lookup"><span data-stu-id="0883f-135">Relationships</span></span>
|<span data-ttu-id="0883f-136">Имя</span><span class="sxs-lookup"><span data-stu-id="0883f-136">Name</span></span>                   |<span data-ttu-id="0883f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0883f-137">Type</span></span>           |<span data-ttu-id="0883f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0883f-138">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0883f-139">Сдвигает</span><span class="sxs-lookup"><span data-stu-id="0883f-139">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="0883f-140">Смены в расписании.</span><span class="sxs-lookup"><span data-stu-id="0883f-140">The shifts in the schedule.</span></span> |
| <span data-ttu-id="0883f-141">Тимесофф</span><span class="sxs-lookup"><span data-stu-id="0883f-141">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="0883f-142">Экземпляры повременных вызовов в расписании.</span><span class="sxs-lookup"><span data-stu-id="0883f-142">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="0883f-143">Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="0883f-143">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="0883f-144">Набор причин незапланированного времени.</span><span class="sxs-lookup"><span data-stu-id="0883f-144">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="0883f-145">Счедулингграупс</span><span class="sxs-lookup"><span data-stu-id="0883f-145">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="0883f-146">Логическая группа пользователей в расписании (обычно по роли).</span><span class="sxs-lookup"><span data-stu-id="0883f-146">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0883f-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0883f-147">JSON representation</span></span>

<span data-ttu-id="0883f-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0883f-148">Here is a JSON representation of the resource.</span></span>

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
