---
title: Тип ресурса Провисионингобжектсуммари
description: Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eabbb0c0cd1cd692ad6ebc5a346c46473161b1
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394605"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="57493-103">Тип ресурса Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="57493-103">provisioningObjectSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57493-104">Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.</span><span class="sxs-lookup"><span data-stu-id="57493-104">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="57493-105">Методы</span><span class="sxs-lookup"><span data-stu-id="57493-105">Methods</span></span>

| <span data-ttu-id="57493-106">Метод</span><span class="sxs-lookup"><span data-stu-id="57493-106">Method</span></span>       | <span data-ttu-id="57493-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57493-107">Return Type</span></span> | <span data-ttu-id="57493-108">Описание</span><span class="sxs-lookup"><span data-stu-id="57493-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="57493-109">Список Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="57493-109">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="57493-110">провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="57493-110">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="57493-111">Получение списка всех событий подготовки, произошедших в клиенте.</span><span class="sxs-lookup"><span data-stu-id="57493-111">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="57493-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="57493-112">Properties</span></span>

| <span data-ttu-id="57493-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="57493-113">Property</span></span>     | <span data-ttu-id="57493-114">Тип</span><span class="sxs-lookup"><span data-stu-id="57493-114">Type</span></span>        | <span data-ttu-id="57493-115">Описание</span><span class="sxs-lookup"><span data-stu-id="57493-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57493-116">action</span><span class="sxs-lookup"><span data-stu-id="57493-116">action</span></span>|<span data-ttu-id="57493-117">String</span><span class="sxs-lookup"><span data-stu-id="57493-117">String</span></span>|<span data-ttu-id="57493-118">Указывает имя действия или имя операции (например, создание пользователя, Добавление участника в группу).</span><span class="sxs-lookup"><span data-stu-id="57493-118">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="57493-119">Список действий, регистрируемых в журнале, можно найти в списке действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="57493-119">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="57493-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="57493-120">activityDateTime</span></span>|<span data-ttu-id="57493-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57493-121">DateTimeOffset</span></span>|<span data-ttu-id="57493-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="57493-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="57493-124">чанжеид</span><span class="sxs-lookup"><span data-stu-id="57493-124">changeId</span></span>|<span data-ttu-id="57493-125">String</span><span class="sxs-lookup"><span data-stu-id="57493-125">String</span></span>|<span data-ttu-id="57493-126">Уникальный идентификатор этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="57493-126">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="57493-127">циклеид</span><span class="sxs-lookup"><span data-stu-id="57493-127">cycleId</span></span>|<span data-ttu-id="57493-128">String</span><span class="sxs-lookup"><span data-stu-id="57493-128">String</span></span>|<span data-ttu-id="57493-129">Уникальный идентификатор для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="57493-129">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="57493-130">дуратионинмиллисекондс</span><span class="sxs-lookup"><span data-stu-id="57493-130">durationInMilliseconds</span></span>|<span data-ttu-id="57493-131">Int32</span><span class="sxs-lookup"><span data-stu-id="57493-131">Int32</span></span>|<span data-ttu-id="57493-132">Указывает время завершения этого действия подготовки.</span><span class="sxs-lookup"><span data-stu-id="57493-132">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="57493-133">Измеряется в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="57493-133">Measured in milliseconds.</span></span>|
|<span data-ttu-id="57493-134">id</span><span class="sxs-lookup"><span data-stu-id="57493-134">id</span></span>|<span data-ttu-id="57493-135">String</span><span class="sxs-lookup"><span data-stu-id="57493-135">String</span></span>| <span data-ttu-id="57493-136">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="57493-136">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="57493-137">Это GUID, предназначенный только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57493-137">This is a read-only GUID.</span></span>|
|<span data-ttu-id="57493-138">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="57493-138">initiatedBy</span></span>|[<span data-ttu-id="57493-139">initiator</span><span class="sxs-lookup"><span data-stu-id="57493-139">initiator</span></span>](initiator.md)|<span data-ttu-id="57493-140">Сведения о том, кто инициировал эту подготовку.</span><span class="sxs-lookup"><span data-stu-id="57493-140">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="57493-141">jobId</span><span class="sxs-lookup"><span data-stu-id="57493-141">jobId</span></span>|<span data-ttu-id="57493-142">String</span><span class="sxs-lookup"><span data-stu-id="57493-142">String</span></span>|<span data-ttu-id="57493-143">Уникальный идентификатор для полного задания подготовки.</span><span class="sxs-lookup"><span data-stu-id="57493-143">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="57493-144">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="57493-144">modifiedProperties</span></span>|<span data-ttu-id="57493-145">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="57493-145">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="57493-146">Сведения о каждом свойстве, которое было изменено в этом действии подготовки для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="57493-146">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="57493-147">провисионингстепс</span><span class="sxs-lookup"><span data-stu-id="57493-147">provisioningSteps</span></span>|<span data-ttu-id="57493-148">Коллекция [провисионингстеп](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="57493-148">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="57493-149">Сведения о каждом этапе подготовки.</span><span class="sxs-lookup"><span data-stu-id="57493-149">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="57493-150">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="57493-150">servicePrincipal</span></span>|<span data-ttu-id="57493-151">Коллекция [servicePrincipal](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="57493-151">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="57493-152">Представляет участника службы, используемого для подготовки.</span><span class="sxs-lookup"><span data-stu-id="57493-152">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="57493-153">саурцеидентити</span><span class="sxs-lookup"><span data-stu-id="57493-153">sourceIdentity</span></span>|[<span data-ttu-id="57493-154">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="57493-154">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="57493-155">Сведения о подготовленном исходном объекте.</span><span class="sxs-lookup"><span data-stu-id="57493-155">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="57493-156">саурцесистем</span><span class="sxs-lookup"><span data-stu-id="57493-156">sourceSystem</span></span>|[<span data-ttu-id="57493-157">провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="57493-157">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="57493-158">Сведения об исходной системе подготовленного объекта.</span><span class="sxs-lookup"><span data-stu-id="57493-158">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="57493-159">статусинфо</span><span class="sxs-lookup"><span data-stu-id="57493-159">statusInfo</span></span>|[<span data-ttu-id="57493-160">statusBase</span><span class="sxs-lookup"><span data-stu-id="57493-160">statusBase</span></span>](statusbase.md)|<span data-ttu-id="57493-161">Сведения о состоянии подготовки.</span><span class="sxs-lookup"><span data-stu-id="57493-161">Details of provisioning status.</span></span>|
|<span data-ttu-id="57493-162">таржетидентити</span><span class="sxs-lookup"><span data-stu-id="57493-162">targetIdentity</span></span>|[<span data-ttu-id="57493-163">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="57493-163">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="57493-164">Сведения о подготовленном целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="57493-164">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="57493-165">таржетсистем</span><span class="sxs-lookup"><span data-stu-id="57493-165">targetSystem</span></span>|[<span data-ttu-id="57493-166">провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="57493-166">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="57493-167">Сведения о целевой системе объекта, подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="57493-167">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="57493-168">tenantId</span><span class="sxs-lookup"><span data-stu-id="57493-168">tenantId</span></span>|<span data-ttu-id="57493-169">String</span><span class="sxs-lookup"><span data-stu-id="57493-169">String</span></span>|<span data-ttu-id="57493-170">Уникальный идентификатор клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="57493-170">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57493-171">Связи</span><span class="sxs-lookup"><span data-stu-id="57493-171">Relationships</span></span>

<span data-ttu-id="57493-172">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="57493-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57493-173">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="57493-173">JSON representation</span></span>

<span data-ttu-id="57493-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57493-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
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
