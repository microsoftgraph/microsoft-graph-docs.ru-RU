---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6bc92b18bd0529066ef9ade2df9c6ccee9628add
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895380"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="01122-103">Тип ресурса "Расписание"</span><span class="sxs-lookup"><span data-stu-id="01122-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01122-104">Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="01122-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="01122-105">Методы</span><span class="sxs-lookup"><span data-stu-id="01122-105">Methods</span></span>

| <span data-ttu-id="01122-106">Метод</span><span class="sxs-lookup"><span data-stu-id="01122-106">Method</span></span>       | <span data-ttu-id="01122-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01122-107">Return Type</span></span>  |<span data-ttu-id="01122-108">Описание</span><span class="sxs-lookup"><span data-stu-id="01122-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01122-109">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="01122-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="01122-110">schedule</span><span class="sxs-lookup"><span data-stu-id="01122-110">schedule</span></span>](schedule.md) | <span data-ttu-id="01122-111">Создайте или замените расписание.</span><span class="sxs-lookup"><span data-stu-id="01122-111">Create or replace a schedule.</span></span>|
|[<span data-ttu-id="01122-112">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="01122-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="01122-113">schedule</span><span class="sxs-lookup"><span data-stu-id="01122-113">schedule</span></span>](schedule.md) | <span data-ttu-id="01122-114">Получение расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-114">Get a schedule.</span></span>|
|[<span data-ttu-id="01122-115">Предоставление общего доступа</span><span class="sxs-lookup"><span data-stu-id="01122-115">Share</span></span>](../api/schedule-share.md) | <span data-ttu-id="01122-116">Нет</span><span class="sxs-lookup"><span data-stu-id="01122-116">None</span></span> | <span data-ttu-id="01122-117">Предоставьте общий доступ к диапазону расписания с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-117">Share a schedule time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="01122-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="01122-118">Properties</span></span>
|<span data-ttu-id="01122-119">Имя</span><span class="sxs-lookup"><span data-stu-id="01122-119">Name</span></span>                   |<span data-ttu-id="01122-120">Тип</span><span class="sxs-lookup"><span data-stu-id="01122-120">Type</span></span>           |<span data-ttu-id="01122-121">Описание</span><span class="sxs-lookup"><span data-stu-id="01122-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="01122-122">id</span><span class="sxs-lookup"><span data-stu-id="01122-122">id</span></span>                    |<span data-ttu-id="01122-123">string</span><span class="sxs-lookup"><span data-stu-id="01122-123">string</span></span>  |<span data-ttu-id="01122-124">Идентификатор расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-124">ID of the schedule.</span></span>|
| <span data-ttu-id="01122-125">enabled</span><span class="sxs-lookup"><span data-stu-id="01122-125">enabled</span></span>               |<span data-ttu-id="01122-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="01122-126">Boolean</span></span>    | <span data-ttu-id="01122-127">Указывает, включено ли расписание для группы.</span><span class="sxs-lookup"><span data-stu-id="01122-127">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="01122-128">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="01122-128">Required.</span></span>|
| <span data-ttu-id="01122-129">timeZone</span><span class="sxs-lookup"><span data-stu-id="01122-129">timeZone</span></span>              |<span data-ttu-id="01122-130">string</span><span class="sxs-lookup"><span data-stu-id="01122-130">string</span></span>  | <span data-ttu-id="01122-131">Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных.</span><span class="sxs-lookup"><span data-stu-id="01122-131">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="01122-132">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="01122-132">Required.</span></span>|
| <span data-ttu-id="01122-133">провисионстатус</span><span class="sxs-lookup"><span data-stu-id="01122-133">provisionStatus</span></span>       |<span data-ttu-id="01122-134">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="01122-134">operationStatus</span></span>    | <span data-ttu-id="01122-135">Состояние подготовки расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-135">The status of the schedule provisioning.</span></span> <span data-ttu-id="01122-136">`notStarted`Возможные значения: `running`,, `completed`,. `failed`</span><span class="sxs-lookup"><span data-stu-id="01122-136">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="01122-137">провисионстатускоде</span><span class="sxs-lookup"><span data-stu-id="01122-137">provisionStatusCode</span></span>   |<span data-ttu-id="01122-138">string</span><span class="sxs-lookup"><span data-stu-id="01122-138">string</span></span>  | <span data-ttu-id="01122-139">Дополнительные сведения о том, почему не удалось подготовить расписание.</span><span class="sxs-lookup"><span data-stu-id="01122-139">Additional information about why schedule provisioning failed.</span></span> |
| <span data-ttu-id="01122-140">тимеклоккенаблед</span><span class="sxs-lookup"><span data-stu-id="01122-140">timeClockEnabled</span></span>                  |<span data-ttu-id="01122-141">Логический</span><span class="sxs-lookup"><span data-stu-id="01122-141">Boolean</span></span>  | <span data-ttu-id="01122-142">Указывает, включено ли время для расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-142">Indicates whether time clock is enabled for the schedule.</span></span>             |
| <span data-ttu-id="01122-143">опеншифтсенаблед</span><span class="sxs-lookup"><span data-stu-id="01122-143">openShiftsEnabled</span></span>                 |<span data-ttu-id="01122-144">Логический</span><span class="sxs-lookup"><span data-stu-id="01122-144">Boolean</span></span>  | <span data-ttu-id="01122-145">Указывает, включены ли для расписания открытые смены.</span><span class="sxs-lookup"><span data-stu-id="01122-145">Indicates whether open shifts are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="01122-146">свапшифтсрекуестсенаблед</span><span class="sxs-lookup"><span data-stu-id="01122-146">swapShiftsRequestsEnabled</span></span>                 |<span data-ttu-id="01122-147">Логический</span><span class="sxs-lookup"><span data-stu-id="01122-147">Boolean</span></span>| <span data-ttu-id="01122-148">Указывает, включены ли запросы замены сдвига для расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-148">Indicates whether swap shifts requests are enabled for the schedule.</span></span>             |
| <span data-ttu-id="01122-149">оффершифтрекуестсенаблед</span><span class="sxs-lookup"><span data-stu-id="01122-149">offerShiftRequestsEnabled</span></span>                 |<span data-ttu-id="01122-150">Логический</span><span class="sxs-lookup"><span data-stu-id="01122-150">Boolean</span></span>  | <span data-ttu-id="01122-151">Указывает, включены ли запросы на смену для расписания.</span><span class="sxs-lookup"><span data-stu-id="01122-151">Indicates whether offer shift requests are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="01122-152">тимеоффрекуестсенаблед</span><span class="sxs-lookup"><span data-stu-id="01122-152">timeOffRequestsEnabled</span></span>                    |<span data-ttu-id="01122-153">Логический</span><span class="sxs-lookup"><span data-stu-id="01122-153">Boolean</span></span> | <span data-ttu-id="01122-154">Указывает, включены ли для расписания запросы по времени.</span><span class="sxs-lookup"><span data-stu-id="01122-154">Indicates whether time off requests are enabled for the schedule.</span></span>             | 



## <a name="relationships"></a><span data-ttu-id="01122-155">Связи</span><span class="sxs-lookup"><span data-stu-id="01122-155">Relationships</span></span>
|<span data-ttu-id="01122-156">Имя</span><span class="sxs-lookup"><span data-stu-id="01122-156">Name</span></span>                   |<span data-ttu-id="01122-157">Тип</span><span class="sxs-lookup"><span data-stu-id="01122-157">Type</span></span>           |<span data-ttu-id="01122-158">Описание</span><span class="sxs-lookup"><span data-stu-id="01122-158">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="01122-159">Сдвигает</span><span class="sxs-lookup"><span data-stu-id="01122-159">shifts</span></span>   | <span data-ttu-id="01122-160">Коллекция [shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="01122-160">[shift](shift.md) collection</span></span>  | <span data-ttu-id="01122-161">Смены в расписании.</span><span class="sxs-lookup"><span data-stu-id="01122-161">The shifts in the schedule.</span></span> |
| <span data-ttu-id="01122-162">тимесофф</span><span class="sxs-lookup"><span data-stu-id="01122-162">timesOff</span></span>   |<span data-ttu-id="01122-163">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="01122-163">[timeOff](timeoff.md) collection</span></span>  | <span data-ttu-id="01122-164">Экземпляры повременных вызовов в расписании.</span><span class="sxs-lookup"><span data-stu-id="01122-164">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="01122-165">тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="01122-165">timeOffReasons</span></span>   |<span data-ttu-id="01122-166">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="01122-166">[timeOffReason](timeoffreason.md) collection</span></span>  | <span data-ttu-id="01122-167">Набор причин незапланированного времени.</span><span class="sxs-lookup"><span data-stu-id="01122-167">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="01122-168">счедулингграупс</span><span class="sxs-lookup"><span data-stu-id="01122-168">schedulingGroups</span></span>   |<span data-ttu-id="01122-169">Коллекция [schedulingGroup](schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="01122-169">[schedulingGroup](schedulinggroup.md) collection</span></span>  | <span data-ttu-id="01122-170">Логическая группа пользователей в расписании (обычно по роли).</span><span class="sxs-lookup"><span data-stu-id="01122-170">The logical grouping of users in the schedule (usually by role).</span></span> |
| <span data-ttu-id="01122-171">опеншифтс</span><span class="sxs-lookup"><span data-stu-id="01122-171">openshifts</span></span>   |<span data-ttu-id="01122-172">Коллекция [опеншифт](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="01122-172">[openShift](openshift.md) collection</span></span> | <span data-ttu-id="01122-173">Набор смен, открытых в группе планирования, в расписании.</span><span class="sxs-lookup"><span data-stu-id="01122-173">The set of open shifts in a scheduling group in the schedule.</span></span> |
| <span data-ttu-id="01122-174">воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="01122-174">workforceintegrations</span></span>   |<span data-ttu-id="01122-175">Коллекция [воркфорцеинтегратион](workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="01122-175">[workforceIntegration](workforceintegration.md) collection</span></span>  | <span data-ttu-id="01122-176">Экземпляр интеграции сотрудников для группы с исходящим трафиком в синхронных уведомлениях об изменениях (для поддерживаемых сущностей).</span><span class="sxs-lookup"><span data-stu-id="01122-176">An instance of a workforce integration per team with outbound data flow on synchronous change notifications (for supported entities).</span></span> |
| <span data-ttu-id="01122-177">свапшифтчанжерекуестс</span><span class="sxs-lookup"><span data-stu-id="01122-177">swapshiftchangerequests</span></span>   |<span data-ttu-id="01122-178">Коллекция [свапшифтсчанжерекуест](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="01122-178">[swapShiftsChangeRequest](swapshiftschangerequest.md) collection</span></span>  | <span data-ttu-id="01122-179">Запросы на замену для сдвигов в расписании.</span><span class="sxs-lookup"><span data-stu-id="01122-179">The swap requests for shifts in the schedule.</span></span> |
| <span data-ttu-id="01122-180">опеншифтчанжерекуестс</span><span class="sxs-lookup"><span data-stu-id="01122-180">openshiftchangerequests</span></span>   |<span data-ttu-id="01122-181">Коллекция [опеншифтчанжерекуест](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="01122-181">[openShiftChangeRequest](openshiftchangerequest.md) collection</span></span>  | <span data-ttu-id="01122-182">Запросы на открытие с открытым сдвигом по расписанию.</span><span class="sxs-lookup"><span data-stu-id="01122-182">The open shift requests in the schedule.</span></span> |
| <span data-ttu-id="01122-183">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="01122-183">timeoffrequest</span></span>   |<span data-ttu-id="01122-184">Коллекция [тимеоффрекуест](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="01122-184">[timeOffRequest](timeoffrequest.md) collection</span></span>  | <span data-ttu-id="01122-185">Время, в течение которого запросы отменяются по расписанию.</span><span class="sxs-lookup"><span data-stu-id="01122-185">The time off requests in the schedule.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="01122-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01122-186">JSON representation</span></span>

<span data-ttu-id="01122-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01122-187">The following is a JSON representation of the resource.</span></span>

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
