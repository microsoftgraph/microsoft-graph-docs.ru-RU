---
title: Перечисление участников группы
description: Получение списка непосредственных участников группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a1c50dfbee4a4846f40d6372a29b1561a1071f5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954051"
---
# <a name="list-group-members"></a><span data-ttu-id="54dbb-103">Перечисление участников группы</span><span class="sxs-lookup"><span data-stu-id="54dbb-103">List group members</span></span>

<span data-ttu-id="54dbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54dbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54dbb-105">Получение списка непосредственных участников группы.</span><span class="sxs-lookup"><span data-stu-id="54dbb-105">Get a list of the group's direct members.</span></span> <span data-ttu-id="54dbb-106">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="54dbb-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="54dbb-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="54dbb-107">This operation is not transitive.</span></span>

<span data-ttu-id="54dbb-108">Если группа содержит более 100 участников, Microsoft Graph возвращает в отклике свойство `@odata.nextLink`, содержащее URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="54dbb-108">When a group contains more than 100 members, Microsoft Graph returns a `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="54dbb-109">При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="54dbb-109">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="54dbb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54dbb-110">Permissions</span></span>

<span data-ttu-id="54dbb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54dbb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54dbb-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54dbb-113">Permission type</span></span> | <span data-ttu-id="54dbb-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54dbb-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="54dbb-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54dbb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="54dbb-116">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="54dbb-116">Group.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="54dbb-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54dbb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54dbb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54dbb-118">Not supported.</span></span> |
| <span data-ttu-id="54dbb-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54dbb-119">Application</span></span> | <span data-ttu-id="54dbb-120">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="54dbb-120">Group.Read.All, Directory.Read.All</span></span> |

> <span data-ttu-id="54dbb-121">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="54dbb-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]
 
## <a name="http-request"></a><span data-ttu-id="54dbb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54dbb-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54dbb-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54dbb-123">Optional query parameters</span></span>

<span data-ttu-id="54dbb-124">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="54dbb-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="54dbb-125">Кроме того, включено приведение к OData, например, вы можете получить только пользователей, которые являются участниками группы.</span><span class="sxs-lookup"><span data-stu-id="54dbb-125">OData cast is also enabled, for example, you can cast to get just the users that are a member of the group.</span></span> <span data-ttu-id="54dbb-126">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="54dbb-126">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="54dbb-127">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="54dbb-127">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="54dbb-128">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="54dbb-128">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54dbb-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54dbb-129">Request headers</span></span>

| <span data-ttu-id="54dbb-130">Имя</span><span class="sxs-lookup"><span data-stu-id="54dbb-130">Name</span></span> | <span data-ttu-id="54dbb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="54dbb-131">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="54dbb-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54dbb-132">Authorization</span></span> | <span data-ttu-id="54dbb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54dbb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54dbb-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="54dbb-135">ConsistencyLevel</span></span> | <span data-ttu-id="54dbb-136">необязательный.</span><span class="sxs-lookup"><span data-stu-id="54dbb-136">eventual.</span></span> <span data-ttu-id="54dbb-137">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="54dbb-137">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="54dbb-138">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="54dbb-138">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54dbb-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54dbb-139">Request body</span></span>

<span data-ttu-id="54dbb-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54dbb-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54dbb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="54dbb-141">Response</span></span>

<span data-ttu-id="54dbb-142">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54dbb-142">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54dbb-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="54dbb-143">Examples</span></span>

### <a name="example-1-get-the-direct-membership-in-a-group"></a><span data-ttu-id="54dbb-144">Пример 1. Получение сведений о непосредственном участии в группе</span><span class="sxs-lookup"><span data-stu-id="54dbb-144">Example 1: Get the direct membership in a group</span></span>

#### <a name="request"></a><span data-ttu-id="54dbb-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="54dbb-145">Request</span></span>

<span data-ttu-id="54dbb-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54dbb-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54dbb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="54dbb-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="54dbb-148">C#</span><span class="sxs-lookup"><span data-stu-id="54dbb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54dbb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54dbb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54dbb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54dbb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54dbb-151">Java</span><span class="sxs-lookup"><span data-stu-id="54dbb-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="54dbb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="54dbb-152">Response</span></span>

<span data-ttu-id="54dbb-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54dbb-153">The following is an example of the response.</span></span>
><span data-ttu-id="54dbb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54dbb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-membership"></a><span data-ttu-id="54dbb-156">Пример 2. Получение только количества всех участий</span><span class="sxs-lookup"><span data-stu-id="54dbb-156">Example 2: Get only a count of all membership</span></span>

#### <a name="request"></a><span data-ttu-id="54dbb-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="54dbb-157">Request</span></span>

<span data-ttu-id="54dbb-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54dbb-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54dbb-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="54dbb-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="54dbb-160">C#</span><span class="sxs-lookup"><span data-stu-id="54dbb-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54dbb-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54dbb-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54dbb-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54dbb-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54dbb-163">Java</span><span class="sxs-lookup"><span data-stu-id="54dbb-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54dbb-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="54dbb-164">Response</span></span>

<span data-ttu-id="54dbb-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54dbb-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="54dbb-166">893</span><span class="sxs-lookup"><span data-stu-id="54dbb-166">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-user-membership"></a><span data-ttu-id="54dbb-167">Пример 3. Использование приведения к OData для получения только количества участий пользователей</span><span class="sxs-lookup"><span data-stu-id="54dbb-167">Example 3: Use OData cast to get only a count of user membership</span></span>

#### <a name="request"></a><span data-ttu-id="54dbb-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="54dbb-168">Request</span></span>

<span data-ttu-id="54dbb-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54dbb-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54dbb-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="54dbb-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_user_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="54dbb-171">C#</span><span class="sxs-lookup"><span data-stu-id="54dbb-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-user-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54dbb-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54dbb-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-user-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54dbb-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54dbb-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-user-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54dbb-174">Java</span><span class="sxs-lookup"><span data-stu-id="54dbb-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-user-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54dbb-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="54dbb-175">Response</span></span>

<span data-ttu-id="54dbb-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54dbb-176">The following is an example of the response.</span></span>

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

<span data-ttu-id="54dbb-177">893</span><span class="sxs-lookup"><span data-stu-id="54dbb-177">893</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-user-membership-in-groups-with-display-names-that-contain-the-letters-pr-including-a-count-of-returned-objects"></a><span data-ttu-id="54dbb-178">Пример 4: используйте $search и приведение OData для получения членства пользователя в группах с отображаемыми именами, содержащими буквы "PR", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="54dbb-178">Example 4: Use $search and OData cast to get user membership in groups with display names that contain the letters 'Pr' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="54dbb-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="54dbb-179">Request</span></span>

<span data-ttu-id="54dbb-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54dbb-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54dbb-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="54dbb-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pr_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members/microsoft.graph.user?$count=true&$orderby=displayName&$search="displayName:Pr"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="54dbb-182">C#</span><span class="sxs-lookup"><span data-stu-id="54dbb-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pr-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54dbb-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54dbb-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pr-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54dbb-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54dbb-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pr-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54dbb-185">Java</span><span class="sxs-lookup"><span data-stu-id="54dbb-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-pr-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54dbb-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="54dbb-186">Response</span></span>

<span data-ttu-id="54dbb-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54dbb-187">The following is an example of the response.</span></span>
><span data-ttu-id="54dbb-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54dbb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    },
    {
      "displayName":"Preston Morales",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="54dbb-190">Пример 5. Использование параметра $filter для получения участия в группах с отображаемым именем, которое начинается на "А", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="54dbb-190">Example 5: Use $filter to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="54dbb-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="54dbb-191">Request</span></span>

<span data-ttu-id="54dbb-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54dbb-192">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54dbb-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="54dbb-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/members?$count=true&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="54dbb-194">C#</span><span class="sxs-lookup"><span data-stu-id="54dbb-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54dbb-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54dbb-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54dbb-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54dbb-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54dbb-197">Java</span><span class="sxs-lookup"><span data-stu-id="54dbb-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54dbb-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="54dbb-198">Response</span></span>

<span data-ttu-id="54dbb-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54dbb-199">The following is an example of the response.</span></span>
><span data-ttu-id="54dbb-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54dbb-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


