---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 19f30dd20d313d5ab7a46dd9368d391b83ee1993
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620733"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="2453d-105">Тип ресурса Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2453d-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2453d-106">Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="2453d-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="2453d-107">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2453d-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="2453d-108">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="2453d-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="2453d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="2453d-109">Methods</span></span>

| <span data-ttu-id="2453d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="2453d-110">Method</span></span>        | <span data-ttu-id="2453d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2453d-111">Return Type</span></span>               | <span data-ttu-id="2453d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2453d-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="2453d-113">List</span><span class="sxs-lookup"><span data-stu-id="2453d-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="2453d-114">Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="2453d-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="2453d-115">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="2453d-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="2453d-116">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2453d-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="2453d-117">Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2453d-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="2453d-118">Чтение свойств и связей объекта Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="2453d-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="2453d-119">[создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="2453d-119">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="2453d-120">Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2453d-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="2453d-121">Создание нового задания для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="2453d-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="2453d-122">Start</span><span class="sxs-lookup"><span data-stu-id="2453d-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="2453d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2453d-123">None</span></span>   |<span data-ttu-id="2453d-124">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2453d-124">Start synchronization.</span></span> <span data-ttu-id="2453d-125">Если задание приостановлено, оно продолжается с того места, где было приостановлено задание.</span><span class="sxs-lookup"><span data-stu-id="2453d-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="2453d-126">Если задание находится в карантине, статус карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="2453d-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="2453d-127">Restart</span><span class="sxs-lookup"><span data-stu-id="2453d-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="2453d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="2453d-128">None</span></span>   |<span data-ttu-id="2453d-129">Принудительно запустить задание и повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2453d-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="2453d-130">Pause</span><span class="sxs-lookup"><span data-stu-id="2453d-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="2453d-131">Нет</span><span class="sxs-lookup"><span data-stu-id="2453d-131">None</span></span>   |<span data-ttu-id="2453d-132">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2453d-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="2453d-133">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="2453d-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="2453d-134">Удаление</span><span class="sxs-lookup"><span data-stu-id="2453d-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="2453d-135">Нет</span><span class="sxs-lookup"><span data-stu-id="2453d-135">None</span></span>   |<span data-ttu-id="2453d-136">Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="2453d-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="2453d-137">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2453d-137">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="2453d-138">Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2453d-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="2453d-139">Получение действующей схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="2453d-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="2453d-140">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2453d-140">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="2453d-141">Нет</span><span class="sxs-lookup"><span data-stu-id="2453d-141">None</span></span>   |<span data-ttu-id="2453d-142">Обновите схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="2453d-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="2453d-143">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="2453d-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="2453d-144">Нет</span><span class="sxs-lookup"><span data-stu-id="2453d-144">None</span></span>|<span data-ttu-id="2453d-145">Проверка предоставленных учетных данных в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="2453d-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="2453d-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="2453d-146">Properties</span></span>

| <span data-ttu-id="2453d-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="2453d-147">Property</span></span>      | <span data-ttu-id="2453d-148">Тип</span><span class="sxs-lookup"><span data-stu-id="2453d-148">Type</span></span>      | <span data-ttu-id="2453d-149">Описание</span><span class="sxs-lookup"><span data-stu-id="2453d-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="2453d-150">id</span><span class="sxs-lookup"><span data-stu-id="2453d-150">id</span></span>             |<span data-ttu-id="2453d-151">String</span><span class="sxs-lookup"><span data-stu-id="2453d-151">String</span></span>                     |<span data-ttu-id="2453d-152">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2453d-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="2453d-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2453d-153">Read-only.</span></span>|
|<span data-ttu-id="2453d-154">schedule</span><span class="sxs-lookup"><span data-stu-id="2453d-154">schedule</span></span>       |[<span data-ttu-id="2453d-155">Синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="2453d-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="2453d-156">Расписание, используемое для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="2453d-156">Schedule used to run the job.</span></span> <span data-ttu-id="2453d-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2453d-157">Read-only.</span></span>|
|<span data-ttu-id="2453d-158">status</span><span class="sxs-lookup"><span data-stu-id="2453d-158">status</span></span>         |[<span data-ttu-id="2453d-159">Синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="2453d-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="2453d-160">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="2453d-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="2453d-161">templateId</span><span class="sxs-lookup"><span data-stu-id="2453d-161">templateId</span></span>     |<span data-ttu-id="2453d-162">String</span><span class="sxs-lookup"><span data-stu-id="2453d-162">String</span></span>    |<span data-ttu-id="2453d-163">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="2453d-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2453d-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="2453d-164">Relationships</span></span>
| <span data-ttu-id="2453d-165">Отношение</span><span class="sxs-lookup"><span data-stu-id="2453d-165">Relationship</span></span> | <span data-ttu-id="2453d-166">Тип</span><span class="sxs-lookup"><span data-stu-id="2453d-166">Type</span></span>   |<span data-ttu-id="2453d-167">Описание</span><span class="sxs-lookup"><span data-stu-id="2453d-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2453d-168">схемы</span><span class="sxs-lookup"><span data-stu-id="2453d-168">schema</span></span>|[<span data-ttu-id="2453d-169">Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2453d-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="2453d-170">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="2453d-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2453d-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2453d-171">JSON representation</span></span>

<span data-ttu-id="2453d-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2453d-172">The following is a JSON representation of the resource.</span></span>

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
