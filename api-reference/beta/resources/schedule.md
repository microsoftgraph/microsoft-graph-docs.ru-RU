---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657513"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="3ade7-103">Тип ресурса "Расписание"</span><span class="sxs-lookup"><span data-stu-id="3ade7-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ade7-104">Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3ade7-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="3ade7-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3ade7-105">Methods</span></span>

| <span data-ttu-id="3ade7-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3ade7-106">Method</span></span>       | <span data-ttu-id="3ade7-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ade7-107">Return Type</span></span>  |<span data-ttu-id="3ade7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ade7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ade7-109">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="3ade7-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="3ade7-110">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="3ade7-110">schedule</span></span>](schedule.md) | <span data-ttu-id="3ade7-111">Создание или замена `schedule`.</span><span class="sxs-lookup"><span data-stu-id="3ade7-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="3ade7-112">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="3ade7-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="3ade7-113">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="3ade7-113">schedule</span></span>](schedule.md) | <span data-ttu-id="3ade7-114">Получение `schedule`.</span><span class="sxs-lookup"><span data-stu-id="3ade7-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="3ade7-115">share</span><span class="sxs-lookup"><span data-stu-id="3ade7-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="3ade7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3ade7-116">None</span></span> | <span data-ttu-id="3ade7-117">Предоставьте общий `schedule` доступ к диапазону времени с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="3ade7-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ade7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ade7-118">Properties</span></span>
|<span data-ttu-id="3ade7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3ade7-119">Name</span></span>                   |<span data-ttu-id="3ade7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3ade7-120">Type</span></span>           |<span data-ttu-id="3ade7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3ade7-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3ade7-122">id</span><span class="sxs-lookup"><span data-stu-id="3ade7-122">id</span></span>                    |`string`  |<span data-ttu-id="3ade7-123">Идентификатор объекта `schedule`.</span><span class="sxs-lookup"><span data-stu-id="3ade7-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="3ade7-124">enabled</span><span class="sxs-lookup"><span data-stu-id="3ade7-124">enabled</span></span>               |`bool`    | <span data-ttu-id="3ade7-125">Указывает, включено ли расписание для группы.</span><span class="sxs-lookup"><span data-stu-id="3ade7-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="3ade7-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ade7-126">Required.</span></span>|
| <span data-ttu-id="3ade7-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="3ade7-127">timeZone</span></span>              |`string`  | <span data-ttu-id="3ade7-128">Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных.</span><span class="sxs-lookup"><span data-stu-id="3ade7-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="3ade7-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ade7-129">Required.</span></span>|
| <span data-ttu-id="3ade7-130">Провисионстатус</span><span class="sxs-lookup"><span data-stu-id="3ade7-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="3ade7-131">Состояние подготовки расписания.</span><span class="sxs-lookup"><span data-stu-id="3ade7-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="3ade7-132">Провисионстатускоде</span><span class="sxs-lookup"><span data-stu-id="3ade7-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="3ade7-133">Дополнительные сведения о том, почему не удалось подготовить расписание.</span><span class="sxs-lookup"><span data-stu-id="3ade7-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="3ade7-134">Связи</span><span class="sxs-lookup"><span data-stu-id="3ade7-134">Relationships</span></span>
|<span data-ttu-id="3ade7-135">Имя</span><span class="sxs-lookup"><span data-stu-id="3ade7-135">Name</span></span>                   |<span data-ttu-id="3ade7-136">Тип</span><span class="sxs-lookup"><span data-stu-id="3ade7-136">Type</span></span>           |<span data-ttu-id="3ade7-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3ade7-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3ade7-138">Сдвигает</span><span class="sxs-lookup"><span data-stu-id="3ade7-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="3ade7-139">Смены в расписании.</span><span class="sxs-lookup"><span data-stu-id="3ade7-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="3ade7-140">Тимесофф</span><span class="sxs-lookup"><span data-stu-id="3ade7-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="3ade7-141">Экземпляры повременных вызовов в расписании.</span><span class="sxs-lookup"><span data-stu-id="3ade7-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="3ade7-142">Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="3ade7-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="3ade7-143">Набор причин незапланированного времени.</span><span class="sxs-lookup"><span data-stu-id="3ade7-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="3ade7-144">Счедулингграупс</span><span class="sxs-lookup"><span data-stu-id="3ade7-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="3ade7-145">Логическая группа пользователей в расписании (обычно по роли).</span><span class="sxs-lookup"><span data-stu-id="3ade7-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3ade7-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ade7-146">JSON representation</span></span>

<span data-ttu-id="3ade7-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ade7-147">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
