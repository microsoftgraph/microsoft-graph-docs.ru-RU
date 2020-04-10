---
title: Тип ресурса Привилежедаппровал
description: Представляет утверждение, запрошенное в результате привилегированного управления удостоверениями для доступа к роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c4148e5740c9b31368be336a615524ced426a560
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219230"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="7afff-103">Тип ресурса Привилежедаппровал</span><span class="sxs-lookup"><span data-stu-id="7afff-103">privilegedApproval resource type</span></span>

<span data-ttu-id="7afff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7afff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7afff-105">Представляет утверждение, запрошенное в результате привилегированного управления удостоверениями для доступа к роли.</span><span class="sxs-lookup"><span data-stu-id="7afff-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="7afff-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7afff-106">Methods</span></span>

| <span data-ttu-id="7afff-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7afff-107">Method</span></span>           | <span data-ttu-id="7afff-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7afff-108">Return Type</span></span>    |<span data-ttu-id="7afff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7afff-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7afff-110">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="7afff-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="7afff-112">Чтение свойств и связей объекта Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="7afff-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="7afff-113">Список объектов Привилежедаппровал</span><span class="sxs-lookup"><span data-stu-id="7afff-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="7afff-114">Коллекция [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="7afff-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="7afff-115">Получение коллекции Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="7afff-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="7afff-116">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="7afff-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="7afff-118">Создание объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="7afff-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="7afff-119">Обновление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="7afff-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="7afff-121">Обновление объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="7afff-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="7afff-122">мирекуестс</span><span class="sxs-lookup"><span data-stu-id="7afff-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="7afff-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7afff-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="7afff-124">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="7afff-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="7afff-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="7afff-125">Properties</span></span>
| <span data-ttu-id="7afff-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7afff-126">Property</span></span>     | <span data-ttu-id="7afff-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7afff-127">Type</span></span>   |<span data-ttu-id="7afff-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7afff-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7afff-129">аппровалдуратион</span><span class="sxs-lookup"><span data-stu-id="7afff-129">approvalDuration</span></span>|<span data-ttu-id="7afff-130">Длительность</span><span class="sxs-lookup"><span data-stu-id="7afff-130">Duration</span></span>||
|<span data-ttu-id="7afff-131">аппровалстате</span><span class="sxs-lookup"><span data-stu-id="7afff-131">approvalState</span></span>|<span data-ttu-id="7afff-132">string</span><span class="sxs-lookup"><span data-stu-id="7afff-132">string</span></span>| <span data-ttu-id="7afff-133">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="7afff-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="7afff-134">аппровалтипе</span><span class="sxs-lookup"><span data-stu-id="7afff-134">approvalType</span></span>|<span data-ttu-id="7afff-135">Строка</span><span class="sxs-lookup"><span data-stu-id="7afff-135">String</span></span>||
|<span data-ttu-id="7afff-136">аппроверреасон</span><span class="sxs-lookup"><span data-stu-id="7afff-136">approverReason</span></span>|<span data-ttu-id="7afff-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7afff-137">String</span></span>||
|<span data-ttu-id="7afff-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7afff-138">endDateTime</span></span>|<span data-ttu-id="7afff-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7afff-139">DateTimeOffset</span></span>|<span data-ttu-id="7afff-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7afff-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7afff-142">id</span><span class="sxs-lookup"><span data-stu-id="7afff-142">id</span></span>|<span data-ttu-id="7afff-143">Строка</span><span class="sxs-lookup"><span data-stu-id="7afff-143">String</span></span>| <span data-ttu-id="7afff-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7afff-144">Read-only.</span></span>|
|<span data-ttu-id="7afff-145">рекуесторреасон</span><span class="sxs-lookup"><span data-stu-id="7afff-145">requestorReason</span></span>|<span data-ttu-id="7afff-146">Строка</span><span class="sxs-lookup"><span data-stu-id="7afff-146">String</span></span>||
|<span data-ttu-id="7afff-147">roleId</span><span class="sxs-lookup"><span data-stu-id="7afff-147">roleId</span></span>|<span data-ttu-id="7afff-148">Строка</span><span class="sxs-lookup"><span data-stu-id="7afff-148">String</span></span>||
|<span data-ttu-id="7afff-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7afff-149">startDateTime</span></span>|<span data-ttu-id="7afff-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7afff-150">DateTimeOffset</span></span>|<span data-ttu-id="7afff-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7afff-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7afff-153">userId</span><span class="sxs-lookup"><span data-stu-id="7afff-153">userId</span></span>|<span data-ttu-id="7afff-154">String</span><span class="sxs-lookup"><span data-stu-id="7afff-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="7afff-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="7afff-155">Relationships</span></span>
| <span data-ttu-id="7afff-156">Связь</span><span class="sxs-lookup"><span data-stu-id="7afff-156">Relationship</span></span> | <span data-ttu-id="7afff-157">Тип</span><span class="sxs-lookup"><span data-stu-id="7afff-157">Type</span></span>   |<span data-ttu-id="7afff-158">Описание</span><span class="sxs-lookup"><span data-stu-id="7afff-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7afff-159">ролеинфо</span><span class="sxs-lookup"><span data-stu-id="7afff-159">roleInfo</span></span>|[<span data-ttu-id="7afff-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="7afff-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="7afff-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7afff-161">Read-only.</span></span> <span data-ttu-id="7afff-162">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7afff-162">Nullable.</span></span>|
|<span data-ttu-id="7afff-163">Request</span><span class="sxs-lookup"><span data-stu-id="7afff-163">request</span></span>|[<span data-ttu-id="7afff-164">привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="7afff-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="7afff-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7afff-165">Read-only.</span></span> <span data-ttu-id="7afff-166">Запрос на назначение роли для этого объекта утверждения</span><span class="sxs-lookup"><span data-stu-id="7afff-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7afff-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7afff-167">JSON representation</span></span>
<span data-ttu-id="7afff-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7afff-168">Here is a JSON representation of the resource.</span></span>

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
