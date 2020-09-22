---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a589d63c59636db385bafb04a8c646dc2dc6c030
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037061"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="4cb2a-103">Тип ресурса "Расписание"</span><span class="sxs-lookup"><span data-stu-id="4cb2a-103">schedule resource type</span></span>

<span data-ttu-id="4cb2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cb2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cb2a-105">Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4cb2a-105">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="4cb2a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4cb2a-106">Methods</span></span>

| <span data-ttu-id="4cb2a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4cb2a-107">Method</span></span>       | <span data-ttu-id="4cb2a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4cb2a-108">Return Type</span></span>  |<span data-ttu-id="4cb2a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb2a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4cb2a-110">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="4cb2a-110">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="4cb2a-111">schedule</span><span class="sxs-lookup"><span data-stu-id="4cb2a-111">schedule</span></span>](schedule.md) | <span data-ttu-id="4cb2a-112">Создайте или замените расписание.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-112">Create or replace a schedule.</span></span>|
|[<span data-ttu-id="4cb2a-113">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="4cb2a-113">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="4cb2a-114">schedule</span><span class="sxs-lookup"><span data-stu-id="4cb2a-114">schedule</span></span>](schedule.md) | <span data-ttu-id="4cb2a-115">Получение расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-115">Get a schedule.</span></span>|
|[<span data-ttu-id="4cb2a-116">Предоставление общего доступа</span><span class="sxs-lookup"><span data-stu-id="4cb2a-116">Share</span></span>](../api/schedule-share.md) | <span data-ttu-id="4cb2a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4cb2a-117">None</span></span> | <span data-ttu-id="4cb2a-118">Предоставьте общий доступ к диапазону расписания с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-118">Share a schedule time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="4cb2a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cb2a-119">Properties</span></span>
|<span data-ttu-id="4cb2a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4cb2a-120">Name</span></span>                   |<span data-ttu-id="4cb2a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb2a-121">Type</span></span>           |<span data-ttu-id="4cb2a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb2a-122">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4cb2a-123">id</span><span class="sxs-lookup"><span data-stu-id="4cb2a-123">id</span></span>                    |<span data-ttu-id="4cb2a-124">string</span><span class="sxs-lookup"><span data-stu-id="4cb2a-124">string</span></span>  |<span data-ttu-id="4cb2a-125">Идентификатор расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-125">ID of the schedule.</span></span>|
| <span data-ttu-id="4cb2a-126">enabled</span><span class="sxs-lookup"><span data-stu-id="4cb2a-126">enabled</span></span>               |<span data-ttu-id="4cb2a-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb2a-127">Boolean</span></span>    | <span data-ttu-id="4cb2a-128">Указывает, включено ли расписание для группы.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-128">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="4cb2a-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-129">Required.</span></span>|
| <span data-ttu-id="4cb2a-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="4cb2a-130">timeZone</span></span>              |<span data-ttu-id="4cb2a-131">string</span><span class="sxs-lookup"><span data-stu-id="4cb2a-131">string</span></span>  | <span data-ttu-id="4cb2a-132">Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-132">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="4cb2a-133">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-133">Required.</span></span>|
| <span data-ttu-id="4cb2a-134">провисионстатус</span><span class="sxs-lookup"><span data-stu-id="4cb2a-134">provisionStatus</span></span>       |<span data-ttu-id="4cb2a-135">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="4cb2a-135">operationStatus</span></span>    | <span data-ttu-id="4cb2a-136">Состояние подготовки расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-136">The status of the schedule provisioning.</span></span> <span data-ttu-id="4cb2a-137">Возможные значения: `notStarted` ,, `running` `completed` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="4cb2a-137">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="4cb2a-138">провисионстатускоде</span><span class="sxs-lookup"><span data-stu-id="4cb2a-138">provisionStatusCode</span></span>   |<span data-ttu-id="4cb2a-139">string</span><span class="sxs-lookup"><span data-stu-id="4cb2a-139">string</span></span>  | <span data-ttu-id="4cb2a-140">Дополнительные сведения о том, почему не удалось подготовить расписание.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-140">Additional information about why schedule provisioning failed.</span></span> |
| <span data-ttu-id="4cb2a-141">тимеклоккенаблед</span><span class="sxs-lookup"><span data-stu-id="4cb2a-141">timeClockEnabled</span></span>                  |<span data-ttu-id="4cb2a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb2a-142">Boolean</span></span>  | <span data-ttu-id="4cb2a-143">Указывает, включено ли время для расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-143">Indicates whether time clock is enabled for the schedule.</span></span>             |
| <span data-ttu-id="4cb2a-144">опеншифтсенаблед</span><span class="sxs-lookup"><span data-stu-id="4cb2a-144">openShiftsEnabled</span></span>                 |<span data-ttu-id="4cb2a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb2a-145">Boolean</span></span>  | <span data-ttu-id="4cb2a-146">Указывает, включены ли для расписания открытые смены.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-146">Indicates whether open shifts are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="4cb2a-147">свапшифтсрекуестсенаблед</span><span class="sxs-lookup"><span data-stu-id="4cb2a-147">swapShiftsRequestsEnabled</span></span>                 |<span data-ttu-id="4cb2a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb2a-148">Boolean</span></span>| <span data-ttu-id="4cb2a-149">Указывает, включены ли запросы замены сдвига для расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-149">Indicates whether swap shifts requests are enabled for the schedule.</span></span>             |
| <span data-ttu-id="4cb2a-150">оффершифтрекуестсенаблед</span><span class="sxs-lookup"><span data-stu-id="4cb2a-150">offerShiftRequestsEnabled</span></span>                 |<span data-ttu-id="4cb2a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb2a-151">Boolean</span></span>  | <span data-ttu-id="4cb2a-152">Указывает, включены ли запросы на смену для расписания.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-152">Indicates whether offer shift requests are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="4cb2a-153">тимеоффрекуестсенаблед</span><span class="sxs-lookup"><span data-stu-id="4cb2a-153">timeOffRequestsEnabled</span></span>                    |<span data-ttu-id="4cb2a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cb2a-154">Boolean</span></span> | <span data-ttu-id="4cb2a-155">Указывает, включены ли для расписания запросы по времени.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-155">Indicates whether time off requests are enabled for the schedule.</span></span>             | 



## <a name="relationships"></a><span data-ttu-id="4cb2a-156">Связи</span><span class="sxs-lookup"><span data-stu-id="4cb2a-156">Relationships</span></span>
|<span data-ttu-id="4cb2a-157">Имя</span><span class="sxs-lookup"><span data-stu-id="4cb2a-157">Name</span></span>                   |<span data-ttu-id="4cb2a-158">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb2a-158">Type</span></span>           |<span data-ttu-id="4cb2a-159">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb2a-159">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4cb2a-160">Сдвигает</span><span class="sxs-lookup"><span data-stu-id="4cb2a-160">shifts</span></span>   | <span data-ttu-id="4cb2a-161">Коллекция [shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-161">[shift](shift.md) collection</span></span>  | <span data-ttu-id="4cb2a-162">Смены в расписании.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-162">The shifts in the schedule.</span></span> |
| <span data-ttu-id="4cb2a-163">тимесофф</span><span class="sxs-lookup"><span data-stu-id="4cb2a-163">timesOff</span></span>   |<span data-ttu-id="4cb2a-164">Коллекция [тимеофф](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-164">[timeOff](timeoff.md) collection</span></span>  | <span data-ttu-id="4cb2a-165">Экземпляры повременных вызовов в расписании.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-165">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="4cb2a-166">тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="4cb2a-166">timeOffReasons</span></span>   |<span data-ttu-id="4cb2a-167">Коллекция [тимеоффреасон](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-167">[timeOffReason](timeoffreason.md) collection</span></span>  | <span data-ttu-id="4cb2a-168">Набор причин незапланированного времени.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-168">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="4cb2a-169">счедулингграупс</span><span class="sxs-lookup"><span data-stu-id="4cb2a-169">schedulingGroups</span></span>   |<span data-ttu-id="4cb2a-170">Коллекция объектов [schedulingGroup](schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-170">[schedulingGroup](schedulinggroup.md) collection</span></span>  | <span data-ttu-id="4cb2a-171">Логическая группа пользователей в расписании (обычно по роли).</span><span class="sxs-lookup"><span data-stu-id="4cb2a-171">The logical grouping of users in the schedule (usually by role).</span></span> |
| <span data-ttu-id="4cb2a-172">опеншифтс</span><span class="sxs-lookup"><span data-stu-id="4cb2a-172">openshifts</span></span>   |<span data-ttu-id="4cb2a-173">Коллекция [опеншифт](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-173">[openShift](openshift.md) collection</span></span> | <span data-ttu-id="4cb2a-174">Набор смен, открытых в группе планирования, в расписании.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-174">The set of open shifts in a scheduling group in the schedule.</span></span> |
| <span data-ttu-id="4cb2a-175">воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="4cb2a-175">workforceintegrations</span></span>   |<span data-ttu-id="4cb2a-176">Коллекция [воркфорцеинтегратион](workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-176">[workforceIntegration](workforceintegration.md) collection</span></span>  | <span data-ttu-id="4cb2a-177">Экземпляр интеграции сотрудников для группы с исходящим трафиком в синхронных уведомлениях об изменениях (для поддерживаемых сущностей).</span><span class="sxs-lookup"><span data-stu-id="4cb2a-177">An instance of a workforce integration per team with outbound data flow on synchronous change notifications (for supported entities).</span></span> |
| <span data-ttu-id="4cb2a-178">свапшифтчанжерекуестс</span><span class="sxs-lookup"><span data-stu-id="4cb2a-178">swapshiftchangerequests</span></span>   |<span data-ttu-id="4cb2a-179">Коллекция [свапшифтсчанжерекуест](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-179">[swapShiftsChangeRequest](swapshiftschangerequest.md) collection</span></span>  | <span data-ttu-id="4cb2a-180">Запросы на замену для сдвигов в расписании.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-180">The swap requests for shifts in the schedule.</span></span> |
| <span data-ttu-id="4cb2a-181">опеншифтчанжерекуестс</span><span class="sxs-lookup"><span data-stu-id="4cb2a-181">openshiftchangerequests</span></span>   |<span data-ttu-id="4cb2a-182">Коллекция [опеншифтчанжерекуест](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-182">[openShiftChangeRequest](openshiftchangerequest.md) collection</span></span>  | <span data-ttu-id="4cb2a-183">Запросы на открытие с открытым сдвигом по расписанию.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-183">The open shift requests in the schedule.</span></span> |
| <span data-ttu-id="4cb2a-184">тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="4cb2a-184">timeoffrequest</span></span>   |<span data-ttu-id="4cb2a-185">Коллекция [тимеоффрекуест](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="4cb2a-185">[timeOffRequest](timeoffrequest.md) collection</span></span>  | <span data-ttu-id="4cb2a-186">Время, в течение которого запросы отменяются по расписанию.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-186">The time off requests in the schedule.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4cb2a-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cb2a-187">JSON representation</span></span>

<span data-ttu-id="4cb2a-188">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cb2a-188">The following is a JSON representation of the resource.</span></span>

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

