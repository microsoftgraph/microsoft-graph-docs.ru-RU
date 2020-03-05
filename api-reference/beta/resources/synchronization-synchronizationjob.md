---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cac54f10a3109be5596a62a84271a485a5f70449
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520074"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="65011-105">Тип ресурса Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="65011-105">synchronizationJob resource type</span></span>

<span data-ttu-id="65011-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65011-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65011-107">Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="65011-107">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="65011-108">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="65011-108">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="65011-109">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="65011-109">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="65011-110">Методы</span><span class="sxs-lookup"><span data-stu-id="65011-110">Methods</span></span>

| <span data-ttu-id="65011-111">Метод</span><span class="sxs-lookup"><span data-stu-id="65011-111">Method</span></span>        | <span data-ttu-id="65011-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65011-112">Return Type</span></span>               | <span data-ttu-id="65011-113">Описание</span><span class="sxs-lookup"><span data-stu-id="65011-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="65011-114">List</span><span class="sxs-lookup"><span data-stu-id="65011-114">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="65011-115">Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="65011-115">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="65011-116">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="65011-116">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="65011-117">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="65011-117">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="65011-118">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="65011-118">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="65011-119">Чтение свойств и связей объекта Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="65011-119">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="65011-120">[создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="65011-120">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="65011-121">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="65011-121">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="65011-122">Создание нового задания для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="65011-122">Create new job for a given application.</span></span>|
|[<span data-ttu-id="65011-123">Начало</span><span class="sxs-lookup"><span data-stu-id="65011-123">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="65011-124">Нет</span><span class="sxs-lookup"><span data-stu-id="65011-124">None</span></span>   |<span data-ttu-id="65011-125">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="65011-125">Start synchronization.</span></span> <span data-ttu-id="65011-126">Если задание приостановлено, оно продолжается с того места, где было приостановлено задание.</span><span class="sxs-lookup"><span data-stu-id="65011-126">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="65011-127">Если задание находится в карантине, статус карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="65011-127">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="65011-128">Restart</span><span class="sxs-lookup"><span data-stu-id="65011-128">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="65011-129">Нет</span><span class="sxs-lookup"><span data-stu-id="65011-129">None</span></span>   |<span data-ttu-id="65011-130">Принудительно запустить задание и повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="65011-130">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="65011-131">Pause</span><span class="sxs-lookup"><span data-stu-id="65011-131">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="65011-132">Нет</span><span class="sxs-lookup"><span data-stu-id="65011-132">None</span></span>   |<span data-ttu-id="65011-133">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="65011-133">Temporarily stop synchronization.</span></span> <span data-ttu-id="65011-134">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="65011-134">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|<span data-ttu-id="65011-135">[удаление](../api/synchronization-synchronizationjob-delete.md);</span><span class="sxs-lookup"><span data-stu-id="65011-135">[Delete](../api/synchronization-synchronizationjob-delete.md)</span></span>        |<span data-ttu-id="65011-136">Нет</span><span class="sxs-lookup"><span data-stu-id="65011-136">None</span></span>   |<span data-ttu-id="65011-137">Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="65011-137">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="65011-138">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="65011-138">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="65011-139">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="65011-139">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="65011-140">Получение действующей схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="65011-140">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="65011-141">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="65011-141">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="65011-142">Нет</span><span class="sxs-lookup"><span data-stu-id="65011-142">None</span></span>   |<span data-ttu-id="65011-143">Обновите схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="65011-143">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="65011-144">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="65011-144">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="65011-145">Нет</span><span class="sxs-lookup"><span data-stu-id="65011-145">None</span></span>|<span data-ttu-id="65011-146">Проверка предоставленных учетных данных в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="65011-146">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="65011-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="65011-147">Properties</span></span>

| <span data-ttu-id="65011-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="65011-148">Property</span></span>      | <span data-ttu-id="65011-149">Тип</span><span class="sxs-lookup"><span data-stu-id="65011-149">Type</span></span>      | <span data-ttu-id="65011-150">Описание</span><span class="sxs-lookup"><span data-stu-id="65011-150">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="65011-151">id</span><span class="sxs-lookup"><span data-stu-id="65011-151">id</span></span>             |<span data-ttu-id="65011-152">String</span><span class="sxs-lookup"><span data-stu-id="65011-152">String</span></span>                     |<span data-ttu-id="65011-153">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="65011-153">Unique synchronization job identifier.</span></span> <span data-ttu-id="65011-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65011-154">Read-only.</span></span>|
|<span data-ttu-id="65011-155">schedule</span><span class="sxs-lookup"><span data-stu-id="65011-155">schedule</span></span>       |[<span data-ttu-id="65011-156">синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="65011-156">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="65011-157">Расписание, используемое для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="65011-157">Schedule used to run the job.</span></span> <span data-ttu-id="65011-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65011-158">Read-only.</span></span>|
|<span data-ttu-id="65011-159">status</span><span class="sxs-lookup"><span data-stu-id="65011-159">status</span></span>         |[<span data-ttu-id="65011-160">синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="65011-160">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="65011-161">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="65011-161">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="65011-162">синчронизатионжобсеттингс</span><span class="sxs-lookup"><span data-stu-id="65011-162">synchronizationJobSettings</span></span>   |<span data-ttu-id="65011-163">[keyValuePair](keyvaluepair.md);</span><span class="sxs-lookup"><span data-stu-id="65011-163">[keyValuePair](keyvaluepair.md)</span></span>    |<span data-ttu-id="65011-164">Параметры, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="65011-164">Settings associated with the job.</span></span> <span data-ttu-id="65011-165">Некоторые параметры наследуются от шаблона.</span><span class="sxs-lookup"><span data-stu-id="65011-165">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="65011-166">templateId</span><span class="sxs-lookup"><span data-stu-id="65011-166">templateId</span></span>     |<span data-ttu-id="65011-167">String</span><span class="sxs-lookup"><span data-stu-id="65011-167">String</span></span>    |<span data-ttu-id="65011-168">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="65011-168">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65011-169">Связи</span><span class="sxs-lookup"><span data-stu-id="65011-169">Relationships</span></span>
| <span data-ttu-id="65011-170">Связь</span><span class="sxs-lookup"><span data-stu-id="65011-170">Relationship</span></span> | <span data-ttu-id="65011-171">Тип</span><span class="sxs-lookup"><span data-stu-id="65011-171">Type</span></span>   |<span data-ttu-id="65011-172">Описание</span><span class="sxs-lookup"><span data-stu-id="65011-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65011-173">схемы</span><span class="sxs-lookup"><span data-stu-id="65011-173">schema</span></span>|[<span data-ttu-id="65011-174">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="65011-174">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="65011-175">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="65011-175">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65011-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65011-176">JSON representation</span></span>

<span data-ttu-id="65011-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65011-177">The following is a JSON representation of the resource.</span></span>

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
