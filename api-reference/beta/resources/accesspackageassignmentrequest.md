---
title: Тип ресурса Акцесспаккажеассигнментрекуест
description: Запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6be3fa431a2216ef8b31b673a5f73ef6067fff9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939203"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="b2b76-103">Тип ресурса Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="b2b76-103">accessPackageAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2b76-104">В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="b2b76-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="b2b76-105">Если запрос выполнен успешно, при наличии необходимых утверждений пользователь получает назначение пакета Access и является темой этого назначенного пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="b2b76-105">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>


## <a name="methods"></a><span data-ttu-id="b2b76-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b2b76-106">Methods</span></span>

| <span data-ttu-id="b2b76-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b2b76-107">Method</span></span>       | <span data-ttu-id="b2b76-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2b76-108">Return Type</span></span> | <span data-ttu-id="b2b76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b76-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b2b76-110">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="b2b76-110">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="b2b76-111">Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b2b76-111">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="b2b76-112">Получение списка объектов акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="b2b76-112">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="b2b76-113">Создание Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="b2b76-113">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="b2b76-114">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="b2b76-114">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="b2b76-115">Создание нового Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="b2b76-115">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="b2b76-116">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="b2b76-116">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="b2b76-117">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="b2b76-117">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="b2b76-118">Чтение свойств и связей объекта Акцесспаккажеассигнментрекуест.</span><span class="sxs-lookup"><span data-stu-id="b2b76-118">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2b76-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2b76-119">Properties</span></span>

| <span data-ttu-id="b2b76-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2b76-120">Property</span></span>     | <span data-ttu-id="b2b76-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b2b76-121">Type</span></span>        | <span data-ttu-id="b2b76-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b76-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2b76-123">комплетеддате</span><span class="sxs-lookup"><span data-stu-id="b2b76-123">completedDate</span></span>|<span data-ttu-id="b2b76-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2b76-124">DateTimeOffset</span></span>|<span data-ttu-id="b2b76-125">Дата завершения обработки (успешное или неудачное) запроса.</span><span class="sxs-lookup"><span data-stu-id="b2b76-125">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="b2b76-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b2b76-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b2b76-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b2b76-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b2b76-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-128">Read-only.</span></span>|
|<span data-ttu-id="b2b76-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2b76-129">createdDateTime</span></span>|<span data-ttu-id="b2b76-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2b76-130">DateTimeOffset</span></span>|<span data-ttu-id="b2b76-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b2b76-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b2b76-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b2b76-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b2b76-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-133">Read-only.</span></span>|
|<span data-ttu-id="b2b76-134">id</span><span class="sxs-lookup"><span data-stu-id="b2b76-134">id</span></span>|<span data-ttu-id="b2b76-135">String</span><span class="sxs-lookup"><span data-stu-id="b2b76-135">String</span></span>| <span data-ttu-id="b2b76-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-136">Read-only.</span></span>|
|<span data-ttu-id="b2b76-137">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="b2b76-137">isValidationOnly</span></span>|<span data-ttu-id="b2b76-138">Логический</span><span class="sxs-lookup"><span data-stu-id="b2b76-138">Boolean</span></span>|<span data-ttu-id="b2b76-139">Имеет значение true, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-139">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="b2b76-140">текста</span><span class="sxs-lookup"><span data-stu-id="b2b76-140">justification</span></span>|<span data-ttu-id="b2b76-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b76-141">String</span></span>|<span data-ttu-id="b2b76-142">Выставляемое по запросу обоснование.</span><span class="sxs-lookup"><span data-stu-id="b2b76-142">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="b2b76-143">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="b2b76-143">requestState</span></span>|<span data-ttu-id="b2b76-144">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b76-144">String</span></span>|<span data-ttu-id="b2b76-145">Один из `Denied`, `Delivered`, `PartiallyDelivered`.</span><span class="sxs-lookup"><span data-stu-id="b2b76-145">One of `Denied`, `Delivered`, `PartiallyDelivered`.</span></span> <span data-ttu-id="b2b76-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-146">Read-only.</span></span>|
|<span data-ttu-id="b2b76-147">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="b2b76-147">requestStatus</span></span>|<span data-ttu-id="b2b76-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b76-148">String</span></span>|<span data-ttu-id="b2b76-149">Дополнительные сведения о состоянии обработки запроса.</span><span class="sxs-lookup"><span data-stu-id="b2b76-149">More information on the request processing status.</span></span> <span data-ttu-id="b2b76-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-150">Read-only.</span></span>|
|<span data-ttu-id="b2b76-151">requestType</span><span class="sxs-lookup"><span data-stu-id="b2b76-151">requestType</span></span>|<span data-ttu-id="b2b76-152">Строка</span><span class="sxs-lookup"><span data-stu-id="b2b76-152">String</span></span>|<span data-ttu-id="b2b76-153">Один из `UserAdd` или `UserRemove`.</span><span class="sxs-lookup"><span data-stu-id="b2b76-153">One of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="b2b76-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-154">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b2b76-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2b76-155">Relationships</span></span>

| <span data-ttu-id="b2b76-156">Связь</span><span class="sxs-lookup"><span data-stu-id="b2b76-156">Relationship</span></span> | <span data-ttu-id="b2b76-157">Тип</span><span class="sxs-lookup"><span data-stu-id="b2b76-157">Type</span></span>        | <span data-ttu-id="b2b76-158">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b76-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2b76-159">опросчика</span><span class="sxs-lookup"><span data-stu-id="b2b76-159">requestor</span></span>|[<span data-ttu-id="b2b76-160">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="b2b76-160">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="b2b76-161">Тема, которая запросила или, если назначено прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="b2b76-161">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="b2b76-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2b76-162">Read-only.</span></span> <span data-ttu-id="b2b76-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b2b76-163">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b2b76-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2b76-164">JSON representation</span></span>

<span data-ttu-id="b2b76-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2b76-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
 
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
