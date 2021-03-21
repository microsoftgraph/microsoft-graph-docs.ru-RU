---
title: тип ресурса privilegedApproval
description: Представляет утверждение, запрашиваемого в привилегированном управлении удостоверениями для получения роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8d092d6c877f9fa2bdce2d645ef56a84508c510d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962590"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="4e260-103">тип ресурса privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-103">privilegedApproval resource type</span></span>

<span data-ttu-id="4e260-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e260-105">Представляет утверждение, запрашиваемого в привилегированном управлении удостоверениями для получения роли.</span><span class="sxs-lookup"><span data-stu-id="4e260-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="4e260-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4e260-106">Methods</span></span>

| <span data-ttu-id="4e260-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4e260-107">Method</span></span>           | <span data-ttu-id="4e260-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e260-108">Return Type</span></span>    |<span data-ttu-id="4e260-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e260-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e260-110">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="4e260-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="4e260-112">Чтение свойств и связей объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="4e260-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="4e260-113">Список объектов privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="4e260-114">Коллекция [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="4e260-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="4e260-115">Получите коллекцию privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="4e260-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="4e260-116">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="4e260-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="4e260-118">Создание объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="4e260-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="4e260-119">Обновление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="4e260-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="4e260-121">Обновление объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="4e260-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="4e260-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="4e260-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="4e260-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4e260-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="4e260-124">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="4e260-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e260-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e260-125">Properties</span></span>
| <span data-ttu-id="4e260-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e260-126">Property</span></span>     | <span data-ttu-id="4e260-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4e260-127">Type</span></span>   |<span data-ttu-id="4e260-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4e260-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e260-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="4e260-129">approvalDuration</span></span>|<span data-ttu-id="4e260-130">Duration</span><span class="sxs-lookup"><span data-stu-id="4e260-130">Duration</span></span>||
|<span data-ttu-id="4e260-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="4e260-131">approvalState</span></span>|<span data-ttu-id="4e260-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="4e260-132">approvalState</span></span>| <span data-ttu-id="4e260-133">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="4e260-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="4e260-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="4e260-134">approvalType</span></span>|<span data-ttu-id="4e260-135">Строка</span><span class="sxs-lookup"><span data-stu-id="4e260-135">String</span></span>||
|<span data-ttu-id="4e260-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="4e260-136">approverReason</span></span>|<span data-ttu-id="4e260-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4e260-137">String</span></span>||
|<span data-ttu-id="4e260-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4e260-138">endDateTime</span></span>|<span data-ttu-id="4e260-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e260-139">DateTimeOffset</span></span>|<span data-ttu-id="4e260-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4e260-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4e260-141">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4e260-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4e260-142">id</span><span class="sxs-lookup"><span data-stu-id="4e260-142">id</span></span>|<span data-ttu-id="4e260-143">String</span><span class="sxs-lookup"><span data-stu-id="4e260-143">String</span></span>| <span data-ttu-id="4e260-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e260-144">Read-only.</span></span>|
|<span data-ttu-id="4e260-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="4e260-145">requestorReason</span></span>|<span data-ttu-id="4e260-146">Строка</span><span class="sxs-lookup"><span data-stu-id="4e260-146">String</span></span>||
|<span data-ttu-id="4e260-147">roleId</span><span class="sxs-lookup"><span data-stu-id="4e260-147">roleId</span></span>|<span data-ttu-id="4e260-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4e260-148">String</span></span>||
|<span data-ttu-id="4e260-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e260-149">startDateTime</span></span>|<span data-ttu-id="4e260-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e260-150">DateTimeOffset</span></span>|<span data-ttu-id="4e260-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4e260-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4e260-152">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4e260-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4e260-153">userId</span><span class="sxs-lookup"><span data-stu-id="4e260-153">userId</span></span>|<span data-ttu-id="4e260-154">String</span><span class="sxs-lookup"><span data-stu-id="4e260-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="4e260-155">Связи</span><span class="sxs-lookup"><span data-stu-id="4e260-155">Relationships</span></span>
| <span data-ttu-id="4e260-156">Связь</span><span class="sxs-lookup"><span data-stu-id="4e260-156">Relationship</span></span> | <span data-ttu-id="4e260-157">Тип</span><span class="sxs-lookup"><span data-stu-id="4e260-157">Type</span></span>   |<span data-ttu-id="4e260-158">Описание</span><span class="sxs-lookup"><span data-stu-id="4e260-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e260-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="4e260-159">roleInfo</span></span>|[<span data-ttu-id="4e260-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="4e260-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="4e260-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e260-161">Read-only.</span></span> <span data-ttu-id="4e260-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4e260-162">Nullable.</span></span>|
|<span data-ttu-id="4e260-163">запрос</span><span class="sxs-lookup"><span data-stu-id="4e260-163">request</span></span>|[<span data-ttu-id="4e260-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4e260-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="4e260-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e260-165">Read-only.</span></span> <span data-ttu-id="4e260-166">Запрос назначения ролей для этого объекта утверждения</span><span class="sxs-lookup"><span data-stu-id="4e260-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e260-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e260-167">JSON representation</span></span>
<span data-ttu-id="4e260-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e260-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->


