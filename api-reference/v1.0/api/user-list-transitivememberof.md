---
title: Перечисление user transitive memberOf
description: Получите группы, роли каталога, в которые входит пользователь. Этот запрос API является транзитным и также возвращает все группы, вложенные пользователем.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ca969071ec4487bf4c6753441e68db7b77206327
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053778"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="4dc23-104">Перечисление user transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="4dc23-104">List user transitive memberOf</span></span>

<span data-ttu-id="4dc23-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc23-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4dc23-106">Получите группы, роли каталога, в которые входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="4dc23-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="4dc23-107">Этот запрос API является транзитным и также возвращает все группы, вложенные пользователем.</span><span class="sxs-lookup"><span data-stu-id="4dc23-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dc23-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc23-108">Permissions</span></span>

<span data-ttu-id="4dc23-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc23-111">Permission type</span></span>      | <span data-ttu-id="4dc23-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dc23-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dc23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dc23-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4dc23-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4dc23-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4dc23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dc23-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dc23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dc23-116">Not supported.</span></span>    |
|<span data-ttu-id="4dc23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dc23-117">Application</span></span> | <span data-ttu-id="4dc23-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc23-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="4dc23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dc23-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4dc23-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4dc23-120">Optional query parameters</span></span>

<span data-ttu-id="4dc23-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="4dc23-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="4dc23-122">Также включено литье OData, например, можно литье, чтобы получить только транзитное членство в группах.</span><span class="sxs-lookup"><span data-stu-id="4dc23-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="4dc23-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="4dc23-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="4dc23-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="4dc23-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="4dc23-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="4dc23-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dc23-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dc23-126">Request headers</span></span>

| <span data-ttu-id="4dc23-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dc23-127">Header</span></span>       | <span data-ttu-id="4dc23-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4dc23-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4dc23-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dc23-129">Authorization</span></span>  | <span data-ttu-id="4dc23-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dc23-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4dc23-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="4dc23-132">ConsistencyLevel</span></span> | <span data-ttu-id="4dc23-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="4dc23-133">eventual.</span></span> <span data-ttu-id="4dc23-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="4dc23-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="4dc23-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="4dc23-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dc23-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dc23-136">Request body</span></span>

<span data-ttu-id="4dc23-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dc23-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dc23-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc23-138">Response</span></span>

<span data-ttu-id="4dc23-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4dc23-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4dc23-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="4dc23-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="4dc23-141">Пример 1. Получить группы, роли каталогов и административные единицы, в которые пользователь входит</span><span class="sxs-lookup"><span data-stu-id="4dc23-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="4dc23-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc23-142">Request</span></span>

<span data-ttu-id="4dc23-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc23-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4dc23-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc23-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="4dc23-145">C#</span><span class="sxs-lookup"><span data-stu-id="4dc23-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dc23-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dc23-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dc23-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dc23-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4dc23-148">Java</span><span class="sxs-lookup"><span data-stu-id="4dc23-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4dc23-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc23-149">Response</span></span>

<span data-ttu-id="4dc23-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dc23-150">The following is an example of the response.</span></span>

><span data-ttu-id="4dc23-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4dc23-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="4dc23-152">Пример 2. Получить только число транзитных членов в группах, ролях каталогов и административных единицах</span><span class="sxs-lookup"><span data-stu-id="4dc23-152">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="4dc23-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc23-153">Request</span></span>

<span data-ttu-id="4dc23-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc23-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4dc23-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc23-155">Response</span></span>

<span data-ttu-id="4dc23-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dc23-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="4dc23-157">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="4dc23-157">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="4dc23-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc23-158">Request</span></span>

<span data-ttu-id="4dc23-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc23-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4dc23-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc23-160">Response</span></span>

<span data-ttu-id="4dc23-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dc23-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
  } -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

588
```

### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="4dc23-162">Пример 4. Использование $search и OData для получения переходного членства в группах с отображаемыми именами, содержами буквы "tier", включая количество возвращенных объектов.</span><span class="sxs-lookup"><span data-stu-id="4dc23-162">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4dc23-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc23-163">Request</span></span>

<span data-ttu-id="4dc23-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc23-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4dc23-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc23-165">Response</span></span>

<span data-ttu-id="4dc23-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dc23-166">The following is an example of the response.</span></span>

><span data-ttu-id="4dc23-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4dc23-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="4dc23-168">Пример 5. Использование $filter и OData для получения переходного членства в группах с именем отображения, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="4dc23-168">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4dc23-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc23-169">Request</span></span>

<span data-ttu-id="4dc23-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc23-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4dc23-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc23-171">Response</span></span>

<span data-ttu-id="4dc23-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4dc23-172">The following is an example of the response.</span></span>

><span data-ttu-id="4dc23-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4dc23-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
