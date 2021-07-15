---
title: Перечисление orgContacts
description: Извлечение списка организационных контактов для этой организации.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b848c97277882b9f925117f6765c41c050cb7b0b
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430293"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="72b26-103">Перечисление orgContacts</span><span class="sxs-lookup"><span data-stu-id="72b26-103">List orgContacts</span></span>

<span data-ttu-id="72b26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b26-105">Получите список организационных контактов для этой организации.</span><span class="sxs-lookup"><span data-stu-id="72b26-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="72b26-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72b26-106">Permissions</span></span>
<span data-ttu-id="72b26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72b26-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72b26-109">Permission type</span></span>      | <span data-ttu-id="72b26-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72b26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72b26-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72b26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72b26-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72b26-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72b26-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72b26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72b26-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72b26-114">Not supported.</span></span>    |
|<span data-ttu-id="72b26-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="72b26-115">Application</span></span> | <span data-ttu-id="72b26-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72b26-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72b26-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72b26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72b26-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72b26-118">Optional query parameters</span></span>
<span data-ttu-id="72b26-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="72b26-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="72b26-120">Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`.</span><span class="sxs-lookup"><span data-stu-id="72b26-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="72b26-121">Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="72b26-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72b26-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72b26-122">Request headers</span></span>
| <span data-ttu-id="72b26-123">Имя</span><span class="sxs-lookup"><span data-stu-id="72b26-123">Name</span></span>       | <span data-ttu-id="72b26-124">Описание</span><span class="sxs-lookup"><span data-stu-id="72b26-124">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="72b26-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72b26-125">Authorization</span></span>  | <span data-ttu-id="72b26-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72b26-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72b26-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="72b26-128">ConsistencyLevel</span></span> | <span data-ttu-id="72b26-129">необязательный.</span><span class="sxs-lookup"><span data-stu-id="72b26-129">eventual.</span></span> <span data-ttu-id="72b26-130">Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`.</span><span class="sxs-lookup"><span data-stu-id="72b26-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="72b26-131">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="72b26-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="72b26-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72b26-132">Request body</span></span>
<span data-ttu-id="72b26-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72b26-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72b26-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b26-134">Response</span></span>

<span data-ttu-id="72b26-135">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72b26-135">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72b26-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="72b26-136">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="72b26-137">Пример 1. Получить организационные контакты для организации</span><span class="sxs-lookup"><span data-stu-id="72b26-137">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="72b26-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="72b26-138">Request</span></span>

<span data-ttu-id="72b26-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72b26-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72b26-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="72b26-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="72b26-141">C#</span><span class="sxs-lookup"><span data-stu-id="72b26-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72b26-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72b26-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72b26-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72b26-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72b26-144">Java</span><span class="sxs-lookup"><span data-stu-id="72b26-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="72b26-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b26-145">Response</span></span>

<span data-ttu-id="72b26-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72b26-146">Here is an example of the response.</span></span> 
><span data-ttu-id="72b26-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72b26-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "companyName":"Contoso",
      "department":"Accounting",
      "displayName":"Eric Solomon",
      "givenName":"Eric",
      "jobTitle":"Accountant",
      "mail":"erics@contoso.com",
      "mailNickname":"erics",
      "surname":"Solomon",
      "addresses":[
        {
          "city":"MyCity",
          "countryOrRegion":"United States",
          "officeLocation":"MyCity",
          "postalCode":"98000",
          "state":"WA",
          "street":"Contoso Way"
        }
      ],
      "phones":[
        {
          "number":"111-1111",
          "type":"businessFax"
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="72b26-148">Пример 2. Получить только количество организационных контактов</span><span class="sxs-lookup"><span data-stu-id="72b26-148">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="72b26-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="72b26-149">Request</span></span>

<span data-ttu-id="72b26-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72b26-150">The following is an example of the request.</span></span> <span data-ttu-id="72b26-151">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`.</span><span class="sxs-lookup"><span data-stu-id="72b26-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="72b26-152">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="72b26-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="72b26-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b26-153">Response</span></span>

<span data-ttu-id="72b26-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72b26-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="72b26-155">Пример 3. Использование $filter и $top для получения одного организационного контакта с именем отображения, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="72b26-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="72b26-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="72b26-156">Request</span></span>

<span data-ttu-id="72b26-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72b26-157">The following is an example of the request.</span></span> <span data-ttu-id="72b26-158">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`.</span><span class="sxs-lookup"><span data-stu-id="72b26-158">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="72b26-159">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="72b26-159">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="72b26-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b26-160">Response</span></span>

<span data-ttu-id="72b26-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72b26-161">The following is an example of the response.</span></span>
><span data-ttu-id="72b26-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72b26-162">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.count":1,
  "value":[
    {
      "displayName":"Abigail Jackson",
      "mail":"abigailJ@contoso.com",
      "mailNickname":"abigailJ"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="72b26-163">Пример 4. Использование $search для получения организационных контактов с именами отображения, которые содержат буквы "wa", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="72b26-163">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="72b26-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="72b26-164">Request</span></span>

<span data-ttu-id="72b26-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72b26-165">The following is an example of the request.</span></span> <span data-ttu-id="72b26-166">Этот запрос требует заглавного **загона ConsistencyLevel,** так как строка запроса `eventual` находится в `$search` `$count=true` запросе.</span><span class="sxs-lookup"><span data-stu-id="72b26-166">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="72b26-167">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="72b26-167">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="72b26-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b26-168">Response</span></span>

<span data-ttu-id="72b26-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72b26-169">The following is an example of the response.</span></span>
><span data-ttu-id="72b26-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72b26-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.count":22,
  "value":[
    {
      "displayName":"Nicole Wagner",
      "mail":"nicolewa@contoso.com",
      "mailNickname":"nicolewa"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


