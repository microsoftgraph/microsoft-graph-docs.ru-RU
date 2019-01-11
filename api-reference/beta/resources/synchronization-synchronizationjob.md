---
title: Тип ресурса synchronizationJob
description: Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог. Задание синхронизации всегда специально для конкретного экземпляра приложения клиента. Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.
localization_priority: Normal
ms.openlocfilehash: 4d65f39cd63357c8fc7c1e22d3d3871eb1646d53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892150"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="5025e-105">Тип ресурса synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5025e-105">synchronizationJob resource type</span></span>

> <span data-ttu-id="5025e-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5025e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5025e-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5025e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5025e-108">Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="5025e-108">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="5025e-109">Задание синхронизации всегда специально для конкретного экземпляра приложения клиента.</span><span class="sxs-lookup"><span data-stu-id="5025e-109">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="5025e-110">Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.</span><span class="sxs-lookup"><span data-stu-id="5025e-110">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="5025e-111">Методы</span><span class="sxs-lookup"><span data-stu-id="5025e-111">Methods</span></span>

| <span data-ttu-id="5025e-112">Метод</span><span class="sxs-lookup"><span data-stu-id="5025e-112">Method</span></span>        | <span data-ttu-id="5025e-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5025e-113">Return Type</span></span>               | <span data-ttu-id="5025e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5025e-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="5025e-115">List</span><span class="sxs-lookup"><span data-stu-id="5025e-115">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="5025e-116">[synchronizationJob](synchronization-synchronizationjob.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5025e-116">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="5025e-117">Список существующих заданий для экземпляра данного приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="5025e-117">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="5025e-118">Получение synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5025e-118">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="5025e-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5025e-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="5025e-120">Чтение свойства и связи объекта synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="5025e-120">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="5025e-121">[создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="5025e-121">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="5025e-122">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5025e-122">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="5025e-123">Создание нового задания для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="5025e-123">Create new job for a given application.</span></span>|
|[<span data-ttu-id="5025e-124">Start</span><span class="sxs-lookup"><span data-stu-id="5025e-124">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="5025e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="5025e-125">None</span></span>   |<span data-ttu-id="5025e-126">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5025e-126">Start synchronization.</span></span> <span data-ttu-id="5025e-127">Если задание находится в приостановленном состоянии, он по-прежнему производится из точки, где был приостановлен задания.</span><span class="sxs-lookup"><span data-stu-id="5025e-127">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="5025e-128">Если задание находится в карантине, состояние карантина снят.</span><span class="sxs-lookup"><span data-stu-id="5025e-128">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="5025e-129">Restart</span><span class="sxs-lookup"><span data-stu-id="5025e-129">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="5025e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5025e-130">None</span></span>   |<span data-ttu-id="5025e-131">Принудительное задание, чтобы начать заново и повторно обрабатывать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5025e-131">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="5025e-132">Pause</span><span class="sxs-lookup"><span data-stu-id="5025e-132">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="5025e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="5025e-133">None</span></span>   |<span data-ttu-id="5025e-134">Временно приостановить синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5025e-134">Temporarily stop synchronization.</span></span> <span data-ttu-id="5025e-135">Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.</span><span class="sxs-lookup"><span data-stu-id="5025e-135">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="5025e-136">Delete</span><span class="sxs-lookup"><span data-stu-id="5025e-136">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="5025e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5025e-137">None</span></span>   |<span data-ttu-id="5025e-138">Остановите синхронизацию и окончательно удалить все состояния, связанных с заданием.</span><span class="sxs-lookup"><span data-stu-id="5025e-138">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="5025e-139">Получение synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="5025e-139">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="5025e-140">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5025e-140">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="5025e-141">Получите схему эффективной синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="5025e-141">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="5025e-142">Обновление synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="5025e-142">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="5025e-143">Нет</span><span class="sxs-lookup"><span data-stu-id="5025e-143">None</span></span>   |<span data-ttu-id="5025e-144">Обновление схемы заданий синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5025e-144">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="5025e-145">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="5025e-145">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="5025e-146">Нет</span><span class="sxs-lookup"><span data-stu-id="5025e-146">None</span></span>|<span data-ttu-id="5025e-147">Тестирование предоставленные учетные данные для целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="5025e-147">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="5025e-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="5025e-148">Properties</span></span>

| <span data-ttu-id="5025e-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="5025e-149">Property</span></span>      | <span data-ttu-id="5025e-150">Тип</span><span class="sxs-lookup"><span data-stu-id="5025e-150">Type</span></span>      | <span data-ttu-id="5025e-151">Описание</span><span class="sxs-lookup"><span data-stu-id="5025e-151">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="5025e-152">id</span><span class="sxs-lookup"><span data-stu-id="5025e-152">id</span></span>             |<span data-ttu-id="5025e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="5025e-153">String</span></span>                     |<span data-ttu-id="5025e-154">Идентификатор задания уникальных синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5025e-154">Unique synchronization job identifier.</span></span> <span data-ttu-id="5025e-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5025e-155">Read-only.</span></span>|
|<span data-ttu-id="5025e-156">расписание</span><span class="sxs-lookup"><span data-stu-id="5025e-156">schedule</span></span>       |[<span data-ttu-id="5025e-157">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="5025e-157">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="5025e-158">Расписание выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="5025e-158">Schedule used to run the job.</span></span> <span data-ttu-id="5025e-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5025e-159">Read-only.</span></span>|
|<span data-ttu-id="5025e-160">status</span><span class="sxs-lookup"><span data-stu-id="5025e-160">status</span></span>         |[<span data-ttu-id="5025e-161">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="5025e-161">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="5025e-162">Состояние задания, которое включает в себя после последнего выполнения задания, текущее состояние задания и ошибках.</span><span class="sxs-lookup"><span data-stu-id="5025e-162">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="5025e-163">templateId</span><span class="sxs-lookup"><span data-stu-id="5025e-163">templateId</span></span>     |<span data-ttu-id="5025e-164">String</span><span class="sxs-lookup"><span data-stu-id="5025e-164">String</span></span>    |<span data-ttu-id="5025e-165">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) на основе этого задания.</span><span class="sxs-lookup"><span data-stu-id="5025e-165">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5025e-166">Связи</span><span class="sxs-lookup"><span data-stu-id="5025e-166">Relationships</span></span>
| <span data-ttu-id="5025e-167">Связь</span><span class="sxs-lookup"><span data-stu-id="5025e-167">Relationship</span></span> | <span data-ttu-id="5025e-168">Тип</span><span class="sxs-lookup"><span data-stu-id="5025e-168">Type</span></span>   |<span data-ttu-id="5025e-169">Описание</span><span class="sxs-lookup"><span data-stu-id="5025e-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5025e-170">схема</span><span class="sxs-lookup"><span data-stu-id="5025e-170">schema</span></span>|[<span data-ttu-id="5025e-171">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5025e-171">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="5025e-172">Схема синхронизации, настроенных для задания.</span><span class="sxs-lookup"><span data-stu-id="5025e-172">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5025e-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5025e-173">JSON representation</span></span>

<span data-ttu-id="5025e-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5025e-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
