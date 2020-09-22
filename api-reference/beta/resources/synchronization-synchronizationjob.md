---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f9d8eecb7b7804af7296bda581eb9b9c9d58d1b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026124"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="ff1cf-103">Тип ресурса Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="ff1cf-103">synchronizationJob resource type</span></span>

<span data-ttu-id="ff1cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff1cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff1cf-105">Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="ff1cf-106">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="ff1cf-107">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="ff1cf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ff1cf-108">Methods</span></span>

| <span data-ttu-id="ff1cf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ff1cf-109">Method</span></span>        | <span data-ttu-id="ff1cf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff1cf-110">Return Type</span></span>               | <span data-ttu-id="ff1cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1cf-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="ff1cf-112">Список</span><span class="sxs-lookup"><span data-stu-id="ff1cf-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="ff1cf-113">Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="ff1cf-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="ff1cf-114">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="ff1cf-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="ff1cf-115">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="ff1cf-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="ff1cf-116">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="ff1cf-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="ff1cf-117">Чтение свойств и связей объекта Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="ff1cf-118">[создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="ff1cf-118">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="ff1cf-119">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="ff1cf-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="ff1cf-120">Создание нового задания для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="ff1cf-121">Начало</span><span class="sxs-lookup"><span data-stu-id="ff1cf-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="ff1cf-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1cf-122">None</span></span>   |<span data-ttu-id="ff1cf-123">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-123">Start synchronization.</span></span> <span data-ttu-id="ff1cf-124">Если задание приостановлено, оно продолжается с того места, где было приостановлено задание.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="ff1cf-125">Если задание находится в карантине, статус карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="ff1cf-126">Перезапуск</span><span class="sxs-lookup"><span data-stu-id="ff1cf-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="ff1cf-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1cf-127">None</span></span>   |<span data-ttu-id="ff1cf-128">Принудительно запустить задание и повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="ff1cf-129">Pause</span><span class="sxs-lookup"><span data-stu-id="ff1cf-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="ff1cf-130">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1cf-130">None</span></span>   |<span data-ttu-id="ff1cf-131">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="ff1cf-132">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="ff1cf-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="ff1cf-133">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="ff1cf-134">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1cf-134">None</span></span>   |<span data-ttu-id="ff1cf-135">Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="ff1cf-136">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="ff1cf-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="ff1cf-137">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="ff1cf-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="ff1cf-138">Получение действующей схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="ff1cf-139">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="ff1cf-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="ff1cf-140">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1cf-140">None</span></span>   |<span data-ttu-id="ff1cf-141">Обновите схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="ff1cf-142">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="ff1cf-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="ff1cf-143">Нет</span><span class="sxs-lookup"><span data-stu-id="ff1cf-143">None</span></span>|<span data-ttu-id="ff1cf-144">Проверка предоставленных учетных данных в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-144">Test provided credentials against target directory.</span></span>|
|[<span data-ttu-id="ff1cf-145">провисионондеманд</span><span class="sxs-lookup"><span data-stu-id="ff1cf-145">provisionOnDemand</span></span>](../api/synchronization-synchronizationjob-provision-on-demand.md)|<span data-ttu-id="ff1cf-146">Коллекция [синчронизатионжобаппликатионпараметерс](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="ff1cf-146">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="ff1cf-147">Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-147">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="ff1cf-148">Ресурс в основном используется для подготовки по требованию.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-148">The resource is primarily used for on-demand provisioning.</span></span> |
## <a name="properties"></a><span data-ttu-id="ff1cf-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff1cf-149">Properties</span></span>

| <span data-ttu-id="ff1cf-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff1cf-150">Property</span></span>      | <span data-ttu-id="ff1cf-151">Тип</span><span class="sxs-lookup"><span data-stu-id="ff1cf-151">Type</span></span>      | <span data-ttu-id="ff1cf-152">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1cf-152">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ff1cf-153">id</span><span class="sxs-lookup"><span data-stu-id="ff1cf-153">id</span></span>             |<span data-ttu-id="ff1cf-154">String</span><span class="sxs-lookup"><span data-stu-id="ff1cf-154">String</span></span>                     |<span data-ttu-id="ff1cf-155">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-155">Unique synchronization job identifier.</span></span> <span data-ttu-id="ff1cf-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-156">Read-only.</span></span>|
|<span data-ttu-id="ff1cf-157">schedule</span><span class="sxs-lookup"><span data-stu-id="ff1cf-157">schedule</span></span>       |[<span data-ttu-id="ff1cf-158">синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="ff1cf-158">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="ff1cf-159">Расписание, используемое для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-159">Schedule used to run the job.</span></span> <span data-ttu-id="ff1cf-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-160">Read-only.</span></span>|
|<span data-ttu-id="ff1cf-161">status</span><span class="sxs-lookup"><span data-stu-id="ff1cf-161">status</span></span>         |[<span data-ttu-id="ff1cf-162">синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="ff1cf-162">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="ff1cf-163">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-163">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="ff1cf-164">синчронизатионжобсеттингс</span><span class="sxs-lookup"><span data-stu-id="ff1cf-164">synchronizationJobSettings</span></span>   |<span data-ttu-id="ff1cf-165">[keyValuePair](keyvaluepair.md);</span><span class="sxs-lookup"><span data-stu-id="ff1cf-165">[keyValuePair](keyvaluepair.md)</span></span>    |<span data-ttu-id="ff1cf-166">Параметры, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-166">Settings associated with the job.</span></span> <span data-ttu-id="ff1cf-167">Некоторые параметры наследуются от шаблона.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-167">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="ff1cf-168">templateId</span><span class="sxs-lookup"><span data-stu-id="ff1cf-168">templateId</span></span>     |<span data-ttu-id="ff1cf-169">String</span><span class="sxs-lookup"><span data-stu-id="ff1cf-169">String</span></span>    |<span data-ttu-id="ff1cf-170">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-170">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff1cf-171">Отношения</span><span class="sxs-lookup"><span data-stu-id="ff1cf-171">Relationships</span></span>
| <span data-ttu-id="ff1cf-172">Связь</span><span class="sxs-lookup"><span data-stu-id="ff1cf-172">Relationship</span></span> | <span data-ttu-id="ff1cf-173">Тип</span><span class="sxs-lookup"><span data-stu-id="ff1cf-173">Type</span></span>   |<span data-ttu-id="ff1cf-174">Описание</span><span class="sxs-lookup"><span data-stu-id="ff1cf-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff1cf-175">схемы</span><span class="sxs-lookup"><span data-stu-id="ff1cf-175">schema</span></span>|[<span data-ttu-id="ff1cf-176">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="ff1cf-176">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="ff1cf-177">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-177">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff1cf-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff1cf-178">JSON representation</span></span>

<span data-ttu-id="ff1cf-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff1cf-179">The following is a JSON representation of the resource.</span></span>

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


