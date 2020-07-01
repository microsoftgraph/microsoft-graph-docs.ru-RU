---
title: Тип ресурса Синчронизатионжоб
description: Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 890da6054328da8619ede99de925b941bd41e20a
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006963"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="2d5f4-103">Тип ресурса Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2d5f4-103">synchronizationJob resource type</span></span>

<span data-ttu-id="2d5f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d5f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d5f4-105">Выполняет синхронизацию с периодического выполнения в фоновом режиме, опрашивает изменения в одном каталоге и помещает их в другой каталог.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="2d5f4-106">Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="2d5f4-107">В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="2d5f4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2d5f4-108">Methods</span></span>

| <span data-ttu-id="2d5f4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2d5f4-109">Method</span></span>        | <span data-ttu-id="2d5f4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d5f4-110">Return Type</span></span>               | <span data-ttu-id="2d5f4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5f4-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="2d5f4-112">Список</span><span class="sxs-lookup"><span data-stu-id="2d5f4-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="2d5f4-113">Коллекция [синчронизатионжоб](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="2d5f4-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="2d5f4-114">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="2d5f4-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="2d5f4-115">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2d5f4-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="2d5f4-116">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2d5f4-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="2d5f4-117">Чтение свойств и связей объекта Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|<span data-ttu-id="2d5f4-118">[Создание](../api/synchronization-synchronizationjob-post.md);</span><span class="sxs-lookup"><span data-stu-id="2d5f4-118">[Create](../api/synchronization-synchronizationjob-post.md)</span></span>         |[<span data-ttu-id="2d5f4-119">синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2d5f4-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="2d5f4-120">Создание нового задания для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="2d5f4-121">Начало</span><span class="sxs-lookup"><span data-stu-id="2d5f4-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="2d5f4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2d5f4-122">None</span></span>   |<span data-ttu-id="2d5f4-123">Запуск синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-123">Start synchronization.</span></span> <span data-ttu-id="2d5f4-124">Если задание приостановлено, оно продолжается с того места, где было приостановлено задание.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="2d5f4-125">Если задание находится в карантине, статус карантина очищается.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="2d5f4-126">Restart</span><span class="sxs-lookup"><span data-stu-id="2d5f4-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="2d5f4-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2d5f4-127">None</span></span>   |<span data-ttu-id="2d5f4-128">Принудительно запустить задание и повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="2d5f4-129">Pause</span><span class="sxs-lookup"><span data-stu-id="2d5f4-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="2d5f4-130">Нет</span><span class="sxs-lookup"><span data-stu-id="2d5f4-130">None</span></span>   |<span data-ttu-id="2d5f4-131">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="2d5f4-132">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="2d5f4-133">Delete</span><span class="sxs-lookup"><span data-stu-id="2d5f4-133">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="2d5f4-134">Нет</span><span class="sxs-lookup"><span data-stu-id="2d5f4-134">None</span></span>   |<span data-ttu-id="2d5f4-135">Остановите синхронизацию и окончательно удалите все состояния, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="2d5f4-136">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2d5f4-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="2d5f4-137">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2d5f4-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="2d5f4-138">Получение действующей схемы синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="2d5f4-139">Обновление Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2d5f4-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="2d5f4-140">Нет</span><span class="sxs-lookup"><span data-stu-id="2d5f4-140">None</span></span>   |<span data-ttu-id="2d5f4-141">Обновите схему синхронизации задания.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="2d5f4-142">Проверка учетных данных</span><span class="sxs-lookup"><span data-stu-id="2d5f4-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="2d5f4-143">Нет</span><span class="sxs-lookup"><span data-stu-id="2d5f4-143">None</span></span>|<span data-ttu-id="2d5f4-144">Проверка предоставленных учетных данных в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-144">Test provided credentials against target directory.</span></span>|
|[<span data-ttu-id="2d5f4-145">провисионондеманд</span><span class="sxs-lookup"><span data-stu-id="2d5f4-145">provisionOnDemand</span></span>](../api/synchronization-synchronizationjob-provision-on-demand.md)|<span data-ttu-id="2d5f4-146">Коллекция [синчронизатионжобаппликатионпараметерс](../resources/synchronization-synchronizationjobapplicationparameters.md)</span><span class="sxs-lookup"><span data-stu-id="2d5f4-146">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="2d5f4-147">Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-147">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="2d5f4-148">Ресурс в основном используется для подготовки по требованию.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-148">The resource is primarily used for on-demand provisioning.</span></span> |
## <a name="properties"></a><span data-ttu-id="2d5f4-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d5f4-149">Properties</span></span>

| <span data-ttu-id="2d5f4-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d5f4-150">Property</span></span>      | <span data-ttu-id="2d5f4-151">Тип</span><span class="sxs-lookup"><span data-stu-id="2d5f4-151">Type</span></span>      | <span data-ttu-id="2d5f4-152">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5f4-152">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="2d5f4-153">id</span><span class="sxs-lookup"><span data-stu-id="2d5f4-153">id</span></span>             |<span data-ttu-id="2d5f4-154">String</span><span class="sxs-lookup"><span data-stu-id="2d5f4-154">String</span></span>                     |<span data-ttu-id="2d5f4-155">Уникальный идентификатор задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-155">Unique synchronization job identifier.</span></span> <span data-ttu-id="2d5f4-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-156">Read-only.</span></span>|
|<span data-ttu-id="2d5f4-157">schedule</span><span class="sxs-lookup"><span data-stu-id="2d5f4-157">schedule</span></span>       |[<span data-ttu-id="2d5f4-158">синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="2d5f4-158">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="2d5f4-159">Расписание, используемое для запуска задания.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-159">Schedule used to run the job.</span></span> <span data-ttu-id="2d5f4-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-160">Read-only.</span></span>|
|<span data-ttu-id="2d5f4-161">status</span><span class="sxs-lookup"><span data-stu-id="2d5f4-161">status</span></span>         |[<span data-ttu-id="2d5f4-162">синчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="2d5f4-162">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="2d5f4-163">Состояние задания, которое включает время последнего запуска задания, текущее состояние задания и ошибки.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-163">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="2d5f4-164">синчронизатионжобсеттингс</span><span class="sxs-lookup"><span data-stu-id="2d5f4-164">synchronizationJobSettings</span></span>   |<span data-ttu-id="2d5f4-165">[keyValuePair](keyvaluepair.md);</span><span class="sxs-lookup"><span data-stu-id="2d5f4-165">[keyValuePair](keyvaluepair.md)</span></span>    |<span data-ttu-id="2d5f4-166">Параметры, связанные с заданием.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-166">Settings associated with the job.</span></span> <span data-ttu-id="2d5f4-167">Некоторые параметры наследуются от шаблона.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-167">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="2d5f4-168">templateId</span><span class="sxs-lookup"><span data-stu-id="2d5f4-168">templateId</span></span>     |<span data-ttu-id="2d5f4-169">String</span><span class="sxs-lookup"><span data-stu-id="2d5f4-169">String</span></span>    |<span data-ttu-id="2d5f4-170">Идентификатор [шаблона синхронизации](synchronization-synchronizationtemplate.md) , на котором основано это задание.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-170">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d5f4-171">Связи</span><span class="sxs-lookup"><span data-stu-id="2d5f4-171">Relationships</span></span>
| <span data-ttu-id="2d5f4-172">Связь</span><span class="sxs-lookup"><span data-stu-id="2d5f4-172">Relationship</span></span> | <span data-ttu-id="2d5f4-173">Тип</span><span class="sxs-lookup"><span data-stu-id="2d5f4-173">Type</span></span>   |<span data-ttu-id="2d5f4-174">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5f4-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d5f4-175">схемы</span><span class="sxs-lookup"><span data-stu-id="2d5f4-175">schema</span></span>|[<span data-ttu-id="2d5f4-176">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="2d5f4-176">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="2d5f4-177">Схема синхронизации, настроенная для задания.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-177">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d5f4-178">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2d5f4-178">JSON representation</span></span>

<span data-ttu-id="2d5f4-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d5f4-179">The following is a JSON representation of the resource.</span></span>

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
