---
title: тип ресурса userConsentRequest
description: Запрос, созданный пользователем на использование приложения, требующее доступа к организационным данным, несанкционированный для предоставления согласия для себя.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9aab98b448333412b8982fc80e68702e4255f66b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469684"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="69353-103">тип ресурса userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="69353-103">userConsentRequest resource type</span></span>

<span data-ttu-id="69353-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69353-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69353-105">[UserConsentRequest](../resources/userconsentrequest.md) создается пользователем при запросе доступа к приложению, к которому требуется авторизация администратора.</span><span class="sxs-lookup"><span data-stu-id="69353-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by an user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="69353-106">Методы</span><span class="sxs-lookup"><span data-stu-id="69353-106">Methods</span></span>

<span data-ttu-id="69353-107">Метод</span><span class="sxs-lookup"><span data-stu-id="69353-107">Method</span></span>|<span data-ttu-id="69353-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="69353-108">Return type</span></span>|<span data-ttu-id="69353-109">Описание</span><span class="sxs-lookup"><span data-stu-id="69353-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69353-110">Список userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="69353-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="69353-111">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="69353-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="69353-112">Получите список объектов [userConsentRequest](../resources/userconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="69353-112">Get a list of the [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="69353-113">Get userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="69353-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="69353-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="69353-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="69353-115">Ознакомьтесь с свойствами и отношениями [объекта userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="69353-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="69353-116">Список userConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="69353-116">List userConsentRequests: filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="69353-117">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="69353-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="69353-118">Получите список объектов [userConsentRequest](../resources/userconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="69353-118">Get a list of the [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="69353-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="69353-119">Properties</span></span>

|<span data-ttu-id="69353-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="69353-120">Property</span></span>|<span data-ttu-id="69353-121">Тип</span><span class="sxs-lookup"><span data-stu-id="69353-121">Type</span></span>|<span data-ttu-id="69353-122">Описание</span><span class="sxs-lookup"><span data-stu-id="69353-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69353-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="69353-123">approvalId</span></span>|<span data-ttu-id="69353-124">String</span><span class="sxs-lookup"><span data-stu-id="69353-124">String</span></span>|<span data-ttu-id="69353-125">Id утверждения.</span><span class="sxs-lookup"><span data-stu-id="69353-125">The id of the approval.</span></span> <span data-ttu-id="69353-126">Это значение равно значению `id` .</span><span class="sxs-lookup"><span data-stu-id="69353-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="69353-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="69353-127">completedDateTime</span></span>|<span data-ttu-id="69353-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69353-128">DateTimeOffset</span></span>|<span data-ttu-id="69353-129">Дата и время, когда **состояние** запроса было отмечено как `Completed` .</span><span class="sxs-lookup"><span data-stu-id="69353-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="69353-130">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="69353-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="69353-131">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="69353-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="69353-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="69353-132">createdBy</span></span>|[<span data-ttu-id="69353-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="69353-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="69353-134">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="69353-134">The user who created the request.</span></span>|
|<span data-ttu-id="69353-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69353-135">createdDateTime</span></span>|<span data-ttu-id="69353-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69353-136">DateTimeOffset</span></span>|<span data-ttu-id="69353-137">Дата и время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="69353-137">The date and time when the request was created.</span></span> <span data-ttu-id="69353-138">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="69353-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="69353-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="69353-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <br><span data-ttu-id="69353-140">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="69353-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="69353-141">customData</span><span class="sxs-lookup"><span data-stu-id="69353-141">customData</span></span>|<span data-ttu-id="69353-142">String</span><span class="sxs-lookup"><span data-stu-id="69353-142">String</span></span>|<span data-ttu-id="69353-143">Свободное текстовое поле для определения настраиваемой информации для запроса согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="69353-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="69353-144">Не используется.</span><span class="sxs-lookup"><span data-stu-id="69353-144">Not used.</span></span>|
|<span data-ttu-id="69353-145">id</span><span class="sxs-lookup"><span data-stu-id="69353-145">id</span></span>|<span data-ttu-id="69353-146">String</span><span class="sxs-lookup"><span data-stu-id="69353-146">String</span></span>|<span data-ttu-id="69353-147">Идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="69353-147">Identifier of the request.</span></span> |
|<span data-ttu-id="69353-148">reason</span><span class="sxs-lookup"><span data-stu-id="69353-148">reason</span></span>|<span data-ttu-id="69353-149">String</span><span class="sxs-lookup"><span data-stu-id="69353-149">String</span></span>|<span data-ttu-id="69353-150">Обоснование пользователем необходимости доступа к приложению.</span><span class="sxs-lookup"><span data-stu-id="69353-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="69353-151">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="69353-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="69353-152">status</span><span class="sxs-lookup"><span data-stu-id="69353-152">status</span></span>|<span data-ttu-id="69353-153">String</span><span class="sxs-lookup"><span data-stu-id="69353-153">String</span></span>|<span data-ttu-id="69353-154">Состояние запроса на согласие приложения пользователя.</span><span class="sxs-lookup"><span data-stu-id="69353-154">The status of the user's app consent request.</span></span> <span data-ttu-id="69353-155">Возможные значения: `Initializing` , `InProgress` и `Completed` .</span><span class="sxs-lookup"><span data-stu-id="69353-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="69353-156">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="69353-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="69353-157">Связи</span><span class="sxs-lookup"><span data-stu-id="69353-157">Relationships</span></span>

|<span data-ttu-id="69353-158">Связь</span><span class="sxs-lookup"><span data-stu-id="69353-158">Relationship</span></span>|<span data-ttu-id="69353-159">Тип</span><span class="sxs-lookup"><span data-stu-id="69353-159">Type</span></span>|<span data-ttu-id="69353-160">Описание</span><span class="sxs-lookup"><span data-stu-id="69353-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69353-161">утверждение</span><span class="sxs-lookup"><span data-stu-id="69353-161">approval</span></span>|[<span data-ttu-id="69353-162">утверждение</span><span class="sxs-lookup"><span data-stu-id="69353-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="69353-163">Решения об утверждении, связанные с запросом.</span><span class="sxs-lookup"><span data-stu-id="69353-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69353-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69353-164">JSON representation</span></span>

<span data-ttu-id="69353-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69353-165">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "reason": "String"
}
```
