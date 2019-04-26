---
title: Тип ресурса Привилежедаппровал
description: Представляет утверждение, запрошенное в результате привилегированного управления удостоверениями для доступа к роли.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563659"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="12815-103">Тип ресурса Привилежедаппровал</span><span class="sxs-lookup"><span data-stu-id="12815-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12815-104">Представляет утверждение, запрошенное в результате привилегированного управления удостоверениями для доступа к роли.</span><span class="sxs-lookup"><span data-stu-id="12815-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="12815-105">Методы</span><span class="sxs-lookup"><span data-stu-id="12815-105">Methods</span></span>

| <span data-ttu-id="12815-106">Метод</span><span class="sxs-lookup"><span data-stu-id="12815-106">Method</span></span>           | <span data-ttu-id="12815-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12815-107">Return Type</span></span>    |<span data-ttu-id="12815-108">Описание</span><span class="sxs-lookup"><span data-stu-id="12815-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12815-109">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="12815-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="12815-111">Чтение свойств и связей объекта Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="12815-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="12815-112">Список объектов Привилежедаппровал</span><span class="sxs-lookup"><span data-stu-id="12815-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="12815-113">Коллекция [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="12815-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="12815-114">Получение коллекции Привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="12815-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="12815-115">Создание privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="12815-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="12815-117">Создание объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="12815-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="12815-118">Обновление privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="12815-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="12815-120">Обновление объекта privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="12815-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="12815-121">Мирекуестс</span><span class="sxs-lookup"><span data-stu-id="12815-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="12815-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="12815-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="12815-123">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="12815-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="12815-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="12815-124">Properties</span></span>
| <span data-ttu-id="12815-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="12815-125">Property</span></span>     | <span data-ttu-id="12815-126">Тип</span><span class="sxs-lookup"><span data-stu-id="12815-126">Type</span></span>   |<span data-ttu-id="12815-127">Описание</span><span class="sxs-lookup"><span data-stu-id="12815-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12815-128">Аппровалдуратион</span><span class="sxs-lookup"><span data-stu-id="12815-128">approvalDuration</span></span>|<span data-ttu-id="12815-129">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="12815-129">Duration</span></span>||
|<span data-ttu-id="12815-130">Аппровалстате</span><span class="sxs-lookup"><span data-stu-id="12815-130">approvalState</span></span>|<span data-ttu-id="12815-131">string</span><span class="sxs-lookup"><span data-stu-id="12815-131">string</span></span>| <span data-ttu-id="12815-132">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="12815-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="12815-133">Аппровалтипе</span><span class="sxs-lookup"><span data-stu-id="12815-133">approvalType</span></span>|<span data-ttu-id="12815-134">String</span><span class="sxs-lookup"><span data-stu-id="12815-134">String</span></span>||
|<span data-ttu-id="12815-135">Аппроверреасон</span><span class="sxs-lookup"><span data-stu-id="12815-135">approverReason</span></span>|<span data-ttu-id="12815-136">String</span><span class="sxs-lookup"><span data-stu-id="12815-136">String</span></span>||
|<span data-ttu-id="12815-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="12815-137">endDateTime</span></span>|<span data-ttu-id="12815-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12815-138">DateTimeOffset</span></span>|<span data-ttu-id="12815-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12815-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="12815-141">id</span><span class="sxs-lookup"><span data-stu-id="12815-141">id</span></span>|<span data-ttu-id="12815-142">String</span><span class="sxs-lookup"><span data-stu-id="12815-142">String</span></span>| <span data-ttu-id="12815-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12815-143">Read-only.</span></span>|
|<span data-ttu-id="12815-144">Рекуесторреасон</span><span class="sxs-lookup"><span data-stu-id="12815-144">requestorReason</span></span>|<span data-ttu-id="12815-145">String</span><span class="sxs-lookup"><span data-stu-id="12815-145">String</span></span>||
|<span data-ttu-id="12815-146">roleId</span><span class="sxs-lookup"><span data-stu-id="12815-146">roleId</span></span>|<span data-ttu-id="12815-147">String</span><span class="sxs-lookup"><span data-stu-id="12815-147">String</span></span>||
|<span data-ttu-id="12815-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="12815-148">startDateTime</span></span>|<span data-ttu-id="12815-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12815-149">DateTimeOffset</span></span>|<span data-ttu-id="12815-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12815-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="12815-152">userId</span><span class="sxs-lookup"><span data-stu-id="12815-152">userId</span></span>|<span data-ttu-id="12815-153">String</span><span class="sxs-lookup"><span data-stu-id="12815-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="12815-154">Связи</span><span class="sxs-lookup"><span data-stu-id="12815-154">Relationships</span></span>
| <span data-ttu-id="12815-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="12815-155">Relationship</span></span> | <span data-ttu-id="12815-156">Тип</span><span class="sxs-lookup"><span data-stu-id="12815-156">Type</span></span>   |<span data-ttu-id="12815-157">Описание</span><span class="sxs-lookup"><span data-stu-id="12815-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12815-158">Ролеинфо</span><span class="sxs-lookup"><span data-stu-id="12815-158">roleInfo</span></span>|[<span data-ttu-id="12815-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="12815-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="12815-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12815-160">Read-only.</span></span> <span data-ttu-id="12815-161">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12815-161">Nullable.</span></span>|
|<span data-ttu-id="12815-162">Request</span><span class="sxs-lookup"><span data-stu-id="12815-162">request</span></span>|[<span data-ttu-id="12815-163">Привилежедролеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="12815-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="12815-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12815-164">Read-only.</span></span> <span data-ttu-id="12815-165">Запрос на назначение роли для этого объекта утверждения</span><span class="sxs-lookup"><span data-stu-id="12815-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12815-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12815-166">JSON representation</span></span>
<span data-ttu-id="12815-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12815-167">Here is a JSON representation of the resource.</span></span>

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
