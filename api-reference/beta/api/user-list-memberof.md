---
title: Перечисление user memberOf
description: Получите группы, роли каталогов и административные единицы, в которые пользователь входит напрямую. Эта операция не является транзитивной.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dcbe9a15f768859a2961a5b31b36d4d8b15f8d2f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050733"
---
# <a name="list-user-memberof"></a><span data-ttu-id="c1a31-104">Перечисление user memberOf</span><span class="sxs-lookup"><span data-stu-id="c1a31-104">List user memberOf</span></span>

<span data-ttu-id="c1a31-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a31-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a31-106">Получение [групп](../resources/group.md), [ролей каталогов](../resources/directoryrole.md) и [административных единиц](../resources/administrativeunit.md), непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1a31-106">Get [groups](../resources/group.md), [directory roles](../resources/directoryrole.md), and [administrative units](../resources/administrativeunit.md) that the user is a direct member of.</span></span> <span data-ttu-id="c1a31-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="c1a31-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a31-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a31-108">Permissions</span></span>

<span data-ttu-id="c1a31-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a31-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1a31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a31-111">Permission type</span></span> | <span data-ttu-id="c1a31-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1a31-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="c1a31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1a31-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c1a31-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1a31-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="c1a31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1a31-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a31-116">Not supported.</span></span> |
| <span data-ttu-id="c1a31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1a31-117">Application</span></span> | <span data-ttu-id="c1a31-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a31-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1a31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1a31-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1a31-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1a31-120">Optional query parameters</span></span>

<span data-ttu-id="c1a31-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c1a31-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="c1a31-122">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1a31-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="c1a31-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="c1a31-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="c1a31-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="c1a31-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c1a31-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="c1a31-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1a31-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1a31-126">Request headers</span></span>

| <span data-ttu-id="c1a31-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1a31-127">Header</span></span> | <span data-ttu-id="c1a31-128">Значение</span><span class="sxs-lookup"><span data-stu-id="c1a31-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="c1a31-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1a31-129">Authorization</span></span>  | <span data-ttu-id="c1a31-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a31-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1a31-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c1a31-132">ConsistencyLevel</span></span> | <span data-ttu-id="c1a31-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a31-133">eventual.</span></span> <span data-ttu-id="c1a31-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="c1a31-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c1a31-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="c1a31-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1a31-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1a31-136">Request body</span></span>

<span data-ttu-id="c1a31-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1a31-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1a31-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a31-138">Response</span></span>

<span data-ttu-id="c1a31-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1a31-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1a31-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1a31-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="c1a31-141">Пример 1. Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1a31-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="c1a31-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a31-142">Request</span></span>

<span data-ttu-id="c1a31-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a31-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1a31-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a31-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="c1a31-145">C#</span><span class="sxs-lookup"><span data-stu-id="c1a31-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a31-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a31-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a31-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a31-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1a31-148">Java</span><span class="sxs-lookup"><span data-stu-id="c1a31-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c1a31-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a31-149">Response</span></span>

<span data-ttu-id="c1a31-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a31-150">The following is an example of the response.</span></span>
><span data-ttu-id="c1a31-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1a31-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="c1a31-152">Пример 2. Получение только количества всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1a31-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="c1a31-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a31-153">Request</span></span>

<span data-ttu-id="c1a31-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a31-154">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual

17
```

#### <a name="response"></a><span data-ttu-id="c1a31-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a31-155">Response</span></span>

<span data-ttu-id="c1a31-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a31-156">The following is an example of the response.</span></span>
><span data-ttu-id="c1a31-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1a31-157">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="c1a31-158">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="c1a31-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="c1a31-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a31-159">Request</span></span>

<span data-ttu-id="c1a31-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a31-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c1a31-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a31-161">Response</span></span>

<span data-ttu-id="c1a31-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a31-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

16
```

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="c1a31-163">Пример 4. Использование параметра $search и приведения к OData для получения участия пользователей в группах с отображаемыми именами, содержащими буквы «tier», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="c1a31-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c1a31-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a31-164">Request</span></span>

<span data-ttu-id="c1a31-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a31-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c1a31-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a31-166">Response</span></span>

<span data-ttu-id="c1a31-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a31-167">The following is an example of the response.</span></span>
><span data-ttu-id="c1a31-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1a31-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c1a31-169">Пример 5. Использование параметра $filter и приведения к OData для получения групп с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="c1a31-169">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c1a31-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a31-170">Request</span></span>

<span data-ttu-id="c1a31-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a31-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c1a31-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a31-172">Response</span></span>

<span data-ttu-id="c1a31-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a31-173">The following is an example of the response.</span></span>
><span data-ttu-id="c1a31-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1a31-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


