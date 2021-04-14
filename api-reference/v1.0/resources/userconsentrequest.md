---
title: тип ресурса userConsentRequest
description: Запрос, созданный пользователем на использование приложения, требующее доступа к организационным данным, несанкционированный для предоставления согласия для себя.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a3ac490e4dcd7231c8b005eeb6a259e525bbf882
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698043"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="08002-103">тип ресурса userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="08002-103">userConsentRequest resource type</span></span>

<span data-ttu-id="08002-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08002-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08002-105">[UserConsentRequest](../resources/userconsentrequest.md) создается пользователем при запросе доступа к приложению, к которому требуется авторизация администратора.</span><span class="sxs-lookup"><span data-stu-id="08002-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by a user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="08002-106">Методы</span><span class="sxs-lookup"><span data-stu-id="08002-106">Methods</span></span>

<span data-ttu-id="08002-107">Метод</span><span class="sxs-lookup"><span data-stu-id="08002-107">Method</span></span>|<span data-ttu-id="08002-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="08002-108">Return type</span></span>|<span data-ttu-id="08002-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08002-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08002-110">Список userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="08002-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="08002-111">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="08002-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="08002-112">Извлечение коллекции [объектов userConsentRequest](userconsentrequest.md) для [приложенияConsentRequest.](appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="08002-112">Retrieve a collection of [userConsentRequest](userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md).</span></span>|
|[<span data-ttu-id="08002-113">Get userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="08002-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="08002-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="08002-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="08002-115">Ознакомьтесь с свойствами и отношениями [объекта userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="08002-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="08002-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="08002-116">filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="08002-117">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="08002-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="08002-118">Ознакомьтесь с свойствами [объектов userConsentRequest](../resources/userconsentrequest.md) для [приложенияConsentRequest,](appconsentrequest.md) для которого текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="08002-118">Read the properties of [userConsentRequest](../resources/userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md) for which the current user is the reviewer.</span></span>|

## <a name="properties"></a><span data-ttu-id="08002-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="08002-119">Properties</span></span>

|<span data-ttu-id="08002-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="08002-120">Property</span></span>|<span data-ttu-id="08002-121">Тип</span><span class="sxs-lookup"><span data-stu-id="08002-121">Type</span></span>|<span data-ttu-id="08002-122">Описание</span><span class="sxs-lookup"><span data-stu-id="08002-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08002-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="08002-123">approvalId</span></span>|<span data-ttu-id="08002-124">String</span><span class="sxs-lookup"><span data-stu-id="08002-124">String</span></span>|<span data-ttu-id="08002-125">Id утверждения.</span><span class="sxs-lookup"><span data-stu-id="08002-125">The id of the approval.</span></span> <span data-ttu-id="08002-126">Это значение равно значению `id` .</span><span class="sxs-lookup"><span data-stu-id="08002-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="08002-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="08002-127">completedDateTime</span></span>|<span data-ttu-id="08002-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08002-128">DateTimeOffset</span></span>|<span data-ttu-id="08002-129">Дата и время, когда **состояние** запроса было отмечено как `Completed` .</span><span class="sxs-lookup"><span data-stu-id="08002-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="08002-130">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="08002-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08002-131">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="08002-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="08002-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="08002-132">createdBy</span></span>|[<span data-ttu-id="08002-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="08002-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="08002-134">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="08002-134">The user who created the request.</span></span>|
|<span data-ttu-id="08002-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08002-135">createdDateTime</span></span>|<span data-ttu-id="08002-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08002-136">DateTimeOffset</span></span>|<span data-ttu-id="08002-137">Дата и время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="08002-137">The date and time when the request was created.</span></span> <span data-ttu-id="08002-138">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="08002-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08002-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="08002-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="08002-140">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="08002-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="08002-141">customData</span><span class="sxs-lookup"><span data-stu-id="08002-141">customData</span></span>|<span data-ttu-id="08002-142">String</span><span class="sxs-lookup"><span data-stu-id="08002-142">String</span></span>|<span data-ttu-id="08002-143">Свободное текстовое поле для определения настраиваемой информации для запроса согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="08002-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="08002-144">Не используется.</span><span class="sxs-lookup"><span data-stu-id="08002-144">Not used.</span></span>|
|<span data-ttu-id="08002-145">id</span><span class="sxs-lookup"><span data-stu-id="08002-145">id</span></span>|<span data-ttu-id="08002-146">String</span><span class="sxs-lookup"><span data-stu-id="08002-146">String</span></span>|<span data-ttu-id="08002-147">Идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="08002-147">Identifier of the request.</span></span> |
|<span data-ttu-id="08002-148">reason</span><span class="sxs-lookup"><span data-stu-id="08002-148">reason</span></span>|<span data-ttu-id="08002-149">String</span><span class="sxs-lookup"><span data-stu-id="08002-149">String</span></span>|<span data-ttu-id="08002-150">Обоснование пользователем необходимости доступа к приложению.</span><span class="sxs-lookup"><span data-stu-id="08002-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="08002-151">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="08002-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="08002-152">status</span><span class="sxs-lookup"><span data-stu-id="08002-152">status</span></span>|<span data-ttu-id="08002-153">String</span><span class="sxs-lookup"><span data-stu-id="08002-153">String</span></span>|<span data-ttu-id="08002-154">Состояние запроса на согласие приложения пользователя.</span><span class="sxs-lookup"><span data-stu-id="08002-154">The status of the user's app consent request.</span></span> <span data-ttu-id="08002-155">Возможные значения: `Initializing` , `InProgress` и `Completed` .</span><span class="sxs-lookup"><span data-stu-id="08002-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="08002-156">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="08002-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="08002-157">Связи</span><span class="sxs-lookup"><span data-stu-id="08002-157">Relationships</span></span>

|<span data-ttu-id="08002-158">Связь</span><span class="sxs-lookup"><span data-stu-id="08002-158">Relationship</span></span>|<span data-ttu-id="08002-159">Тип</span><span class="sxs-lookup"><span data-stu-id="08002-159">Type</span></span>|<span data-ttu-id="08002-160">Описание</span><span class="sxs-lookup"><span data-stu-id="08002-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08002-161">утверждение</span><span class="sxs-lookup"><span data-stu-id="08002-161">approval</span></span>|[<span data-ttu-id="08002-162">утверждение</span><span class="sxs-lookup"><span data-stu-id="08002-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="08002-163">Решения об утверждении, связанные с запросом.</span><span class="sxs-lookup"><span data-stu-id="08002-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08002-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08002-164">JSON representation</span></span>

<span data-ttu-id="08002-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08002-165">The following is a JSON representation of the resource.</span></span>
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
