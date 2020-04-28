---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18c8076a55643289e8ef33fa4316cd224abfe02e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217544"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="d3985-103">Тип ресурса Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="d3985-103">synchronizationJob resource type</span></span>

<span data-ttu-id="d3985-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3985-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3985-105">Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="d3985-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="d3985-106">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d3985-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="d3985-107">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="d3985-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="d3985-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d3985-108">Methods</span></span>

| <span data-ttu-id="d3985-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d3985-109">Method</span></span>        | <span data-ttu-id="d3985-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d3985-110">Return Type</span></span>               | <span data-ttu-id="d3985-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3985-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="d3985-112">List</span><span class="sxs-lookup"><span data-stu-id="d3985-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="d3985-113">Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="d3985-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="d3985-114">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="d3985-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="d3985-115">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="d3985-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="d3985-116">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="d3985-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="d3985-117">Чтение свойств и связей объекта Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="d3985-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="d3985-118">[создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="d3985-118">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="d3985-119">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="d3985-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="d3985-120">Создание нового задания для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="d3985-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="d3985-121">Начало</span><span class="sxs-lookup"><span data-stu-id="d3985-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="d3985-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d3985-122">None</span></span>   |<span data-ttu-id="d3985-123">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3985-123">Start synchronization.</span></span> <span data-ttu-id="d3985-124">Если задание приостановлено, оно продолжается с того места, где было приостановлено задание.</span><span class="sxs-lookup"><span data-stu-id="d3985-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="d3985-125">Если задание находится в карантине, статус карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="d3985-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="d3985-126">Restart</span><span class="sxs-lookup"><span data-stu-id="d3985-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="d3985-127">Нет</span><span class="sxs-lookup"><span data-stu-id="d3985-127">None</span></span>   |<span data-ttu-id="d3985-128">Принудительно запустить задание и повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d3985-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="d3985-129">Pause</span><span class="sxs-lookup"><span data-stu-id="d3985-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="d3985-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d3985-130">None</span></span>   |<span data-ttu-id="d3985-131">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3985-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="d3985-132">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="d3985-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|<span data-ttu-id="d3985-133">[удаление](../api/synchronization-synchronizationjob-delete.md);</span><span class="sxs-lookup"><span data-stu-id="d3985-133">[Delete](../api/synchronization-synchronizationjob-delete.md)</span></span>        |<span data-ttu-id="d3985-134">Нет</span><span class="sxs-lookup"><span data-stu-id="d3985-134">None</span></span>   |<span data-ttu-id="d3985-135">Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="d3985-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="d3985-136">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="d3985-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="d3985-137">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="d3985-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="d3985-138">Получение действующей схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="d3985-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="d3985-139">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="d3985-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="d3985-140">Нет</span><span class="sxs-lookup"><span data-stu-id="d3985-140">None</span></span>   |<span data-ttu-id="d3985-141">Обновите схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="d3985-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="d3985-142">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="d3985-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="d3985-143">Нет</span><span class="sxs-lookup"><span data-stu-id="d3985-143">None</span></span>|<span data-ttu-id="d3985-144">Проверка предоставленных учетных данных в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="d3985-144">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3985-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3985-145">Properties</span></span>

| <span data-ttu-id="d3985-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3985-146">Property</span></span>      | <span data-ttu-id="d3985-147">Тип</span><span class="sxs-lookup"><span data-stu-id="d3985-147">Type</span></span>      | <span data-ttu-id="d3985-148">Описание</span><span class="sxs-lookup"><span data-stu-id="d3985-148">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d3985-149">id</span><span class="sxs-lookup"><span data-stu-id="d3985-149">id</span></span>             |<span data-ttu-id="d3985-150">String</span><span class="sxs-lookup"><span data-stu-id="d3985-150">String</span></span>                     |<span data-ttu-id="d3985-151">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3985-151">Unique synchronization job identifier.</span></span> <span data-ttu-id="d3985-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3985-152">Read-only.</span></span>|
|<span data-ttu-id="d3985-153">schedule</span><span class="sxs-lookup"><span data-stu-id="d3985-153">schedule</span></span>       |[<span data-ttu-id="d3985-154">синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="d3985-154">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="d3985-155">Расписание, используемое для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="d3985-155">Schedule used to run the job.</span></span> <span data-ttu-id="d3985-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3985-156">Read-only.</span></span>|
|<span data-ttu-id="d3985-157">status</span><span class="sxs-lookup"><span data-stu-id="d3985-157">status</span></span>         |[<span data-ttu-id="d3985-158">синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="d3985-158">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="d3985-159">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="d3985-159">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="d3985-160">синчронизатионжобсеттингс</span><span class="sxs-lookup"><span data-stu-id="d3985-160">synchronizationJobSettings</span></span>   |<span data-ttu-id="d3985-161">[keyValuePair](keyvaluepair.md);</span><span class="sxs-lookup"><span data-stu-id="d3985-161">[keyValuePair](keyvaluepair.md)</span></span>    |<span data-ttu-id="d3985-162">Параметры, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="d3985-162">Settings associated with the job.</span></span> <span data-ttu-id="d3985-163">Некоторые параметры наследуются от шаблона.</span><span class="sxs-lookup"><span data-stu-id="d3985-163">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="d3985-164">templateId</span><span class="sxs-lookup"><span data-stu-id="d3985-164">templateId</span></span>     |<span data-ttu-id="d3985-165">String</span><span class="sxs-lookup"><span data-stu-id="d3985-165">String</span></span>    |<span data-ttu-id="d3985-166">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="d3985-166">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3985-167">Связи</span><span class="sxs-lookup"><span data-stu-id="d3985-167">Relationships</span></span>
| <span data-ttu-id="d3985-168">Связь</span><span class="sxs-lookup"><span data-stu-id="d3985-168">Relationship</span></span> | <span data-ttu-id="d3985-169">Тип</span><span class="sxs-lookup"><span data-stu-id="d3985-169">Type</span></span>   |<span data-ttu-id="d3985-170">Описание</span><span class="sxs-lookup"><span data-stu-id="d3985-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3985-171">схемы</span><span class="sxs-lookup"><span data-stu-id="d3985-171">schema</span></span>|[<span data-ttu-id="d3985-172">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="d3985-172">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="d3985-173">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="d3985-173">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3985-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3985-174">JSON representation</span></span>

<span data-ttu-id="d3985-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3985-175">The following is a JSON representation of the resource.</span></span>

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
