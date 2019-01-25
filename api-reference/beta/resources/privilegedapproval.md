---
title: Тип ресурса privilegedApproval
description: Представляет утверждения, запрашиваемых в привилегированной управления удостоверениями для получения в роли.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516891"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="8b55c-103">Тип ресурса privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b55c-104">Представляет утверждения, запрашиваемых в привилегированной управления удостоверениями для получения в роли.</span><span class="sxs-lookup"><span data-stu-id="8b55c-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="8b55c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8b55c-105">Methods</span></span>

| <span data-ttu-id="8b55c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8b55c-106">Method</span></span>           | <span data-ttu-id="8b55c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8b55c-107">Return Type</span></span>    |<span data-ttu-id="8b55c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8b55c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b55c-109">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="8b55c-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="8b55c-111">Чтение свойства и связи объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="8b55c-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="8b55c-112">Список объектов privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="8b55c-113">[privilegedApproval](privilegedapproval.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8b55c-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="8b55c-114">Получите коллекцию privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="8b55c-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="8b55c-115">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="8b55c-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="8b55c-117">Создание объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="8b55c-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="8b55c-118">Обновление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="8b55c-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="8b55c-120">Обновление объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="8b55c-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="8b55c-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="8b55c-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="8b55c-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8b55c-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="8b55c-123">Получите запрашивающего запросов на утверждение.</span><span class="sxs-lookup"><span data-stu-id="8b55c-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b55c-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b55c-124">Properties</span></span>
| <span data-ttu-id="8b55c-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b55c-125">Property</span></span>     | <span data-ttu-id="8b55c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8b55c-126">Type</span></span>   |<span data-ttu-id="8b55c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8b55c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b55c-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="8b55c-128">approvalDuration</span></span>|<span data-ttu-id="8b55c-129">Длительность</span><span class="sxs-lookup"><span data-stu-id="8b55c-129">Duration</span></span>||
|<span data-ttu-id="8b55c-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="8b55c-130">approvalState</span></span>|<span data-ttu-id="8b55c-131">string</span><span class="sxs-lookup"><span data-stu-id="8b55c-131">string</span></span>| <span data-ttu-id="8b55c-132">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="8b55c-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="8b55c-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="8b55c-133">approvalType</span></span>|<span data-ttu-id="8b55c-134">String</span><span class="sxs-lookup"><span data-stu-id="8b55c-134">String</span></span>||
|<span data-ttu-id="8b55c-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="8b55c-135">approverReason</span></span>|<span data-ttu-id="8b55c-136">String</span><span class="sxs-lookup"><span data-stu-id="8b55c-136">String</span></span>||
|<span data-ttu-id="8b55c-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8b55c-137">endDateTime</span></span>|<span data-ttu-id="8b55c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b55c-138">DateTimeOffset</span></span>|<span data-ttu-id="8b55c-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8b55c-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8b55c-141">id</span><span class="sxs-lookup"><span data-stu-id="8b55c-141">id</span></span>|<span data-ttu-id="8b55c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="8b55c-142">String</span></span>| <span data-ttu-id="8b55c-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b55c-143">Read-only.</span></span>|
|<span data-ttu-id="8b55c-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="8b55c-144">requestorReason</span></span>|<span data-ttu-id="8b55c-145">String</span><span class="sxs-lookup"><span data-stu-id="8b55c-145">String</span></span>||
|<span data-ttu-id="8b55c-146">roleId</span><span class="sxs-lookup"><span data-stu-id="8b55c-146">roleId</span></span>|<span data-ttu-id="8b55c-147">String</span><span class="sxs-lookup"><span data-stu-id="8b55c-147">String</span></span>||
|<span data-ttu-id="8b55c-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8b55c-148">startDateTime</span></span>|<span data-ttu-id="8b55c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b55c-149">DateTimeOffset</span></span>|<span data-ttu-id="8b55c-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8b55c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8b55c-152">userId</span><span class="sxs-lookup"><span data-stu-id="8b55c-152">userId</span></span>|<span data-ttu-id="8b55c-153">String</span><span class="sxs-lookup"><span data-stu-id="8b55c-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="8b55c-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="8b55c-154">Relationships</span></span>
| <span data-ttu-id="8b55c-155">Связь</span><span class="sxs-lookup"><span data-stu-id="8b55c-155">Relationship</span></span> | <span data-ttu-id="8b55c-156">Тип</span><span class="sxs-lookup"><span data-stu-id="8b55c-156">Type</span></span>   |<span data-ttu-id="8b55c-157">Описание</span><span class="sxs-lookup"><span data-stu-id="8b55c-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b55c-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="8b55c-158">roleInfo</span></span>|[<span data-ttu-id="8b55c-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="8b55c-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="8b55c-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8b55c-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8b55c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b55c-162">request</span></span>|[<span data-ttu-id="8b55c-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8b55c-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="8b55c-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b55c-164">Read-only.</span></span> <span data-ttu-id="8b55c-165">Запрос назначения ролей для данного объекта утверждения</span><span class="sxs-lookup"><span data-stu-id="8b55c-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b55c-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b55c-166">JSON representation</span></span>
<span data-ttu-id="8b55c-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b55c-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
