---
title: Тип ресурса Провисионингобжектсуммари
description: Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26c217720692b0d36cfa0acf7537b757c92399ac
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349438"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="20b81-103">Тип ресурса Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="20b81-103">provisioningObjectSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20b81-104">Представляет действие, выполненное службой подготовки Azure AD и связанными с ним свойствами.</span><span class="sxs-lookup"><span data-stu-id="20b81-104">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="20b81-105">Методы</span><span class="sxs-lookup"><span data-stu-id="20b81-105">Methods</span></span>

| <span data-ttu-id="20b81-106">Метод</span><span class="sxs-lookup"><span data-stu-id="20b81-106">Method</span></span>       | <span data-ttu-id="20b81-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20b81-107">Return Type</span></span> | <span data-ttu-id="20b81-108">Описание</span><span class="sxs-lookup"><span data-stu-id="20b81-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="20b81-109">Список Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="20b81-109">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="20b81-110">Провисионингобжектсуммари</span><span class="sxs-lookup"><span data-stu-id="20b81-110">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="20b81-111">Получение списка всех событий подготовки, произошедших в клиенте.</span><span class="sxs-lookup"><span data-stu-id="20b81-111">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="20b81-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="20b81-112">Properties</span></span>

| <span data-ttu-id="20b81-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="20b81-113">Property</span></span>     | <span data-ttu-id="20b81-114">Тип</span><span class="sxs-lookup"><span data-stu-id="20b81-114">Type</span></span>        | <span data-ttu-id="20b81-115">Описание</span><span class="sxs-lookup"><span data-stu-id="20b81-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20b81-116">action</span><span class="sxs-lookup"><span data-stu-id="20b81-116">action</span></span>|<span data-ttu-id="20b81-117">String</span><span class="sxs-lookup"><span data-stu-id="20b81-117">String</span></span>|<span data-ttu-id="20b81-118">Указывает имя действия или имя операции (например, создание пользователя, Добавление участника в группу).</span><span class="sxs-lookup"><span data-stu-id="20b81-118">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="20b81-119">Список действий, регистрируемых в журнале, можно найти в списке действий Azure AD.</span><span class="sxs-lookup"><span data-stu-id="20b81-119">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="20b81-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="20b81-120">activityDateTime</span></span>|<span data-ttu-id="20b81-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b81-121">DateTimeOffset</span></span>|<span data-ttu-id="20b81-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="20b81-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="20b81-124">Чанжеид</span><span class="sxs-lookup"><span data-stu-id="20b81-124">changeId</span></span>|<span data-ttu-id="20b81-125">String</span><span class="sxs-lookup"><span data-stu-id="20b81-125">String</span></span>|<span data-ttu-id="20b81-126">Уникальный идентификатор этого изменения в этом цикле.</span><span class="sxs-lookup"><span data-stu-id="20b81-126">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="20b81-127">Циклеид</span><span class="sxs-lookup"><span data-stu-id="20b81-127">cycleId</span></span>|<span data-ttu-id="20b81-128">String</span><span class="sxs-lookup"><span data-stu-id="20b81-128">String</span></span>|<span data-ttu-id="20b81-129">Уникальный идентификатор для итерации задания.</span><span class="sxs-lookup"><span data-stu-id="20b81-129">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="20b81-130">Дуратионинмиллисекондс</span><span class="sxs-lookup"><span data-stu-id="20b81-130">durationInMilliseconds</span></span>|<span data-ttu-id="20b81-131">Int32</span><span class="sxs-lookup"><span data-stu-id="20b81-131">Int32</span></span>|<span data-ttu-id="20b81-132">Указывает время завершения этого действия подготовки.</span><span class="sxs-lookup"><span data-stu-id="20b81-132">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="20b81-133">Измеряется в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="20b81-133">Measured in milliseconds.</span></span>|
|<span data-ttu-id="20b81-134">id</span><span class="sxs-lookup"><span data-stu-id="20b81-134">id</span></span>|<span data-ttu-id="20b81-135">String</span><span class="sxs-lookup"><span data-stu-id="20b81-135">String</span></span>| <span data-ttu-id="20b81-136">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="20b81-136">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="20b81-137">Это GUID, предназначенный только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20b81-137">This is a read-only GUID.</span></span>|
|<span data-ttu-id="20b81-138">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="20b81-138">initiatedBy</span></span>|[<span data-ttu-id="20b81-139">стороны</span><span class="sxs-lookup"><span data-stu-id="20b81-139">initiator</span></span>](initiator.md)|<span data-ttu-id="20b81-140">Сведения о том, кто инициировал эту подготовку.</span><span class="sxs-lookup"><span data-stu-id="20b81-140">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="20b81-141">jobId</span><span class="sxs-lookup"><span data-stu-id="20b81-141">jobId</span></span>|<span data-ttu-id="20b81-142">String</span><span class="sxs-lookup"><span data-stu-id="20b81-142">String</span></span>|<span data-ttu-id="20b81-143">Уникальный идентификатор для полного задания подготовки.</span><span class="sxs-lookup"><span data-stu-id="20b81-143">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="20b81-144">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="20b81-144">modifiedProperties</span></span>|<span data-ttu-id="20b81-145">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="20b81-145">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="20b81-146">Сведения о каждом свойстве, которое было изменено в этом действии подготовки для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="20b81-146">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="20b81-147">Провисионингстепс</span><span class="sxs-lookup"><span data-stu-id="20b81-147">provisioningSteps</span></span>|<span data-ttu-id="20b81-148">Коллекция [провисионингстеп](provisioningstep.md)</span><span class="sxs-lookup"><span data-stu-id="20b81-148">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="20b81-149">Сведения о каждом этапе подготовки.</span><span class="sxs-lookup"><span data-stu-id="20b81-149">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="20b81-150">Саурцеидентити</span><span class="sxs-lookup"><span data-stu-id="20b81-150">sourceIdentity</span></span>|[<span data-ttu-id="20b81-151">Провисионедидентити</span><span class="sxs-lookup"><span data-stu-id="20b81-151">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="20b81-152">Сведения о подготовленном исходном объекте.</span><span class="sxs-lookup"><span data-stu-id="20b81-152">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="20b81-153">Саурцесистем</span><span class="sxs-lookup"><span data-stu-id="20b81-153">sourceSystem</span></span>|[<span data-ttu-id="20b81-154">Провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="20b81-154">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="20b81-155">Сведения об исходной системе подготовленного объекта.</span><span class="sxs-lookup"><span data-stu-id="20b81-155">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="20b81-156">Статусинфо</span><span class="sxs-lookup"><span data-stu-id="20b81-156">statusInfo</span></span>|[<span data-ttu-id="20b81-157">Статусбасе</span><span class="sxs-lookup"><span data-stu-id="20b81-157">statusBase</span></span>](statusbase.md)|<span data-ttu-id="20b81-158">Сведения о состоянии подготовки.</span><span class="sxs-lookup"><span data-stu-id="20b81-158">Details of provisioning status.</span></span>|
|<span data-ttu-id="20b81-159">Таржетидентити</span><span class="sxs-lookup"><span data-stu-id="20b81-159">targetIdentity</span></span>|[<span data-ttu-id="20b81-160">Провисионедидентити</span><span class="sxs-lookup"><span data-stu-id="20b81-160">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="20b81-161">Сведения о подготовленном целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="20b81-161">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="20b81-162">Таржетсистем</span><span class="sxs-lookup"><span data-stu-id="20b81-162">targetSystem</span></span>|[<span data-ttu-id="20b81-163">Провисионингсистемдетаилс</span><span class="sxs-lookup"><span data-stu-id="20b81-163">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="20b81-164">Сведения о целевой системе объекта, подготавливается к работе.</span><span class="sxs-lookup"><span data-stu-id="20b81-164">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="20b81-165">tenantId</span><span class="sxs-lookup"><span data-stu-id="20b81-165">tenantId</span></span>|<span data-ttu-id="20b81-166">String</span><span class="sxs-lookup"><span data-stu-id="20b81-166">String</span></span>|<span data-ttu-id="20b81-167">Уникальный идентификатор клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="20b81-167">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20b81-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="20b81-168">Relationships</span></span>

<span data-ttu-id="20b81-169">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="20b81-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20b81-170">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="20b81-170">JSON representation</span></span>

<span data-ttu-id="20b81-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20b81-171">The following is a JSON representation of the resource.</span></span>

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
