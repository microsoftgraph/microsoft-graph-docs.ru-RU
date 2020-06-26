---
title: Группа списка memberOf
description: Получение групп и административных единиц, непосредственным участником которых является группа.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9711354a6c85933f9e7bbc440964d66990fbe898
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895841"
---
# <a name="list-group-memberof"></a><span data-ttu-id="782f6-103">Группа списка memberOf</span><span class="sxs-lookup"><span data-stu-id="782f6-103">List group memberOf</span></span>

<span data-ttu-id="782f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="782f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="782f6-105">Получение групп и административных единиц, непосредственным участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="782f6-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="782f6-106">This operation is not transitive.</span><span class="sxs-lookup"><span data-stu-id="782f6-106">This operation is not transitive.</span></span> <span data-ttu-id="782f6-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span><span class="sxs-lookup"><span data-stu-id="782f6-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="782f6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="782f6-108">Permissions</span></span>

<span data-ttu-id="782f6-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="782f6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="782f6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="782f6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="782f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="782f6-111">Permission type</span></span> | <span data-ttu-id="782f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="782f6-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="782f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="782f6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="782f6-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="782f6-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="782f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="782f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="782f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="782f6-116">Not supported.</span></span> |
| <span data-ttu-id="782f6-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="782f6-117">Application</span></span> | <span data-ttu-id="782f6-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="782f6-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="782f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="782f6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="782f6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="782f6-120">Optional query parameters</span></span>

<span data-ttu-id="782f6-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="782f6-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="782f6-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только те группы, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="782f6-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="782f6-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="782f6-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="782f6-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="782f6-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="782f6-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="782f6-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="782f6-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="782f6-126">Request headers</span></span>

| <span data-ttu-id="782f6-127">Имя</span><span class="sxs-lookup"><span data-stu-id="782f6-127">Name</span></span> | <span data-ttu-id="782f6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="782f6-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="782f6-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="782f6-129">Authorization</span></span>  | <span data-ttu-id="782f6-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="782f6-130">Bearer {token}.</span></span> <span data-ttu-id="782f6-131">Required.</span><span class="sxs-lookup"><span data-stu-id="782f6-131">Required.</span></span> |
| <span data-ttu-id="782f6-132">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="782f6-132">ConsistencyLevel</span></span> | <span data-ttu-id="782f6-133">закончить.</span><span class="sxs-lookup"><span data-stu-id="782f6-133">eventual.</span></span> <span data-ttu-id="782f6-134">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="782f6-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="782f6-135">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="782f6-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="782f6-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="782f6-136">Request body</span></span>

<span data-ttu-id="782f6-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="782f6-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="782f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="782f6-138">Response</span></span>

<span data-ttu-id="782f6-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="782f6-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="782f6-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="782f6-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="782f6-141">Пример 1: получение групп и административных единиц, непосредственным участником которых является группа</span><span class="sxs-lookup"><span data-stu-id="782f6-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="782f6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="782f6-142">Request</span></span>

<span data-ttu-id="782f6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="782f6-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="782f6-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="782f6-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="782f6-145">C#</span><span class="sxs-lookup"><span data-stu-id="782f6-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="782f6-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="782f6-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="782f6-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="782f6-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="782f6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="782f6-148">Response</span></span>

<span data-ttu-id="782f6-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="782f6-149">The following is an example of the response.</span></span>
><span data-ttu-id="782f6-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="782f6-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="782f6-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="782f6-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="782f6-152">Пример 2: получение только количества всех членств</span><span class="sxs-lookup"><span data-stu-id="782f6-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="782f6-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="782f6-153">Request</span></span>

<span data-ttu-id="782f6-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="782f6-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="782f6-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="782f6-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="782f6-156">C#</span><span class="sxs-lookup"><span data-stu-id="782f6-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="782f6-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="782f6-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="782f6-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="782f6-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="782f6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="782f6-159">Response</span></span>

<span data-ttu-id="782f6-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="782f6-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="782f6-161">394</span><span class="sxs-lookup"><span data-stu-id="782f6-161">394</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="782f6-162">Пример 3: Использование приведения OData для получения только количества участников группы</span><span class="sxs-lookup"><span data-stu-id="782f6-162">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="782f6-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="782f6-163">Request</span></span>

<span data-ttu-id="782f6-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="782f6-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="782f6-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="782f6-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="782f6-166">C#</span><span class="sxs-lookup"><span data-stu-id="782f6-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="782f6-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="782f6-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="782f6-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="782f6-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="782f6-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="782f6-169">Response</span></span>

<span data-ttu-id="782f6-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="782f6-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="782f6-171">394</span><span class="sxs-lookup"><span data-stu-id="782f6-171">394</span></span>

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="782f6-172">Пример 4: использование функции CAST и $search для получения членства с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="782f6-172">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="782f6-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="782f6-173">Request</span></span>

<span data-ttu-id="782f6-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="782f6-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="782f6-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="782f6-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="782f6-176">C#</span><span class="sxs-lookup"><span data-stu-id="782f6-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="782f6-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="782f6-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="782f6-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="782f6-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="782f6-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="782f6-179">Response</span></span>

<span data-ttu-id="782f6-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="782f6-180">The following is an example of the response.</span></span>
><span data-ttu-id="782f6-181">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="782f6-181">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="782f6-182">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="782f6-182">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="782f6-183">Пример 5: использование функции CAST и $filter для получения членства с отображаемым именем, начинающимся с буквы "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="782f6-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="782f6-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="782f6-184">Request</span></span>

<span data-ttu-id="782f6-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="782f6-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="782f6-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="782f6-186">Response</span></span>

<span data-ttu-id="782f6-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="782f6-187">The following is an example of the response.</span></span>
><span data-ttu-id="782f6-188">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="782f6-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="782f6-189">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="782f6-189">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
