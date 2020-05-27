---
title: Список servicePrincipal memberOf
description: Получение групп и ролей каталогов, непосредственным участником которых является данный участник службы. Эта операция не является транзитивной.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 2d36c6b57fc5b73b0faec50d73de67a575aed811
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383114"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="6ecca-104">Список servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="6ecca-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="6ecca-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ecca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ecca-106">Получение групп и ролей каталогов, непосредственным участником которых является [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="6ecca-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="6ecca-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="6ecca-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ecca-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecca-108">Permissions</span></span>

<span data-ttu-id="6ecca-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ecca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecca-111">Permission type</span></span>      | <span data-ttu-id="6ecca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ecca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ecca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ecca-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6ecca-114">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="6ecca-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ecca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ecca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ecca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ecca-116">Not supported.</span></span>    |
|<span data-ttu-id="6ecca-117">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="6ecca-117">Application</span></span> | <span data-ttu-id="6ecca-118">Application. Read. ALL, Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6ecca-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6ecca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ecca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ecca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ecca-120">Optional query parameters</span></span>

<span data-ttu-id="6ecca-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="6ecca-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="6ecca-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только перечисление directoryrole, членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ecca-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="6ecca-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="6ecca-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="6ecca-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecca-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6ecca-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="6ecca-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ecca-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ecca-126">Request headers</span></span>

| <span data-ttu-id="6ecca-127">Имя</span><span class="sxs-lookup"><span data-stu-id="6ecca-127">Name</span></span>       | <span data-ttu-id="6ecca-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6ecca-128">Type</span></span> | <span data-ttu-id="6ecca-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6ecca-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ecca-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ecca-130">Authorization</span></span>  | <span data-ttu-id="6ecca-131">string</span><span class="sxs-lookup"><span data-stu-id="6ecca-131">string</span></span>  | <span data-ttu-id="6ecca-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ecca-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ecca-134">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="6ecca-134">ConsistencyLevel</span></span> | <span data-ttu-id="6ecca-135">закончить.</span><span class="sxs-lookup"><span data-stu-id="6ecca-135">eventual.</span></span> <span data-ttu-id="6ecca-136">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="6ecca-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="6ecca-137">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="6ecca-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ecca-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ecca-138">Request body</span></span>
<span data-ttu-id="6ecca-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ecca-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ecca-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecca-140">Response</span></span>

<span data-ttu-id="6ecca-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecca-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ecca-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ecca-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="6ecca-143">Пример 1: получение групп и ролей каталогов, непосредственным участником которых является участник службы</span><span class="sxs-lookup"><span data-stu-id="6ecca-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="6ecca-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecca-144">Request</span></span>

<span data-ttu-id="6ecca-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecca-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ecca-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ecca-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="6ecca-147">C#</span><span class="sxs-lookup"><span data-stu-id="6ecca-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ecca-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ecca-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ecca-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ecca-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ecca-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecca-150">Response</span></span>

<span data-ttu-id="6ecca-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecca-151">The following is an example of the response.</span></span> 
> <span data-ttu-id="6ecca-152">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6ecca-152">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6ecca-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ecca-153">All of the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="6ecca-154">Пример 2: получение только количества всех членств</span><span class="sxs-lookup"><span data-stu-id="6ecca-154">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="6ecca-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecca-155">Request</span></span>

<span data-ttu-id="6ecca-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecca-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ecca-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ecca-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6ecca-158">C#</span><span class="sxs-lookup"><span data-stu-id="6ecca-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ecca-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ecca-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ecca-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ecca-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ecca-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecca-161">Response</span></span>

<span data-ttu-id="6ecca-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecca-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="6ecca-163">394</span><span class="sxs-lookup"><span data-stu-id="6ecca-163">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="6ecca-164">Пример 3: Использование приведения OData для получения только количества участников группы</span><span class="sxs-lookup"><span data-stu-id="6ecca-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="6ecca-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecca-165">Request</span></span>

<span data-ttu-id="6ecca-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecca-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ecca-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ecca-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="6ecca-168">C#</span><span class="sxs-lookup"><span data-stu-id="6ecca-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-group-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ecca-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ecca-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-group-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ecca-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ecca-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-group-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6ecca-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ecca-171">Response</span></span>

<span data-ttu-id="6ecca-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecca-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="6ecca-173">394</span><span class="sxs-lookup"><span data-stu-id="6ecca-173">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="6ecca-174">Пример 4: использование $search и функции OData для получения сведений о членстве в группах с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="6ecca-174">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6ecca-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecca-175">Request</span></span>

<span data-ttu-id="6ecca-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecca-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6ecca-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ecca-177">Response</span></span>

<span data-ttu-id="6ecca-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecca-178">The following is an example of the response.</span></span>
><span data-ttu-id="6ecca-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ecca-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6ecca-181">Пример 5: используйте $filter и приведение OData для получения сведений о членстве в группах с отображаемым именем, начинающимся с буквы "A", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="6ecca-181">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6ecca-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecca-182">Request</span></span>

<span data-ttu-id="6ecca-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecca-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6ecca-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ecca-184">Response</span></span>

<span data-ttu-id="6ecca-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecca-185">The following is an example of the response.</span></span>
><span data-ttu-id="6ecca-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ecca-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
