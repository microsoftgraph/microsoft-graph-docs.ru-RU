---
title: Тип ресурса synchronizationJob
description: Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог. Задание синхронизации всегда специально для конкретного экземпляра приложения клиента. Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510570"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="d99a6-105">Тип ресурса synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d99a6-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d99a6-106">Выполняет синхронизацию с периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="d99a6-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="d99a6-107">Задание синхронизации всегда специально для конкретного экземпляра приложения клиента.</span><span class="sxs-lookup"><span data-stu-id="d99a6-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="d99a6-108">Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.</span><span class="sxs-lookup"><span data-stu-id="d99a6-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="d99a6-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d99a6-109">Methods</span></span>

| <span data-ttu-id="d99a6-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d99a6-110">Method</span></span>        | <span data-ttu-id="d99a6-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d99a6-111">Return Type</span></span>               | <span data-ttu-id="d99a6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d99a6-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="d99a6-113">List</span><span class="sxs-lookup"><span data-stu-id="d99a6-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="d99a6-114">[synchronizationJob](synchronization-synchronizationjob.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d99a6-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="d99a6-115">Список существующих заданий для экземпляра данного приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="d99a6-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="d99a6-116">Получение synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d99a6-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="d99a6-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d99a6-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="d99a6-118">Чтение свойства и связи объекта synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="d99a6-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="d99a6-119">Create</span><span class="sxs-lookup"><span data-stu-id="d99a6-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="d99a6-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d99a6-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="d99a6-121">Создание нового задания для данного приложения.</span><span class="sxs-lookup"><span data-stu-id="d99a6-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="d99a6-122">Start</span><span class="sxs-lookup"><span data-stu-id="d99a6-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="d99a6-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d99a6-123">None</span></span>   |<span data-ttu-id="d99a6-124">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d99a6-124">Start synchronization.</span></span> <span data-ttu-id="d99a6-125">Если задание находится в приостановленном состоянии, он по-прежнему производится из точки, где был приостановлен задания.</span><span class="sxs-lookup"><span data-stu-id="d99a6-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="d99a6-126">Если задание находится в карантине, состояние карантина снят.</span><span class="sxs-lookup"><span data-stu-id="d99a6-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="d99a6-127">Restart</span><span class="sxs-lookup"><span data-stu-id="d99a6-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="d99a6-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d99a6-128">None</span></span>   |<span data-ttu-id="d99a6-129">Принудительное задание, чтобы начать заново и повторно обрабатывать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d99a6-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="d99a6-130">Pause</span><span class="sxs-lookup"><span data-stu-id="d99a6-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="d99a6-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d99a6-131">None</span></span>   |<span data-ttu-id="d99a6-132">Временно приостановить синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d99a6-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="d99a6-133">Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.</span><span class="sxs-lookup"><span data-stu-id="d99a6-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="d99a6-134">Delete</span><span class="sxs-lookup"><span data-stu-id="d99a6-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="d99a6-135">Нет</span><span class="sxs-lookup"><span data-stu-id="d99a6-135">None</span></span>   |<span data-ttu-id="d99a6-136">Остановите синхронизацию и окончательно удалить все состояния, связанных с заданием.</span><span class="sxs-lookup"><span data-stu-id="d99a6-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="d99a6-137">Получение synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="d99a6-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="d99a6-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="d99a6-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="d99a6-139">Получите схему эффективной синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="d99a6-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="d99a6-140">Обновление synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="d99a6-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="d99a6-141">Нет</span><span class="sxs-lookup"><span data-stu-id="d99a6-141">None</span></span>   |<span data-ttu-id="d99a6-142">Обновление схемы заданий синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d99a6-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="d99a6-143">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="d99a6-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="d99a6-144">Нет</span><span class="sxs-lookup"><span data-stu-id="d99a6-144">None</span></span>|<span data-ttu-id="d99a6-145">Тестирование предоставленные учетные данные для целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="d99a6-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="d99a6-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="d99a6-146">Properties</span></span>

| <span data-ttu-id="d99a6-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="d99a6-147">Property</span></span>      | <span data-ttu-id="d99a6-148">Тип</span><span class="sxs-lookup"><span data-stu-id="d99a6-148">Type</span></span>      | <span data-ttu-id="d99a6-149">Описание</span><span class="sxs-lookup"><span data-stu-id="d99a6-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d99a6-150">id</span><span class="sxs-lookup"><span data-stu-id="d99a6-150">id</span></span>             |<span data-ttu-id="d99a6-151">String</span><span class="sxs-lookup"><span data-stu-id="d99a6-151">String</span></span>                     |<span data-ttu-id="d99a6-152">Идентификатор задания уникальных синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d99a6-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="d99a6-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d99a6-153">Read-only.</span></span>|
|<span data-ttu-id="d99a6-154">Расписание</span><span class="sxs-lookup"><span data-stu-id="d99a6-154">schedule</span></span>       |[<span data-ttu-id="d99a6-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="d99a6-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="d99a6-156">Расписание выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="d99a6-156">Schedule used to run the job.</span></span> <span data-ttu-id="d99a6-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d99a6-157">Read-only.</span></span>|
|<span data-ttu-id="d99a6-158">status</span><span class="sxs-lookup"><span data-stu-id="d99a6-158">status</span></span>         |[<span data-ttu-id="d99a6-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="d99a6-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="d99a6-160">Состояние задания, которое включает в себя после последнего выполнения задания, текущее состояние задания и ошибках.</span><span class="sxs-lookup"><span data-stu-id="d99a6-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="d99a6-161">templateId</span><span class="sxs-lookup"><span data-stu-id="d99a6-161">templateId</span></span>     |<span data-ttu-id="d99a6-162">String</span><span class="sxs-lookup"><span data-stu-id="d99a6-162">String</span></span>    |<span data-ttu-id="d99a6-163">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) на основе этого задания.</span><span class="sxs-lookup"><span data-stu-id="d99a6-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d99a6-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="d99a6-164">Relationships</span></span>
| <span data-ttu-id="d99a6-165">Связь</span><span class="sxs-lookup"><span data-stu-id="d99a6-165">Relationship</span></span> | <span data-ttu-id="d99a6-166">Тип</span><span class="sxs-lookup"><span data-stu-id="d99a6-166">Type</span></span>   |<span data-ttu-id="d99a6-167">Описание</span><span class="sxs-lookup"><span data-stu-id="d99a6-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d99a6-168">схема</span><span class="sxs-lookup"><span data-stu-id="d99a6-168">schema</span></span>|[<span data-ttu-id="d99a6-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="d99a6-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="d99a6-170">Схема синхронизации, настроенных для задания.</span><span class="sxs-lookup"><span data-stu-id="d99a6-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d99a6-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d99a6-171">JSON representation</span></span>

<span data-ttu-id="d99a6-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d99a6-172">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
