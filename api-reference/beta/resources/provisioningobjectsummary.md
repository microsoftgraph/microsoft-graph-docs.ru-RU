---
title: тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2bfe519d6a5cab816bdd35da451221be58105e37
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719404"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="da8e7-103">тип ресурса provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="da8e7-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="da8e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da8e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da8e7-105">Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.</span><span class="sxs-lookup"><span data-stu-id="da8e7-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="da8e7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="da8e7-106">Methods</span></span>

| <span data-ttu-id="da8e7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="da8e7-107">Method</span></span>  | <span data-ttu-id="da8e7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da8e7-108">Return Type</span></span> | <span data-ttu-id="da8e7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="da8e7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="da8e7-110">Список provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="da8e7-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="da8e7-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="da8e7-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="da8e7-112">Получите список всех событий, которые произошли в клиенте.</span><span class="sxs-lookup"><span data-stu-id="da8e7-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="da8e7-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="da8e7-113">Properties</span></span>

| <span data-ttu-id="da8e7-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="da8e7-114">Property</span></span>     | <span data-ttu-id="da8e7-115">Тип</span><span class="sxs-lookup"><span data-stu-id="da8e7-115">Type</span></span>        | <span data-ttu-id="da8e7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="da8e7-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da8e7-117">action</span><span class="sxs-lookup"><span data-stu-id="da8e7-117">action</span></span>|<span data-ttu-id="da8e7-118">String</span><span class="sxs-lookup"><span data-stu-id="da8e7-118">String</span></span>|<span data-ttu-id="da8e7-119">Указывает имя действия или имя операции (например, Создание пользователя, добавление участника в группу).</span><span class="sxs-lookup"><span data-stu-id="da8e7-119">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="da8e7-120">Список действий, зарегистрированных в журнале, обратитесь к списку действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da8e7-120">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="da8e7-121">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="da8e7-121">activityDateTime</span></span>|<span data-ttu-id="da8e7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da8e7-122">DateTimeOffset</span></span>|<span data-ttu-id="da8e7-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="da8e7-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da8e7-124">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="da8e7-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="da8e7-125">changeId</span><span class="sxs-lookup"><span data-stu-id="da8e7-125">changeId</span></span>|<span data-ttu-id="da8e7-126">String</span><span class="sxs-lookup"><span data-stu-id="da8e7-126">String</span></span>|<span data-ttu-id="da8e7-127">Уникальный ID этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="da8e7-127">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="da8e7-128">cycleId</span><span class="sxs-lookup"><span data-stu-id="da8e7-128">cycleId</span></span>|<span data-ttu-id="da8e7-129">String</span><span class="sxs-lookup"><span data-stu-id="da8e7-129">String</span></span>|<span data-ttu-id="da8e7-130">Уникальный ID для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="da8e7-130">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="da8e7-131">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="da8e7-131">durationInMilliseconds</span></span>|<span data-ttu-id="da8e7-132">Int32</span><span class="sxs-lookup"><span data-stu-id="da8e7-132">Int32</span></span>|<span data-ttu-id="da8e7-133">Указывает, сколько времени потребовалось для завершения этого действия по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="da8e7-133">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="da8e7-134">Измеряется в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="da8e7-134">Measured in milliseconds.</span></span>|
|<span data-ttu-id="da8e7-135">id</span><span class="sxs-lookup"><span data-stu-id="da8e7-135">id</span></span>|<span data-ttu-id="da8e7-136">String</span><span class="sxs-lookup"><span data-stu-id="da8e7-136">String</span></span>| <span data-ttu-id="da8e7-137">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="da8e7-137">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="da8e7-138">Это GUID только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da8e7-138">This is a read-only GUID.</span></span>|
|<span data-ttu-id="da8e7-139">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="da8e7-139">initiatedBy</span></span>|[<span data-ttu-id="da8e7-140">initiator</span><span class="sxs-lookup"><span data-stu-id="da8e7-140">initiator</span></span>](initiator.md)|<span data-ttu-id="da8e7-141">Сведения о том, кто инициировал это подготовка.</span><span class="sxs-lookup"><span data-stu-id="da8e7-141">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="da8e7-142">jobId</span><span class="sxs-lookup"><span data-stu-id="da8e7-142">jobId</span></span>|<span data-ttu-id="da8e7-143">String</span><span class="sxs-lookup"><span data-stu-id="da8e7-143">String</span></span>|<span data-ttu-id="da8e7-144">Уникальный ID для всего задания по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="da8e7-144">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="da8e7-145">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="da8e7-145">modifiedProperties</span></span>|<span data-ttu-id="da8e7-146">[измененная коллекцияProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="da8e7-146">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="da8e7-147">Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.</span><span class="sxs-lookup"><span data-stu-id="da8e7-147">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="da8e7-148">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="da8e7-148">provisioningSteps</span></span>|<span data-ttu-id="da8e7-149">[provisioningStep](provisioningstep.md) collection</span><span class="sxs-lookup"><span data-stu-id="da8e7-149">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="da8e7-150">Сведения о каждом шаге в области подготовка.</span><span class="sxs-lookup"><span data-stu-id="da8e7-150">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="da8e7-151">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="da8e7-151">servicePrincipal</span></span>|<span data-ttu-id="da8e7-152">Коллекция [servicePrincipal](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="da8e7-152">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="da8e7-153">Представляет принцип службы, используемый для обеспечения.</span><span class="sxs-lookup"><span data-stu-id="da8e7-153">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="da8e7-154">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="da8e7-154">sourceIdentity</span></span>|[<span data-ttu-id="da8e7-155">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="da8e7-155">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="da8e7-156">Сведения о предварительном предоставлении объекта-источника.</span><span class="sxs-lookup"><span data-stu-id="da8e7-156">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="da8e7-157">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="da8e7-157">sourceSystem</span></span>|[<span data-ttu-id="da8e7-158">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="da8e7-158">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="da8e7-159">Сведения о исходных системах объекта, который был закамут.</span><span class="sxs-lookup"><span data-stu-id="da8e7-159">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="da8e7-160">statusInfo</span><span class="sxs-lookup"><span data-stu-id="da8e7-160">statusInfo</span></span>|[<span data-ttu-id="da8e7-161">statusBase</span><span class="sxs-lookup"><span data-stu-id="da8e7-161">statusBase</span></span>](statusbase.md)|<span data-ttu-id="da8e7-162">Сведения о состоянии подготовка.</span><span class="sxs-lookup"><span data-stu-id="da8e7-162">Details of provisioning status.</span></span>|
|<span data-ttu-id="da8e7-163">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="da8e7-163">targetIdentity</span></span>|[<span data-ttu-id="da8e7-164">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="da8e7-164">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="da8e7-165">Сведения о предварительном предоставлении целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="da8e7-165">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="da8e7-166">targetSystem</span><span class="sxs-lookup"><span data-stu-id="da8e7-166">targetSystem</span></span>|[<span data-ttu-id="da8e7-167">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="da8e7-167">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="da8e7-168">Сведения о целевой системе объекта.</span><span class="sxs-lookup"><span data-stu-id="da8e7-168">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="da8e7-169">tenantId</span><span class="sxs-lookup"><span data-stu-id="da8e7-169">tenantId</span></span>|<span data-ttu-id="da8e7-170">String</span><span class="sxs-lookup"><span data-stu-id="da8e7-170">String</span></span>|<span data-ttu-id="da8e7-171">Уникальный ID клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da8e7-171">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da8e7-172">Связи</span><span class="sxs-lookup"><span data-stu-id="da8e7-172">Relationships</span></span>

<span data-ttu-id="da8e7-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="da8e7-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da8e7-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="da8e7-174">JSON representation</span></span>

<span data-ttu-id="da8e7-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da8e7-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
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
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
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


