---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8d9cad16e33b022fa7c9d4e97a4d28e89436041
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113919"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="50858-105">Тип ресурса Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="50858-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50858-106">Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="50858-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="50858-107">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="50858-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="50858-108">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="50858-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="50858-109">Методы</span><span class="sxs-lookup"><span data-stu-id="50858-109">Methods</span></span>

| <span data-ttu-id="50858-110">Метод</span><span class="sxs-lookup"><span data-stu-id="50858-110">Method</span></span>        | <span data-ttu-id="50858-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50858-111">Return Type</span></span>               | <span data-ttu-id="50858-112">Описание</span><span class="sxs-lookup"><span data-stu-id="50858-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="50858-113">List</span><span class="sxs-lookup"><span data-stu-id="50858-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="50858-114">Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="50858-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="50858-115">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="50858-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="50858-116">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="50858-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="50858-117">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="50858-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="50858-118">Чтение свойств и связей объекта Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="50858-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="50858-119">[создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="50858-119">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="50858-120">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="50858-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="50858-121">Создание нового задания для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="50858-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="50858-122">Start</span><span class="sxs-lookup"><span data-stu-id="50858-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="50858-123">Нет</span><span class="sxs-lookup"><span data-stu-id="50858-123">None</span></span>   |<span data-ttu-id="50858-124">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="50858-124">Start synchronization.</span></span> <span data-ttu-id="50858-125">Если задание приостановлено, оно продолжается с того места, где было приостановлено задание.</span><span class="sxs-lookup"><span data-stu-id="50858-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="50858-126">Если задание находится в карантине, статус карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="50858-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="50858-127">Restart</span><span class="sxs-lookup"><span data-stu-id="50858-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="50858-128">Нет</span><span class="sxs-lookup"><span data-stu-id="50858-128">None</span></span>   |<span data-ttu-id="50858-129">Принудительно запустить задание и повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="50858-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="50858-130">Pause</span><span class="sxs-lookup"><span data-stu-id="50858-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="50858-131">Нет</span><span class="sxs-lookup"><span data-stu-id="50858-131">None</span></span>   |<span data-ttu-id="50858-132">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="50858-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="50858-133">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="50858-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="50858-134">Удаление</span><span class="sxs-lookup"><span data-stu-id="50858-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="50858-135">Нет</span><span class="sxs-lookup"><span data-stu-id="50858-135">None</span></span>   |<span data-ttu-id="50858-136">Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="50858-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="50858-137">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="50858-137">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="50858-138">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="50858-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="50858-139">Получение действующей схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="50858-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="50858-140">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="50858-140">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="50858-141">Нет</span><span class="sxs-lookup"><span data-stu-id="50858-141">None</span></span>   |<span data-ttu-id="50858-142">Обновите схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="50858-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="50858-143">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="50858-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="50858-144">Нет</span><span class="sxs-lookup"><span data-stu-id="50858-144">None</span></span>|<span data-ttu-id="50858-145">Проверка предоставленных учетных данных в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="50858-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="50858-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="50858-146">Properties</span></span>

| <span data-ttu-id="50858-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="50858-147">Property</span></span>      | <span data-ttu-id="50858-148">Тип</span><span class="sxs-lookup"><span data-stu-id="50858-148">Type</span></span>      | <span data-ttu-id="50858-149">Описание</span><span class="sxs-lookup"><span data-stu-id="50858-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="50858-150">id</span><span class="sxs-lookup"><span data-stu-id="50858-150">id</span></span>             |<span data-ttu-id="50858-151">String</span><span class="sxs-lookup"><span data-stu-id="50858-151">String</span></span>                     |<span data-ttu-id="50858-152">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="50858-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="50858-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50858-153">Read-only.</span></span>|
|<span data-ttu-id="50858-154">schedule</span><span class="sxs-lookup"><span data-stu-id="50858-154">schedule</span></span>       |[<span data-ttu-id="50858-155">синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="50858-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="50858-156">Расписание, используемое для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="50858-156">Schedule used to run the job.</span></span> <span data-ttu-id="50858-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50858-157">Read-only.</span></span>|
|<span data-ttu-id="50858-158">status</span><span class="sxs-lookup"><span data-stu-id="50858-158">status</span></span>         |[<span data-ttu-id="50858-159">синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="50858-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="50858-160">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="50858-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="50858-161">синчронизатионжобсеттингс</span><span class="sxs-lookup"><span data-stu-id="50858-161">synchronizationJobSettings</span></span>   |<span data-ttu-id="50858-162">[keyValuePair](keyvaluepair.md);</span><span class="sxs-lookup"><span data-stu-id="50858-162">[keyValuePair](keyvaluepair.md)</span></span>    |<span data-ttu-id="50858-163">Параметры, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="50858-163">Settings associated with the job.</span></span> <span data-ttu-id="50858-164">Некоторые параметры наследуются от шаблона.</span><span class="sxs-lookup"><span data-stu-id="50858-164">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="50858-165">templateId</span><span class="sxs-lookup"><span data-stu-id="50858-165">templateId</span></span>     |<span data-ttu-id="50858-166">String.</span><span class="sxs-lookup"><span data-stu-id="50858-166">String</span></span>    |<span data-ttu-id="50858-167">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="50858-167">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50858-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="50858-168">Relationships</span></span>
| <span data-ttu-id="50858-169">Отношение</span><span class="sxs-lookup"><span data-stu-id="50858-169">Relationship</span></span> | <span data-ttu-id="50858-170">Тип</span><span class="sxs-lookup"><span data-stu-id="50858-170">Type</span></span>   |<span data-ttu-id="50858-171">Описание</span><span class="sxs-lookup"><span data-stu-id="50858-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50858-172">схемы</span><span class="sxs-lookup"><span data-stu-id="50858-172">schema</span></span>|[<span data-ttu-id="50858-173">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="50858-173">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="50858-174">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="50858-174">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50858-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50858-175">JSON representation</span></span>

<span data-ttu-id="50858-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50858-176">The following is a JSON representation of the resource.</span></span>

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
