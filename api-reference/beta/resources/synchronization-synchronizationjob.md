---
title: Тип ресурса synchronizationJob
description: Выполняет синхронизацию путем периодического выполнения в фоновом режиме, опроса изменений в одном каталоге и их перенанесения в другой каталог.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f0036cd26a72effba41085d9a4638647fd4060e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132043"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="f79d0-103">Тип ресурса synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f79d0-103">synchronizationJob resource type</span></span>

<span data-ttu-id="f79d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f79d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f79d0-105">Выполняет синхронизацию путем периодического выполнения в фоновом режиме, опроса изменений в одном каталоге и их перенанесения в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="f79d0-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="f79d0-106">Задание синхронизации всегда является специфическим для конкретного экземпляра приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f79d0-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="f79d0-107">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге и настроить схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="f79d0-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="f79d0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f79d0-108">Methods</span></span>

| <span data-ttu-id="f79d0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f79d0-109">Method</span></span>        | <span data-ttu-id="f79d0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f79d0-110">Return Type</span></span>               | <span data-ttu-id="f79d0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f79d0-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="f79d0-112">Список</span><span class="sxs-lookup"><span data-stu-id="f79d0-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="f79d0-113">[Коллекция synchronizationJob](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="f79d0-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="f79d0-114">Список существующих заданий для заданного экземпляра приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="f79d0-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="f79d0-115">Get synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f79d0-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="f79d0-116">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f79d0-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="f79d0-117">Чтение свойств и связей объекта synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="f79d0-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="f79d0-118">Создание</span><span class="sxs-lookup"><span data-stu-id="f79d0-118">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="f79d0-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f79d0-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="f79d0-120">Создайте новое задание для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="f79d0-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="f79d0-121">Начало</span><span class="sxs-lookup"><span data-stu-id="f79d0-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="f79d0-122">Нет</span><span class="sxs-lookup"><span data-stu-id="f79d0-122">None</span></span>   |<span data-ttu-id="f79d0-123">Запустите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="f79d0-123">Start synchronization.</span></span> <span data-ttu-id="f79d0-124">Если задание приостановлено, оно продолжается с момента приостановки задания.</span><span class="sxs-lookup"><span data-stu-id="f79d0-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="f79d0-125">Если задание находится в карантине, состояние карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="f79d0-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="f79d0-126">Restart</span><span class="sxs-lookup"><span data-stu-id="f79d0-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="f79d0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f79d0-127">None</span></span>   |<span data-ttu-id="f79d0-128">При принудительном запуске задания и повторной обработке всех объектов в каталоге.</span><span class="sxs-lookup"><span data-stu-id="f79d0-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="f79d0-129">Pause</span><span class="sxs-lookup"><span data-stu-id="f79d0-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="f79d0-130">Нет</span><span class="sxs-lookup"><span data-stu-id="f79d0-130">None</span></span>   |<span data-ttu-id="f79d0-131">Временно остановите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="f79d0-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="f79d0-132">Все ходы выполнения, включая состояние задания, сохраняются, и задание продолжит работу с того места, где оно было отключено при [запуске](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="f79d0-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="f79d0-133">Delete</span><span class="sxs-lookup"><span data-stu-id="f79d0-133">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="f79d0-134">Нет</span><span class="sxs-lookup"><span data-stu-id="f79d0-134">None</span></span>   |<span data-ttu-id="f79d0-135">Остановите синхронизацию и окончательно удалите все состояние, связанное с заданием.</span><span class="sxs-lookup"><span data-stu-id="f79d0-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="f79d0-136">Get synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f79d0-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="f79d0-137">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f79d0-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="f79d0-138">Получить эффективную схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="f79d0-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="f79d0-139">Обновление synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f79d0-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="f79d0-140">Нет</span><span class="sxs-lookup"><span data-stu-id="f79d0-140">None</span></span>   |<span data-ttu-id="f79d0-141">Обновление схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="f79d0-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="f79d0-142">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="f79d0-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="f79d0-143">Нет</span><span class="sxs-lookup"><span data-stu-id="f79d0-143">None</span></span>|<span data-ttu-id="f79d0-144">Проверьте предоставленные учетные данные в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="f79d0-144">Test provided credentials against target directory.</span></span>|
|[<span data-ttu-id="f79d0-145">provisionOnDemand</span><span class="sxs-lookup"><span data-stu-id="f79d0-145">provisionOnDemand</span></span>](../api/synchronization-synchronizationjob-provision-on-demand.md)|<span data-ttu-id="f79d0-146">[Коллекция synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="f79d0-146">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="f79d0-147">Представляет объекты, которые будут быть выполнены с выполнением правил синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f79d0-147">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="f79d0-148">Ресурс в основном используется для предоставления по требованию.</span><span class="sxs-lookup"><span data-stu-id="f79d0-148">The resource is primarily used for on-demand provisioning.</span></span> |
## <a name="properties"></a><span data-ttu-id="f79d0-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="f79d0-149">Properties</span></span>

| <span data-ttu-id="f79d0-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="f79d0-150">Property</span></span>      | <span data-ttu-id="f79d0-151">Тип</span><span class="sxs-lookup"><span data-stu-id="f79d0-151">Type</span></span>      | <span data-ttu-id="f79d0-152">Описание</span><span class="sxs-lookup"><span data-stu-id="f79d0-152">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f79d0-153">id</span><span class="sxs-lookup"><span data-stu-id="f79d0-153">id</span></span>             |<span data-ttu-id="f79d0-154">Строка</span><span class="sxs-lookup"><span data-stu-id="f79d0-154">String</span></span>                     |<span data-ttu-id="f79d0-155">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f79d0-155">Unique synchronization job identifier.</span></span> <span data-ttu-id="f79d0-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f79d0-156">Read-only.</span></span>|
|<span data-ttu-id="f79d0-157">schedule</span><span class="sxs-lookup"><span data-stu-id="f79d0-157">schedule</span></span>       |[<span data-ttu-id="f79d0-158">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="f79d0-158">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="f79d0-159">Расписание, используемая для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="f79d0-159">Schedule used to run the job.</span></span> <span data-ttu-id="f79d0-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f79d0-160">Read-only.</span></span>|
|<span data-ttu-id="f79d0-161">status</span><span class="sxs-lookup"><span data-stu-id="f79d0-161">status</span></span>         |[<span data-ttu-id="f79d0-162">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="f79d0-162">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="f79d0-163">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="f79d0-163">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="f79d0-164">synchronizationJobSettings</span><span class="sxs-lookup"><span data-stu-id="f79d0-164">synchronizationJobSettings</span></span>   |<span data-ttu-id="f79d0-165">[keyValuePair](keyvaluepair.md);</span><span class="sxs-lookup"><span data-stu-id="f79d0-165">[keyValuePair](keyvaluepair.md)</span></span>    |<span data-ttu-id="f79d0-166">Параметры, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="f79d0-166">Settings associated with the job.</span></span> <span data-ttu-id="f79d0-167">Некоторые параметры наследуются от шаблона.</span><span class="sxs-lookup"><span data-stu-id="f79d0-167">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="f79d0-168">templateId</span><span class="sxs-lookup"><span data-stu-id="f79d0-168">templateId</span></span>     |<span data-ttu-id="f79d0-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f79d0-169">String</span></span>    |<span data-ttu-id="f79d0-170">Идентификатор шаблона [синхронизации, на](synchronization-synchronizationtemplate.md) котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="f79d0-170">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f79d0-171">Связи</span><span class="sxs-lookup"><span data-stu-id="f79d0-171">Relationships</span></span>
| <span data-ttu-id="f79d0-172">Связь</span><span class="sxs-lookup"><span data-stu-id="f79d0-172">Relationship</span></span> | <span data-ttu-id="f79d0-173">Тип</span><span class="sxs-lookup"><span data-stu-id="f79d0-173">Type</span></span>   |<span data-ttu-id="f79d0-174">Описание</span><span class="sxs-lookup"><span data-stu-id="f79d0-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f79d0-175">схема</span><span class="sxs-lookup"><span data-stu-id="f79d0-175">schema</span></span>|[<span data-ttu-id="f79d0-176">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f79d0-176">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="f79d0-177">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="f79d0-177">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f79d0-178">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f79d0-178">JSON representation</span></span>

<span data-ttu-id="f79d0-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f79d0-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "synchronizationJobSettings": {"@odata.type": "microsoft.graph.keyValuePair"},
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
  "suppressions": []
}
-->


