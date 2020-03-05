---
title: Тип ресурса Провисионингобжектсуммари
description: Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ed6b760af60900436d22da4ae1302f458d50c4c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521343"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="eb3d0-103">Тип ресурса Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="eb3d0-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="eb3d0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb3d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb3d0-105">Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="eb3d0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="eb3d0-106">Methods</span></span>

| <span data-ttu-id="eb3d0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="eb3d0-107">Method</span></span>       | <span data-ttu-id="eb3d0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb3d0-108">Return Type</span></span> | <span data-ttu-id="eb3d0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="eb3d0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb3d0-110">Список Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="eb3d0-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="eb3d0-111">провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="eb3d0-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="eb3d0-112">Получение списка всех событий подготовки, произошедших в клиенте.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="eb3d0-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb3d0-113">Properties</span></span>

| <span data-ttu-id="eb3d0-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb3d0-114">Property</span></span>     | <span data-ttu-id="eb3d0-115">Тип</span><span class="sxs-lookup"><span data-stu-id="eb3d0-115">Type</span></span>        | <span data-ttu-id="eb3d0-116">Описание</span><span class="sxs-lookup"><span data-stu-id="eb3d0-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb3d0-117">action</span><span class="sxs-lookup"><span data-stu-id="eb3d0-117">action</span></span>|<span data-ttu-id="eb3d0-118">String</span><span class="sxs-lookup"><span data-stu-id="eb3d0-118">String</span></span>|<span data-ttu-id="eb3d0-119">Указывает имя действия или имя операции (например, создание пользователя, Добавление участника в группу).</span><span class="sxs-lookup"><span data-stu-id="eb3d0-119">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="eb3d0-120">Список действий, регистрируемых в журнале, можно найти в списке действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-120">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="eb3d0-121">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="eb3d0-121">activityDateTime</span></span>|<span data-ttu-id="eb3d0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb3d0-122">DateTimeOffset</span></span>|<span data-ttu-id="eb3d0-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eb3d0-125">чанжеид</span><span class="sxs-lookup"><span data-stu-id="eb3d0-125">changeId</span></span>|<span data-ttu-id="eb3d0-126">String</span><span class="sxs-lookup"><span data-stu-id="eb3d0-126">String</span></span>|<span data-ttu-id="eb3d0-127">Уникальный идентификатор этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-127">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="eb3d0-128">циклеид</span><span class="sxs-lookup"><span data-stu-id="eb3d0-128">cycleId</span></span>|<span data-ttu-id="eb3d0-129">String</span><span class="sxs-lookup"><span data-stu-id="eb3d0-129">String</span></span>|<span data-ttu-id="eb3d0-130">Уникальный идентификатор для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-130">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="eb3d0-131">дуратионинмиллисекондс</span><span class="sxs-lookup"><span data-stu-id="eb3d0-131">durationInMilliseconds</span></span>|<span data-ttu-id="eb3d0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="eb3d0-132">Int32</span></span>|<span data-ttu-id="eb3d0-133">Указывает время завершения этого действия подготовки.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-133">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="eb3d0-134">Измеряется в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-134">Measured in milliseconds.</span></span>|
|<span data-ttu-id="eb3d0-135">id</span><span class="sxs-lookup"><span data-stu-id="eb3d0-135">id</span></span>|<span data-ttu-id="eb3d0-136">String</span><span class="sxs-lookup"><span data-stu-id="eb3d0-136">String</span></span>| <span data-ttu-id="eb3d0-137">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-137">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="eb3d0-138">Это GUID, предназначенный только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-138">This is a read-only GUID.</span></span>|
|<span data-ttu-id="eb3d0-139">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="eb3d0-139">initiatedBy</span></span>|[<span data-ttu-id="eb3d0-140">initiator</span><span class="sxs-lookup"><span data-stu-id="eb3d0-140">initiator</span></span>](initiator.md)|<span data-ttu-id="eb3d0-141">Сведения о том, кто инициировал эту подготовку.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-141">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="eb3d0-142">jobId</span><span class="sxs-lookup"><span data-stu-id="eb3d0-142">jobId</span></span>|<span data-ttu-id="eb3d0-143">String</span><span class="sxs-lookup"><span data-stu-id="eb3d0-143">String</span></span>|<span data-ttu-id="eb3d0-144">Уникальный идентификатор для полного задания подготовки.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-144">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="eb3d0-145">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="eb3d0-145">modifiedProperties</span></span>|<span data-ttu-id="eb3d0-146">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="eb3d0-146">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="eb3d0-147">Сведения о каждом свойстве, которое было изменено в этом действии подготовки для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-147">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="eb3d0-148">провисионингстепс</span><span class="sxs-lookup"><span data-stu-id="eb3d0-148">provisioningSteps</span></span>|<span data-ttu-id="eb3d0-149">Коллекция [провисионингстеп](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="eb3d0-149">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="eb3d0-150">Сведения о каждом этапе подготовки.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-150">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="eb3d0-151">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="eb3d0-151">servicePrincipal</span></span>|<span data-ttu-id="eb3d0-152">Коллекция [servicePrincipal](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="eb3d0-152">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="eb3d0-153">Представляет участника службы, используемого для подготовки.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-153">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="eb3d0-154">саурцеидентити</span><span class="sxs-lookup"><span data-stu-id="eb3d0-154">sourceIdentity</span></span>|[<span data-ttu-id="eb3d0-155">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="eb3d0-155">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="eb3d0-156">Сведения о подготовленном исходном объекте.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-156">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="eb3d0-157">саурцесистем</span><span class="sxs-lookup"><span data-stu-id="eb3d0-157">sourceSystem</span></span>|[<span data-ttu-id="eb3d0-158">провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="eb3d0-158">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="eb3d0-159">Сведения об исходной системе подготовленного объекта.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-159">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="eb3d0-160">статусинфо</span><span class="sxs-lookup"><span data-stu-id="eb3d0-160">statusInfo</span></span>|[<span data-ttu-id="eb3d0-161">statusBase</span><span class="sxs-lookup"><span data-stu-id="eb3d0-161">statusBase</span></span>](statusbase.md)|<span data-ttu-id="eb3d0-162">Сведения о состоянии подготовки.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-162">Details of provisioning status.</span></span>|
|<span data-ttu-id="eb3d0-163">таржетидентити</span><span class="sxs-lookup"><span data-stu-id="eb3d0-163">targetIdentity</span></span>|[<span data-ttu-id="eb3d0-164">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="eb3d0-164">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="eb3d0-165">Сведения о подготовленном целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-165">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="eb3d0-166">таржетсистем</span><span class="sxs-lookup"><span data-stu-id="eb3d0-166">targetSystem</span></span>|[<span data-ttu-id="eb3d0-167">провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="eb3d0-167">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="eb3d0-168">Сведения о целевой системе объекта, подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-168">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="eb3d0-169">tenantId</span><span class="sxs-lookup"><span data-stu-id="eb3d0-169">tenantId</span></span>|<span data-ttu-id="eb3d0-170">String</span><span class="sxs-lookup"><span data-stu-id="eb3d0-170">String</span></span>|<span data-ttu-id="eb3d0-171">Уникальный идентификатор клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-171">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb3d0-172">Связи</span><span class="sxs-lookup"><span data-stu-id="eb3d0-172">Relationships</span></span>

<span data-ttu-id="eb3d0-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb3d0-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="eb3d0-174">JSON representation</span></span>

<span data-ttu-id="eb3d0-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb3d0-175">The following is a JSON representation of the resource.</span></span>

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
