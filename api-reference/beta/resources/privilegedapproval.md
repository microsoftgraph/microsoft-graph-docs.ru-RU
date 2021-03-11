---
title: тип ресурса privilegedApproval
description: Представляет утверждение, запрашиваемого в привилегированном управлении удостоверениями для получения роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7d7842b89bce06d582aa827b853e4170b0693ff8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721609"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="f5909-103">тип ресурса privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-103">privilegedApproval resource type</span></span>

<span data-ttu-id="f5909-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5909-105">Представляет утверждение, запрашиваемого в привилегированном управлении удостоверениями для получения роли.</span><span class="sxs-lookup"><span data-stu-id="f5909-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="f5909-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f5909-106">Methods</span></span>

| <span data-ttu-id="f5909-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f5909-107">Method</span></span>           | <span data-ttu-id="f5909-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f5909-108">Return Type</span></span>    |<span data-ttu-id="f5909-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f5909-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5909-110">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="f5909-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="f5909-112">Чтение свойств и связей объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f5909-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="f5909-113">Список объектов privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="f5909-114">Коллекция [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="f5909-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="f5909-115">Получите коллекцию privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f5909-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="f5909-116">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="f5909-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="f5909-118">Создание объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f5909-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="f5909-119">Обновление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="f5909-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="f5909-121">Обновление объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="f5909-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="f5909-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="f5909-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="f5909-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="f5909-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="f5909-124">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="f5909-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5909-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5909-125">Properties</span></span>
| <span data-ttu-id="f5909-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5909-126">Property</span></span>     | <span data-ttu-id="f5909-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f5909-127">Type</span></span>   |<span data-ttu-id="f5909-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f5909-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5909-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="f5909-129">approvalDuration</span></span>|<span data-ttu-id="f5909-130">Duration</span><span class="sxs-lookup"><span data-stu-id="f5909-130">Duration</span></span>||
|<span data-ttu-id="f5909-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="f5909-131">approvalState</span></span>|<span data-ttu-id="f5909-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f5909-132">string</span></span>| <span data-ttu-id="f5909-133">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="f5909-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="f5909-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="f5909-134">approvalType</span></span>|<span data-ttu-id="f5909-135">String</span><span class="sxs-lookup"><span data-stu-id="f5909-135">String</span></span>||
|<span data-ttu-id="f5909-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="f5909-136">approverReason</span></span>|<span data-ttu-id="f5909-137">String</span><span class="sxs-lookup"><span data-stu-id="f5909-137">String</span></span>||
|<span data-ttu-id="f5909-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f5909-138">endDateTime</span></span>|<span data-ttu-id="f5909-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5909-139">DateTimeOffset</span></span>|<span data-ttu-id="f5909-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f5909-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f5909-141">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f5909-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f5909-142">id</span><span class="sxs-lookup"><span data-stu-id="f5909-142">id</span></span>|<span data-ttu-id="f5909-143">String</span><span class="sxs-lookup"><span data-stu-id="f5909-143">String</span></span>| <span data-ttu-id="f5909-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5909-144">Read-only.</span></span>|
|<span data-ttu-id="f5909-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="f5909-145">requestorReason</span></span>|<span data-ttu-id="f5909-146">String</span><span class="sxs-lookup"><span data-stu-id="f5909-146">String</span></span>||
|<span data-ttu-id="f5909-147">roleId</span><span class="sxs-lookup"><span data-stu-id="f5909-147">roleId</span></span>|<span data-ttu-id="f5909-148">String</span><span class="sxs-lookup"><span data-stu-id="f5909-148">String</span></span>||
|<span data-ttu-id="f5909-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f5909-149">startDateTime</span></span>|<span data-ttu-id="f5909-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5909-150">DateTimeOffset</span></span>|<span data-ttu-id="f5909-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f5909-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f5909-152">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f5909-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f5909-153">userId</span><span class="sxs-lookup"><span data-stu-id="f5909-153">userId</span></span>|<span data-ttu-id="f5909-154">String</span><span class="sxs-lookup"><span data-stu-id="f5909-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="f5909-155">Связи</span><span class="sxs-lookup"><span data-stu-id="f5909-155">Relationships</span></span>
| <span data-ttu-id="f5909-156">Связь</span><span class="sxs-lookup"><span data-stu-id="f5909-156">Relationship</span></span> | <span data-ttu-id="f5909-157">Тип</span><span class="sxs-lookup"><span data-stu-id="f5909-157">Type</span></span>   |<span data-ttu-id="f5909-158">Описание</span><span class="sxs-lookup"><span data-stu-id="f5909-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5909-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="f5909-159">roleInfo</span></span>|[<span data-ttu-id="f5909-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f5909-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="f5909-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5909-161">Read-only.</span></span> <span data-ttu-id="f5909-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f5909-162">Nullable.</span></span>|
|<span data-ttu-id="f5909-163">запрос</span><span class="sxs-lookup"><span data-stu-id="f5909-163">request</span></span>|[<span data-ttu-id="f5909-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f5909-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="f5909-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5909-165">Read-only.</span></span> <span data-ttu-id="f5909-166">Запрос назначения ролей для этого объекта утверждения</span><span class="sxs-lookup"><span data-stu-id="f5909-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5909-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5909-167">JSON representation</span></span>
<span data-ttu-id="f5909-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5909-168">Here is a JSON representation of the resource.</span></span>

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


