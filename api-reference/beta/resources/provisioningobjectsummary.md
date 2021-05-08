---
title: тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7004a611c3fe36e2ce2d32824a5e9b78e53e61bd
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231915"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="d53d9-103">тип ресурса provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="d53d9-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="d53d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d53d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION]
><span data-ttu-id="d53d9-105">Свойства **действия** **и statusInfo** обесценяются.</span><span class="sxs-lookup"><span data-stu-id="d53d9-105">The **action** and **statusInfo** properties are deprecated.</span></span> <span data-ttu-id="d53d9-106">Действие **свойства** должно быть заменено **provisioningAction**.</span><span class="sxs-lookup"><span data-stu-id="d53d9-106">Property **action** should be replaced by **provisioningAction**.</span></span> <span data-ttu-id="d53d9-107">Состояние **свойстваInfo** должно быть заменено **provisioningStatusInfo**.</span><span class="sxs-lookup"><span data-stu-id="d53d9-107">Property **statusInfo** should be replaced by **provisioningStatusInfo**.</span></span>

<span data-ttu-id="d53d9-108">Представляет действие, выполняемые службой подготовка Azure AD и связанными с ней свойствами.</span><span class="sxs-lookup"><span data-stu-id="d53d9-108">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="d53d9-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d53d9-109">Methods</span></span>

| <span data-ttu-id="d53d9-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d53d9-110">Method</span></span>  | <span data-ttu-id="d53d9-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d53d9-111">Return Type</span></span> | <span data-ttu-id="d53d9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d53d9-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d53d9-113">Список provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="d53d9-113">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="d53d9-114">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="d53d9-114">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="d53d9-115">Получите список всех событий, которые произошли в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d53d9-115">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="d53d9-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d53d9-116">Properties</span></span>

| <span data-ttu-id="d53d9-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d53d9-117">Property</span></span>     | <span data-ttu-id="d53d9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d53d9-118">Type</span></span>        | <span data-ttu-id="d53d9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d53d9-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d53d9-120">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="d53d9-120">provisioningAction</span></span>|<span data-ttu-id="d53d9-121">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-121">string</span></span>|<span data-ttu-id="d53d9-122">Указывает имя действия или имя операции.</span><span class="sxs-lookup"><span data-stu-id="d53d9-122">Indicates the activity name or the operation name.</span></span> <span data-ttu-id="d53d9-123">Возможные значения: `create` `update` , , , , , `delete` `stageddelete` и `disable` `other` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="d53d9-123">Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`.</span></span> <span data-ttu-id="d53d9-124">Список действий, зарегистрированных в журнале, обратитесь к списку действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d53d9-124">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="d53d9-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d53d9-125">activityDateTime</span></span>|<span data-ttu-id="d53d9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d53d9-126">DateTimeOffset</span></span>|<span data-ttu-id="d53d9-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d53d9-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d53d9-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d53d9-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d53d9-129">changeId</span><span class="sxs-lookup"><span data-stu-id="d53d9-129">changeId</span></span>|<span data-ttu-id="d53d9-130">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-130">String</span></span>|<span data-ttu-id="d53d9-131">Уникальный ID этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="d53d9-131">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="d53d9-132">cycleId</span><span class="sxs-lookup"><span data-stu-id="d53d9-132">cycleId</span></span>|<span data-ttu-id="d53d9-133">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-133">String</span></span>|<span data-ttu-id="d53d9-134">Уникальный ID для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="d53d9-134">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="d53d9-135">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="d53d9-135">durationInMilliseconds</span></span>|<span data-ttu-id="d53d9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d53d9-136">Int32</span></span>|<span data-ttu-id="d53d9-137">Указывает, сколько времени потребовалось для завершения этого действия по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="d53d9-137">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="d53d9-138">Измеряется в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="d53d9-138">Measured in milliseconds.</span></span>|
|<span data-ttu-id="d53d9-139">id</span><span class="sxs-lookup"><span data-stu-id="d53d9-139">id</span></span>|<span data-ttu-id="d53d9-140">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-140">String</span></span>| <span data-ttu-id="d53d9-141">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="d53d9-141">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="d53d9-142">Это GUID только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d53d9-142">This is a read-only GUID.</span></span>|
|<span data-ttu-id="d53d9-143">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d53d9-143">initiatedBy</span></span>|[<span data-ttu-id="d53d9-144">initiator</span><span class="sxs-lookup"><span data-stu-id="d53d9-144">initiator</span></span>](initiator.md)|<span data-ttu-id="d53d9-145">Сведения о том, кто инициировал это подготовка.</span><span class="sxs-lookup"><span data-stu-id="d53d9-145">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="d53d9-146">jobId</span><span class="sxs-lookup"><span data-stu-id="d53d9-146">jobId</span></span>|<span data-ttu-id="d53d9-147">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-147">String</span></span>|<span data-ttu-id="d53d9-148">Уникальный ID для всего задания по подготовкам.</span><span class="sxs-lookup"><span data-stu-id="d53d9-148">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="d53d9-149">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="d53d9-149">modifiedProperties</span></span>|<span data-ttu-id="d53d9-150">[измененная коллекцияProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d53d9-150">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="d53d9-151">Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.</span><span class="sxs-lookup"><span data-stu-id="d53d9-151">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="d53d9-152">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="d53d9-152">provisioningSteps</span></span>|<span data-ttu-id="d53d9-153">[provisioningStep](provisioningstep.md) collection</span><span class="sxs-lookup"><span data-stu-id="d53d9-153">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="d53d9-154">Сведения о каждом шаге в области подготовка.</span><span class="sxs-lookup"><span data-stu-id="d53d9-154">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="d53d9-155">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="d53d9-155">servicePrincipal</span></span>|<span data-ttu-id="d53d9-156">Коллекция [servicePrincipal](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="d53d9-156">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="d53d9-157">Представляет принцип службы, используемый для обеспечения.</span><span class="sxs-lookup"><span data-stu-id="d53d9-157">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="d53d9-158">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="d53d9-158">sourceIdentity</span></span>|[<span data-ttu-id="d53d9-159">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="d53d9-159">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="d53d9-160">Сведения о предварительном предоставлении объекта-источника.</span><span class="sxs-lookup"><span data-stu-id="d53d9-160">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="d53d9-161">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="d53d9-161">sourceSystem</span></span>|[<span data-ttu-id="d53d9-162">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="d53d9-162">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="d53d9-163">Сведения о исходных системах объекта, который был закамут.</span><span class="sxs-lookup"><span data-stu-id="d53d9-163">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="d53d9-164">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="d53d9-164">provisioningStatusInfo</span></span>|[<span data-ttu-id="d53d9-165">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="d53d9-165">provisioningStatusInfo</span></span>](provisioningstatusinfo.md)|<span data-ttu-id="d53d9-166">Сведения о состоянии подготовка.</span><span class="sxs-lookup"><span data-stu-id="d53d9-166">Details of provisioning status.</span></span>|
|<span data-ttu-id="d53d9-167">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="d53d9-167">targetIdentity</span></span>|[<span data-ttu-id="d53d9-168">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="d53d9-168">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="d53d9-169">Сведения о предварительном предоставлении целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="d53d9-169">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="d53d9-170">targetSystem</span><span class="sxs-lookup"><span data-stu-id="d53d9-170">targetSystem</span></span>|[<span data-ttu-id="d53d9-171">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="d53d9-171">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="d53d9-172">Сведения о целевой системе объекта.</span><span class="sxs-lookup"><span data-stu-id="d53d9-172">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="d53d9-173">tenantId</span><span class="sxs-lookup"><span data-stu-id="d53d9-173">tenantId</span></span>|<span data-ttu-id="d53d9-174">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-174">String</span></span>|<span data-ttu-id="d53d9-175">Уникальный ID клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d53d9-175">Unique Azure AD tenant ID.</span></span>|
|<span data-ttu-id="d53d9-176">действие (неподготовлено)</span><span class="sxs-lookup"><span data-stu-id="d53d9-176">action (deprecated)</span></span>|<span data-ttu-id="d53d9-177">String</span><span class="sxs-lookup"><span data-stu-id="d53d9-177">String</span></span>|<span data-ttu-id="d53d9-178">Указывает имя действия или имя операции (например, Создание пользователя, добавление участника в группу).</span><span class="sxs-lookup"><span data-stu-id="d53d9-178">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="d53d9-179">Список действий, зарегистрированных в журнале, обратитесь к списку действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d53d9-179">For a list of activities logged, refer to Azure AD activity list.</span></span> <span data-ttu-id="d53d9-180">Это не так.</span><span class="sxs-lookup"><span data-stu-id="d53d9-180">This is deprecated.</span></span> <span data-ttu-id="d53d9-181">Вместо этого используйте provisioningAction.</span><span class="sxs-lookup"><span data-stu-id="d53d9-181">Please use provisioningAction instead.</span></span>|
|<span data-ttu-id="d53d9-182">statusInfo (deprecated)</span><span class="sxs-lookup"><span data-stu-id="d53d9-182">statusInfo (deprecated)</span></span>|[<span data-ttu-id="d53d9-183">statusBase</span><span class="sxs-lookup"><span data-stu-id="d53d9-183">statusBase</span></span>](statusbase.md)|<span data-ttu-id="d53d9-184">Сведения о состоянии подготовка.</span><span class="sxs-lookup"><span data-stu-id="d53d9-184">Details of provisioning status.</span></span> <span data-ttu-id="d53d9-185">Это не так.</span><span class="sxs-lookup"><span data-stu-id="d53d9-185">This is deprecated.</span></span> <span data-ttu-id="d53d9-186">Вместо этого используйте provisioningStatusInfo.</span><span class="sxs-lookup"><span data-stu-id="d53d9-186">Please use provisioningStatusInfo instead.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d53d9-187">Связи</span><span class="sxs-lookup"><span data-stu-id="d53d9-187">Relationships</span></span>

<span data-ttu-id="d53d9-188">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d53d9-188">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d53d9-189">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d53d9-189">JSON representation</span></span>

<span data-ttu-id="d53d9-190">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d53d9-190">The following is a JSON representation of the resource.</span></span>

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
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
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


