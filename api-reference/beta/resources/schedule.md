---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563151"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="670e1-103">Тип ресурса "Расписание"</span><span class="sxs-lookup"><span data-stu-id="670e1-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="670e1-104">Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="670e1-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="670e1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="670e1-105">Methods</span></span>

| <span data-ttu-id="670e1-106">Метод</span><span class="sxs-lookup"><span data-stu-id="670e1-106">Method</span></span>       | <span data-ttu-id="670e1-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="670e1-107">Return Type</span></span>  |<span data-ttu-id="670e1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="670e1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="670e1-109">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="670e1-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="670e1-110">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="670e1-110">schedule</span></span>](schedule.md) | <span data-ttu-id="670e1-111">Создание или замена `schedule`.</span><span class="sxs-lookup"><span data-stu-id="670e1-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="670e1-112">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="670e1-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="670e1-113">Диспетчер</span><span class="sxs-lookup"><span data-stu-id="670e1-113">schedule</span></span>](schedule.md) | <span data-ttu-id="670e1-114">Получение `schedule`.</span><span class="sxs-lookup"><span data-stu-id="670e1-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="670e1-115">share</span><span class="sxs-lookup"><span data-stu-id="670e1-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="670e1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="670e1-116">None</span></span> | <span data-ttu-id="670e1-117">Предоставьте общий `schedule` доступ к диапазону времени с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="670e1-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="670e1-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="670e1-118">Properties</span></span>
|<span data-ttu-id="670e1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="670e1-119">Name</span></span>                   |<span data-ttu-id="670e1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="670e1-120">Type</span></span>           |<span data-ttu-id="670e1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="670e1-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="670e1-122">id</span><span class="sxs-lookup"><span data-stu-id="670e1-122">id</span></span>                    |`string`  |<span data-ttu-id="670e1-123">Идентификатор объекта `schedule`.</span><span class="sxs-lookup"><span data-stu-id="670e1-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="670e1-124">enabled</span><span class="sxs-lookup"><span data-stu-id="670e1-124">enabled</span></span>               |`bool`    | <span data-ttu-id="670e1-125">Указывает, включено ли расписание для группы.</span><span class="sxs-lookup"><span data-stu-id="670e1-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="670e1-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="670e1-126">Required.</span></span>|
| <span data-ttu-id="670e1-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="670e1-127">timeZone</span></span>              |`string`  | <span data-ttu-id="670e1-128">Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных.</span><span class="sxs-lookup"><span data-stu-id="670e1-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="670e1-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="670e1-129">Required.</span></span>|
| <span data-ttu-id="670e1-130">Провисионстатус</span><span class="sxs-lookup"><span data-stu-id="670e1-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="670e1-131">Состояние подготовки расписания.</span><span class="sxs-lookup"><span data-stu-id="670e1-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="670e1-132">Провисионстатускоде</span><span class="sxs-lookup"><span data-stu-id="670e1-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="670e1-133">Дополнительные сведения о том, почему не удалось подготовить расписание.</span><span class="sxs-lookup"><span data-stu-id="670e1-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="670e1-134">Связи</span><span class="sxs-lookup"><span data-stu-id="670e1-134">Relationships</span></span>
|<span data-ttu-id="670e1-135">Имя</span><span class="sxs-lookup"><span data-stu-id="670e1-135">Name</span></span>                   |<span data-ttu-id="670e1-136">Тип</span><span class="sxs-lookup"><span data-stu-id="670e1-136">Type</span></span>           |<span data-ttu-id="670e1-137">Описание</span><span class="sxs-lookup"><span data-stu-id="670e1-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="670e1-138">Сдвигает</span><span class="sxs-lookup"><span data-stu-id="670e1-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="670e1-139">Смены в расписании.</span><span class="sxs-lookup"><span data-stu-id="670e1-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="670e1-140">Тимесофф</span><span class="sxs-lookup"><span data-stu-id="670e1-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="670e1-141">Экземпляры повременных вызовов в расписании.</span><span class="sxs-lookup"><span data-stu-id="670e1-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="670e1-142">Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="670e1-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="670e1-143">Набор причин незапланированного времени.</span><span class="sxs-lookup"><span data-stu-id="670e1-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="670e1-144">Счедулингграупс</span><span class="sxs-lookup"><span data-stu-id="670e1-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="670e1-145">Логическая группа пользователей в расписании (обычно по роли).</span><span class="sxs-lookup"><span data-stu-id="670e1-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="670e1-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="670e1-146">JSON representation</span></span>

<span data-ttu-id="670e1-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="670e1-147">Here is a JSON representation of the resource.</span></span>

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
