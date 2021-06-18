---
title: Перечисление user memberOf
description: Получите группы, роли каталогов и административные единицы, в которые пользователь входит напрямую. Эта операция не является транзитивной.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dc874763490136c62e851585aaba3df9c5be3f13
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010229"
---
# <a name="list-user-memberof"></a><span data-ttu-id="f90a0-104">Перечисление user memberOf</span><span class="sxs-lookup"><span data-stu-id="f90a0-104">List user memberOf</span></span>

<span data-ttu-id="f90a0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f90a0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f90a0-106">Получение [групп](../resources/group.md), [ролей каталогов](../resources/directoryrole.md) и [административных единиц](../resources/administrativeunit.md), непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f90a0-106">Get [groups](../resources/group.md), [directory roles](../resources/directoryrole.md), and [administrative units](../resources/administrativeunit.md) that the user is a direct member of.</span></span> <span data-ttu-id="f90a0-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="f90a0-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f90a0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f90a0-108">Permissions</span></span>

<span data-ttu-id="f90a0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f90a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f90a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f90a0-111">Permission type</span></span> | <span data-ttu-id="f90a0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f90a0-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f90a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f90a0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f90a0-114">GroupMember.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f90a0-114">GroupMember.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f90a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f90a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f90a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f90a0-116">Not supported.</span></span> |
| <span data-ttu-id="f90a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f90a0-117">Application</span></span> | <span data-ttu-id="f90a0-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f90a0-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f90a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f90a0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f90a0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f90a0-120">Optional query parameters</span></span>

<span data-ttu-id="f90a0-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f90a0-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="f90a0-122">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f90a0-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="f90a0-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="f90a0-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="f90a0-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="f90a0-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="f90a0-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="f90a0-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f90a0-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f90a0-126">Request headers</span></span>

| <span data-ttu-id="f90a0-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f90a0-127">Header</span></span> | <span data-ttu-id="f90a0-128">Значение</span><span class="sxs-lookup"><span data-stu-id="f90a0-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="f90a0-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f90a0-129">Authorization</span></span>  | <span data-ttu-id="f90a0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f90a0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f90a0-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f90a0-132">ConsistencyLevel</span></span> | <span data-ttu-id="f90a0-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="f90a0-133">eventual.</span></span> <span data-ttu-id="f90a0-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="f90a0-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="f90a0-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="f90a0-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f90a0-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f90a0-136">Request body</span></span>

<span data-ttu-id="f90a0-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f90a0-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f90a0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f90a0-138">Response</span></span>

<span data-ttu-id="f90a0-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f90a0-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f90a0-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="f90a0-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="f90a0-141">Пример 1. Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f90a0-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="f90a0-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f90a0-142">Request</span></span>

<span data-ttu-id="f90a0-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f90a0-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f90a0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f90a0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="f90a0-145">C#</span><span class="sxs-lookup"><span data-stu-id="f90a0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f90a0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f90a0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f90a0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f90a0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f90a0-148">Java</span><span class="sxs-lookup"><span data-stu-id="f90a0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f90a0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f90a0-149">Response</span></span>

<span data-ttu-id="f90a0-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f90a0-150">The following is an example of the response.</span></span>
><span data-ttu-id="f90a0-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f90a0-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="f90a0-152">Пример 2. Получение только количества всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f90a0-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="f90a0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f90a0-153">Request</span></span>

<span data-ttu-id="f90a0-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f90a0-154">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual

17
```

#### <a name="response"></a><span data-ttu-id="f90a0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f90a0-155">Response</span></span>

<span data-ttu-id="f90a0-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f90a0-156">The following is an example of the response.</span></span>
><span data-ttu-id="f90a0-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f90a0-157">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="f90a0-158">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="f90a0-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="f90a0-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f90a0-159">Request</span></span>

<span data-ttu-id="f90a0-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f90a0-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f90a0-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f90a0-161">Response</span></span>

<span data-ttu-id="f90a0-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f90a0-162">The following is an example of the response.</span></span>

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

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="f90a0-163">Пример 4. Использование параметра $search и приведения к OData для получения участия пользователей в группах с отображаемыми именами, содержащими буквы «tier», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="f90a0-163">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f90a0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f90a0-164">Request</span></span>

<span data-ttu-id="f90a0-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f90a0-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f90a0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f90a0-166">Response</span></span>

<span data-ttu-id="f90a0-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f90a0-167">The following is an example of the response.</span></span>
><span data-ttu-id="f90a0-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f90a0-168">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f90a0-169">Пример 5. Использование параметра $filter и приведения к OData для получения групп с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="f90a0-169">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f90a0-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="f90a0-170">Request</span></span>

<span data-ttu-id="f90a0-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f90a0-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f90a0-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="f90a0-172">Response</span></span>

<span data-ttu-id="f90a0-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f90a0-173">The following is an example of the response.</span></span>
><span data-ttu-id="f90a0-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f90a0-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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


