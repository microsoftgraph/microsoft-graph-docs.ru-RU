---
title: Тип ресурса provisioningObjectSummary
description: Представляет действие, выполняемые службой предоставления Azure AD, и связанные с ней свойства.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2b1add3f614fd05060df2dfc45b84a46f19dd134
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156352"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="fddfd-103">Тип ресурса provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="fddfd-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="fddfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fddfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fddfd-105">Представляет действие, выполняемые службой предоставления Azure AD, и связанные с ней свойства.</span><span class="sxs-lookup"><span data-stu-id="fddfd-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="fddfd-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fddfd-106">Methods</span></span>

| <span data-ttu-id="fddfd-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fddfd-107">Method</span></span>  | <span data-ttu-id="fddfd-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fddfd-108">Return Type</span></span> | <span data-ttu-id="fddfd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fddfd-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fddfd-110">Список provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="fddfd-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="fddfd-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="fddfd-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="fddfd-112">Получите список всех событий предоставления, произошедших в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fddfd-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="fddfd-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="fddfd-113">Properties</span></span>

| <span data-ttu-id="fddfd-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="fddfd-114">Property</span></span>     | <span data-ttu-id="fddfd-115">Тип</span><span class="sxs-lookup"><span data-stu-id="fddfd-115">Type</span></span>        | <span data-ttu-id="fddfd-116">Описание</span><span class="sxs-lookup"><span data-stu-id="fddfd-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fddfd-117">action</span><span class="sxs-lookup"><span data-stu-id="fddfd-117">action</span></span>|<span data-ttu-id="fddfd-118">String</span><span class="sxs-lookup"><span data-stu-id="fddfd-118">String</span></span>|<span data-ttu-id="fddfd-119">Указывает имя действия или имя операции (например, "Создать пользователя", "Добавить участника в группу").</span><span class="sxs-lookup"><span data-stu-id="fddfd-119">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="fddfd-120">Список зарегистрированных действий можно найти в списке действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fddfd-120">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="fddfd-121">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="fddfd-121">activityDateTime</span></span>|<span data-ttu-id="fddfd-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fddfd-122">DateTimeOffset</span></span>|<span data-ttu-id="fddfd-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fddfd-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fddfd-125">changeId</span><span class="sxs-lookup"><span data-stu-id="fddfd-125">changeId</span></span>|<span data-ttu-id="fddfd-126">String</span><span class="sxs-lookup"><span data-stu-id="fddfd-126">String</span></span>|<span data-ttu-id="fddfd-127">Уникальный ИД этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="fddfd-127">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="fddfd-128">cycleId</span><span class="sxs-lookup"><span data-stu-id="fddfd-128">cycleId</span></span>|<span data-ttu-id="fddfd-129">String</span><span class="sxs-lookup"><span data-stu-id="fddfd-129">String</span></span>|<span data-ttu-id="fddfd-130">Уникальный ИД для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="fddfd-130">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="fddfd-131">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="fddfd-131">durationInMilliseconds</span></span>|<span data-ttu-id="fddfd-132">Int32</span><span class="sxs-lookup"><span data-stu-id="fddfd-132">Int32</span></span>|<span data-ttu-id="fddfd-133">Указывает, сколько времени потребовалось для завершения этого действия.</span><span class="sxs-lookup"><span data-stu-id="fddfd-133">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="fddfd-134">Измеряется в миллисекунах.</span><span class="sxs-lookup"><span data-stu-id="fddfd-134">Measured in milliseconds.</span></span>|
|<span data-ttu-id="fddfd-135">id</span><span class="sxs-lookup"><span data-stu-id="fddfd-135">id</span></span>|<span data-ttu-id="fddfd-136">String</span><span class="sxs-lookup"><span data-stu-id="fddfd-136">String</span></span>| <span data-ttu-id="fddfd-137">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="fddfd-137">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="fddfd-138">Это GUID только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fddfd-138">This is a read-only GUID.</span></span>|
|<span data-ttu-id="fddfd-139">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="fddfd-139">initiatedBy</span></span>|[<span data-ttu-id="fddfd-140">initiator</span><span class="sxs-lookup"><span data-stu-id="fddfd-140">initiator</span></span>](initiator.md)|<span data-ttu-id="fddfd-141">Сведения о том, кто инициировал эту подготовка.</span><span class="sxs-lookup"><span data-stu-id="fddfd-141">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="fddfd-142">jobId</span><span class="sxs-lookup"><span data-stu-id="fddfd-142">jobId</span></span>|<span data-ttu-id="fddfd-143">String</span><span class="sxs-lookup"><span data-stu-id="fddfd-143">String</span></span>|<span data-ttu-id="fddfd-144">Уникальный ИД для всего задания по обеспечению.</span><span class="sxs-lookup"><span data-stu-id="fddfd-144">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="fddfd-145">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="fddfd-145">modifiedProperties</span></span>|<span data-ttu-id="fddfd-146">[Коллекция modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="fddfd-146">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="fddfd-147">Сведения о каждом свойстве, которое было изменено в этом действии по обеспечению этого объекта.</span><span class="sxs-lookup"><span data-stu-id="fddfd-147">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="fddfd-148">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="fddfd-148">provisioningSteps</span></span>|<span data-ttu-id="fddfd-149">[Коллекция provisioningStep](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="fddfd-149">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="fddfd-150">Подробные сведения о каждом шаге в предоставлении.</span><span class="sxs-lookup"><span data-stu-id="fddfd-150">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="fddfd-151">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="fddfd-151">servicePrincipal</span></span>|<span data-ttu-id="fddfd-152">Коллекция [servicePrincipal](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="fddfd-152">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="fddfd-153">Представляет основной сервис, используемый для предоставления.</span><span class="sxs-lookup"><span data-stu-id="fddfd-153">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="fddfd-154">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="fddfd-154">sourceIdentity</span></span>|[<span data-ttu-id="fddfd-155">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="fddfd-155">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="fddfd-156">Сведения о объекте-источнике, который необходимо подготовка.</span><span class="sxs-lookup"><span data-stu-id="fddfd-156">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="fddfd-157">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="fddfd-157">sourceSystem</span></span>|[<span data-ttu-id="fddfd-158">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="fddfd-158">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="fddfd-159">Сведения об источнике системы для объекта, который необходимо подготовка.</span><span class="sxs-lookup"><span data-stu-id="fddfd-159">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="fddfd-160">statusInfo</span><span class="sxs-lookup"><span data-stu-id="fddfd-160">statusInfo</span></span>|[<span data-ttu-id="fddfd-161">statusBase</span><span class="sxs-lookup"><span data-stu-id="fddfd-161">statusBase</span></span>](statusbase.md)|<span data-ttu-id="fddfd-162">Сведения о состоянии предоставления.</span><span class="sxs-lookup"><span data-stu-id="fddfd-162">Details of provisioning status.</span></span>|
|<span data-ttu-id="fddfd-163">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="fddfd-163">targetIdentity</span></span>|[<span data-ttu-id="fddfd-164">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="fddfd-164">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="fddfd-165">Сведения о подготовках целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="fddfd-165">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="fddfd-166">targetSystem</span><span class="sxs-lookup"><span data-stu-id="fddfd-166">targetSystem</span></span>|[<span data-ttu-id="fddfd-167">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="fddfd-167">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="fddfd-168">Сведения о целевой системе для объекта, который необходимо подготовка.</span><span class="sxs-lookup"><span data-stu-id="fddfd-168">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="fddfd-169">tenantId</span><span class="sxs-lookup"><span data-stu-id="fddfd-169">tenantId</span></span>|<span data-ttu-id="fddfd-170">String</span><span class="sxs-lookup"><span data-stu-id="fddfd-170">String</span></span>|<span data-ttu-id="fddfd-171">Уникальный ИД клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fddfd-171">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fddfd-172">Связи</span><span class="sxs-lookup"><span data-stu-id="fddfd-172">Relationships</span></span>

<span data-ttu-id="fddfd-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fddfd-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fddfd-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fddfd-174">JSON representation</span></span>

<span data-ttu-id="fddfd-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fddfd-175">The following is a JSON representation of the resource.</span></span>

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


