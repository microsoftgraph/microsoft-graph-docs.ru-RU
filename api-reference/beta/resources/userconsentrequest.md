---
title: тип ресурса userConsentRequest
description: Запрос, созданный пользователем на использование приложения, требующее доступа к организационным данным, несанкционированный для предоставления согласия для себя.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ea9520e34237a0e4b60e5e077a487182b18369e6
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698072"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="5ed18-103">тип ресурса userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="5ed18-103">userConsentRequest resource type</span></span>

<span data-ttu-id="5ed18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ed18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ed18-105">[UserConsentRequest](../resources/userconsentrequest.md) создается пользователем при запросе доступа к приложению, к которому требуется авторизация администратора.</span><span class="sxs-lookup"><span data-stu-id="5ed18-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by a user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="5ed18-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5ed18-106">Methods</span></span>
|<span data-ttu-id="5ed18-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5ed18-107">Method</span></span>|<span data-ttu-id="5ed18-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5ed18-108">Return type</span></span>|<span data-ttu-id="5ed18-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed18-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ed18-110">Список userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="5ed18-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="5ed18-111">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5ed18-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="5ed18-112">Извлечение коллекции [объектов userConsentRequest](userconsentrequest.md) для [приложенияConsentRequest.](appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5ed18-112">Retrieve a collection of [userConsentRequest](userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md).</span></span>|
|[<span data-ttu-id="5ed18-113">Get userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="5ed18-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="5ed18-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="5ed18-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="5ed18-115">Ознакомьтесь с свойствами и отношениями [объекта userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5ed18-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="5ed18-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="5ed18-116">filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="5ed18-117">[коллекция userConsentRequest](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5ed18-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="5ed18-118">Ознакомьтесь с свойствами [объектов userConsentRequest](../resources/userconsentrequest.md) для [приложенияConsentRequest,](appconsentrequest.md) для которого текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="5ed18-118">Read the properties of [userConsentRequest](../resources/userconsentrequest.md) objects for an [appConsentRequest](appconsentrequest.md) for which the current user is the reviewer.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ed18-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ed18-119">Properties</span></span>
|<span data-ttu-id="5ed18-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ed18-120">Property</span></span>|<span data-ttu-id="5ed18-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5ed18-121">Type</span></span>|<span data-ttu-id="5ed18-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed18-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed18-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="5ed18-123">approvalId</span></span>|<span data-ttu-id="5ed18-124">String</span><span class="sxs-lookup"><span data-stu-id="5ed18-124">String</span></span>|<span data-ttu-id="5ed18-125">Id утверждения.</span><span class="sxs-lookup"><span data-stu-id="5ed18-125">The id of the approval.</span></span> <span data-ttu-id="5ed18-126">Это значение равно значению `id` .</span><span class="sxs-lookup"><span data-stu-id="5ed18-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="5ed18-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed18-127">completedDateTime</span></span>|<span data-ttu-id="5ed18-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed18-128">DateTimeOffset</span></span>|<span data-ttu-id="5ed18-129">Дата и время, когда **состояние** запроса было отмечено как `Completed` .</span><span class="sxs-lookup"><span data-stu-id="5ed18-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="5ed18-130">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5ed18-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5ed18-131">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5ed18-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5ed18-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="5ed18-132">createdBy</span></span>|[<span data-ttu-id="5ed18-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="5ed18-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="5ed18-134">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="5ed18-134">The user who created the request.</span></span>|
|<span data-ttu-id="5ed18-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ed18-135">createdDateTime</span></span>|<span data-ttu-id="5ed18-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ed18-136">DateTimeOffset</span></span>|<span data-ttu-id="5ed18-137">Дата и время создания запроса.</span><span class="sxs-lookup"><span data-stu-id="5ed18-137">The date and time when the request was created.</span></span> <span data-ttu-id="5ed18-138">Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5ed18-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5ed18-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5ed18-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5ed18-140">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="5ed18-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="5ed18-141">customData</span><span class="sxs-lookup"><span data-stu-id="5ed18-141">customData</span></span>|<span data-ttu-id="5ed18-142">String</span><span class="sxs-lookup"><span data-stu-id="5ed18-142">String</span></span>|<span data-ttu-id="5ed18-143">Свободное текстовое поле для определения настраиваемой информации для запроса согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5ed18-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="5ed18-144">Не используется.</span><span class="sxs-lookup"><span data-stu-id="5ed18-144">Not used.</span></span>|
|<span data-ttu-id="5ed18-145">id</span><span class="sxs-lookup"><span data-stu-id="5ed18-145">id</span></span>|<span data-ttu-id="5ed18-146">String</span><span class="sxs-lookup"><span data-stu-id="5ed18-146">String</span></span>|<span data-ttu-id="5ed18-147">Идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="5ed18-147">Identifier of the request.</span></span> |
|<span data-ttu-id="5ed18-148">reason</span><span class="sxs-lookup"><span data-stu-id="5ed18-148">reason</span></span>|<span data-ttu-id="5ed18-149">String</span><span class="sxs-lookup"><span data-stu-id="5ed18-149">String</span></span>|<span data-ttu-id="5ed18-150">Обоснование пользователем необходимости доступа к приложению.</span><span class="sxs-lookup"><span data-stu-id="5ed18-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="5ed18-151">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="5ed18-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="5ed18-152">status</span><span class="sxs-lookup"><span data-stu-id="5ed18-152">status</span></span>|<span data-ttu-id="5ed18-153">String</span><span class="sxs-lookup"><span data-stu-id="5ed18-153">String</span></span>|<span data-ttu-id="5ed18-154">Состояние запроса на согласие приложения пользователя.</span><span class="sxs-lookup"><span data-stu-id="5ed18-154">The status of the user's app consent request.</span></span> <span data-ttu-id="5ed18-155">Возможные значения: `Initializing` , `InProgress` и `Completed` .</span><span class="sxs-lookup"><span data-stu-id="5ed18-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="5ed18-156">Поддерживает `$filter` `eq` (только) и `$orderby` .</span><span class="sxs-lookup"><span data-stu-id="5ed18-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5ed18-157">Связи</span><span class="sxs-lookup"><span data-stu-id="5ed18-157">Relationships</span></span>
|<span data-ttu-id="5ed18-158">Связь</span><span class="sxs-lookup"><span data-stu-id="5ed18-158">Relationship</span></span>|<span data-ttu-id="5ed18-159">Тип</span><span class="sxs-lookup"><span data-stu-id="5ed18-159">Type</span></span>|<span data-ttu-id="5ed18-160">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed18-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed18-161">утверждение</span><span class="sxs-lookup"><span data-stu-id="5ed18-161">approval</span></span>|[<span data-ttu-id="5ed18-162">утверждение</span><span class="sxs-lookup"><span data-stu-id="5ed18-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="5ed18-163">Решения об утверждении, связанные с запросом.</span><span class="sxs-lookup"><span data-stu-id="5ed18-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ed18-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ed18-164">JSON representation</span></span>
<span data-ttu-id="5ed18-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ed18-165">The following is a JSON representation of the resource.</span></span>
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

