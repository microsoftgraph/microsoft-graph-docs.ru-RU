---
title: тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d9852745ed14cacd47389da5031cb83af306e2d0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241553"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="b9906-103">тип ресурса provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="b9906-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="b9906-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9906-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b9906-105">Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.</span><span class="sxs-lookup"><span data-stu-id="b9906-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="b9906-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b9906-106">Methods</span></span>

| <span data-ttu-id="b9906-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b9906-107">Method</span></span>  | <span data-ttu-id="b9906-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b9906-108">Return Type</span></span> | <span data-ttu-id="b9906-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b9906-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b9906-110">Список provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="b9906-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="b9906-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="b9906-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="b9906-112">Получите список всех событий, которые произошли в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b9906-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="b9906-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9906-113">Properties</span></span>

| <span data-ttu-id="b9906-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9906-114">Property</span></span>     | <span data-ttu-id="b9906-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b9906-115">Type</span></span>        | <span data-ttu-id="b9906-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b9906-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9906-117">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="b9906-117">provisioningAction</span></span>|<span data-ttu-id="b9906-118">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="b9906-118">provisioningAction</span></span>|<span data-ttu-id="b9906-119">Указывает имя действия или имя операции.</span><span class="sxs-lookup"><span data-stu-id="b9906-119">Indicates the activity name or the operation name.</span></span> <span data-ttu-id="b9906-120">Возможные значения: `create` `update` , , , , , `delete` `stageddelete` и `disable` `other` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="b9906-120">Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`.</span></span> <span data-ttu-id="b9906-121">Список действий, зарегистрированных в журнале, обратитесь к списку действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b9906-121">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="b9906-122">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="b9906-122">activityDateTime</span></span>|<span data-ttu-id="b9906-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9906-123">DateTimeOffset</span></span>|<span data-ttu-id="b9906-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b9906-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9906-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b9906-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b9906-126">changeId</span><span class="sxs-lookup"><span data-stu-id="b9906-126">changeId</span></span>|<span data-ttu-id="b9906-127">Строка</span><span class="sxs-lookup"><span data-stu-id="b9906-127">String</span></span>|<span data-ttu-id="b9906-128">Уникальный ID этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="b9906-128">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="b9906-129">cycleId</span><span class="sxs-lookup"><span data-stu-id="b9906-129">cycleId</span></span>|<span data-ttu-id="b9906-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b9906-130">String</span></span>|<span data-ttu-id="b9906-131">Уникальный ID для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="b9906-131">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="b9906-132">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="b9906-132">durationInMilliseconds</span></span>|<span data-ttu-id="b9906-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b9906-133">Int32</span></span>|<span data-ttu-id="b9906-134">Указывает, сколько времени потребовалось для завершения этого действия по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="b9906-134">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="b9906-135">Измеряется в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="b9906-135">Measured in milliseconds.</span></span>|
|<span data-ttu-id="b9906-136">id</span><span class="sxs-lookup"><span data-stu-id="b9906-136">id</span></span>|<span data-ttu-id="b9906-137">String</span><span class="sxs-lookup"><span data-stu-id="b9906-137">String</span></span>| <span data-ttu-id="b9906-138">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="b9906-138">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="b9906-139">Это GUID только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9906-139">This is a read-only GUID.</span></span>|
|<span data-ttu-id="b9906-140">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="b9906-140">initiatedBy</span></span>|[<span data-ttu-id="b9906-141">initiator</span><span class="sxs-lookup"><span data-stu-id="b9906-141">initiator</span></span>](initiator.md)|<span data-ttu-id="b9906-142">Сведения о том, кто инициировал это подготовка.</span><span class="sxs-lookup"><span data-stu-id="b9906-142">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="b9906-143">jobId</span><span class="sxs-lookup"><span data-stu-id="b9906-143">jobId</span></span>|<span data-ttu-id="b9906-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b9906-144">String</span></span>|<span data-ttu-id="b9906-145">Уникальный ID для всего задания по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="b9906-145">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="b9906-146">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b9906-146">modifiedProperties</span></span>|<span data-ttu-id="b9906-147">[измененная коллекцияProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b9906-147">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="b9906-148">Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.</span><span class="sxs-lookup"><span data-stu-id="b9906-148">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="b9906-149">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="b9906-149">provisioningSteps</span></span>|<span data-ttu-id="b9906-150">[provisioningStep](provisioningstep.md) collection</span><span class="sxs-lookup"><span data-stu-id="b9906-150">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="b9906-151">Сведения о каждом шаге в области подготовка.</span><span class="sxs-lookup"><span data-stu-id="b9906-151">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="b9906-152">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b9906-152">servicePrincipal</span></span>|<span data-ttu-id="b9906-153">Коллекция [servicePrincipal](provisioningserviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="b9906-153">[servicePrincipal](provisioningserviceprincipal.md) collection</span></span>|<span data-ttu-id="b9906-154">Представляет принцип службы, используемый для обеспечения.</span><span class="sxs-lookup"><span data-stu-id="b9906-154">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="b9906-155">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="b9906-155">sourceIdentity</span></span>|[<span data-ttu-id="b9906-156">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="b9906-156">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="b9906-157">Сведения о предварительном предоставлении объекта-источника.</span><span class="sxs-lookup"><span data-stu-id="b9906-157">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="b9906-158">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="b9906-158">sourceSystem</span></span>|[<span data-ttu-id="b9906-159">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="b9906-159">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="b9906-160">Сведения о исходных системах объекта, который был закамут.</span><span class="sxs-lookup"><span data-stu-id="b9906-160">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="b9906-161">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="b9906-161">provisioningStatusInfo</span></span>|[<span data-ttu-id="b9906-162">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="b9906-162">provisioningStatusInfo</span></span>](provisioningstatusinfo.md)|<span data-ttu-id="b9906-163">Сведения о состоянии подготовка.</span><span class="sxs-lookup"><span data-stu-id="b9906-163">Details of provisioning status.</span></span>|
|<span data-ttu-id="b9906-164">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="b9906-164">targetIdentity</span></span>|[<span data-ttu-id="b9906-165">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="b9906-165">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="b9906-166">Сведения о предварительном предоставлении целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="b9906-166">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="b9906-167">targetSystem</span><span class="sxs-lookup"><span data-stu-id="b9906-167">targetSystem</span></span>|[<span data-ttu-id="b9906-168">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="b9906-168">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="b9906-169">Сведения о целевой системе объекта.</span><span class="sxs-lookup"><span data-stu-id="b9906-169">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="b9906-170">tenantId</span><span class="sxs-lookup"><span data-stu-id="b9906-170">tenantId</span></span>|<span data-ttu-id="b9906-171">String</span><span class="sxs-lookup"><span data-stu-id="b9906-171">String</span></span>|<span data-ttu-id="b9906-172">Уникальный ID клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b9906-172">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9906-173">Связи</span><span class="sxs-lookup"><span data-stu-id="b9906-173">Relationships</span></span>

<span data-ttu-id="b9906-174">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9906-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9906-175">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9906-175">JSON representation</span></span>

<span data-ttu-id="b9906-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9906-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


