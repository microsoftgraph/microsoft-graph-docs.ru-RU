---
title: Перечисление orgContacts
description: Получение списка контактов Организации для этой Организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 85992f10a29962c2ceea9ca9fcfd8f0ce3353a71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969517"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="af4d3-103">Перечисление orgContacts</span><span class="sxs-lookup"><span data-stu-id="af4d3-103">List orgContacts</span></span>

<span data-ttu-id="af4d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af4d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af4d3-105">Получение списка контактов Организации для этой Организации.</span><span class="sxs-lookup"><span data-stu-id="af4d3-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="af4d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af4d3-106">Permissions</span></span>
<span data-ttu-id="af4d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af4d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af4d3-109">Permission type</span></span>      | <span data-ttu-id="af4d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af4d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af4d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af4d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af4d3-112">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="af4d3-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af4d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af4d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af4d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af4d3-114">Not supported.</span></span>    |
|<span data-ttu-id="af4d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af4d3-115">Application</span></span> | <span data-ttu-id="af4d3-116">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af4d3-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af4d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af4d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af4d3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="af4d3-118">Optional query parameters</span></span>
<span data-ttu-id="af4d3-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="af4d3-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="af4d3-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="af4d3-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="af4d3-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="af4d3-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="af4d3-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="af4d3-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af4d3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af4d3-123">Request headers</span></span>
| <span data-ttu-id="af4d3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="af4d3-124">Name</span></span>       | <span data-ttu-id="af4d3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="af4d3-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="af4d3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af4d3-126">Authorization</span></span>  | <span data-ttu-id="af4d3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af4d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af4d3-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="af4d3-129">ConsistencyLevel</span></span> | <span data-ttu-id="af4d3-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="af4d3-130">eventual.</span></span> <span data-ttu-id="af4d3-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="af4d3-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="af4d3-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="af4d3-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af4d3-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af4d3-133">Request body</span></span>
<span data-ttu-id="af4d3-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af4d3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af4d3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4d3-135">Response</span></span>

<span data-ttu-id="af4d3-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af4d3-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af4d3-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="af4d3-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="af4d3-138">Пример 1: получение организационных контактов для Организации</span><span class="sxs-lookup"><span data-stu-id="af4d3-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="af4d3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="af4d3-139">Request</span></span>

<span data-ttu-id="af4d3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af4d3-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af4d3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="af4d3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="af4d3-142">C#</span><span class="sxs-lookup"><span data-stu-id="af4d3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af4d3-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af4d3-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af4d3-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af4d3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="af4d3-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4d3-145">Response</span></span>

<span data-ttu-id="af4d3-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af4d3-146">Here is an example of the response.</span></span> 
><span data-ttu-id="af4d3-147">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af4d3-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="af4d3-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af4d3-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="af4d3-149">Пример 2: получение только количества контактов Организации</span><span class="sxs-lookup"><span data-stu-id="af4d3-149">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="af4d3-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="af4d3-150">Request</span></span>

<span data-ttu-id="af4d3-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af4d3-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="af4d3-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="af4d3-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="af4d3-153">C#</span><span class="sxs-lookup"><span data-stu-id="af4d3-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af4d3-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af4d3-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af4d3-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af4d3-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="af4d3-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4d3-156">Response</span></span>

<span data-ttu-id="af4d3-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af4d3-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="af4d3-158">893</span><span class="sxs-lookup"><span data-stu-id="af4d3-158">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="af4d3-159">Пример 3: использование $filter и $top для получения одного организационного контакта с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="af4d3-159">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="af4d3-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="af4d3-160">Request</span></span>

<span data-ttu-id="af4d3-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af4d3-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="af4d3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="af4d3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="af4d3-163">C#</span><span class="sxs-lookup"><span data-stu-id="af4d3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af4d3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af4d3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af4d3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af4d3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="af4d3-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4d3-166">Response</span></span>

<span data-ttu-id="af4d3-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af4d3-167">The following is an example of the response.</span></span>
><span data-ttu-id="af4d3-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af4d3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="af4d3-170">Пример 4: использование $search для получения организационных контактов с отображаемыми именами, содержащими "WA", в том числе от количества возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="af4d3-170">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="af4d3-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="af4d3-171">Request</span></span>

<span data-ttu-id="af4d3-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af4d3-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="af4d3-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="af4d3-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="af4d3-174">C#</span><span class="sxs-lookup"><span data-stu-id="af4d3-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phone-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af4d3-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af4d3-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phone-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af4d3-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af4d3-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phone-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="af4d3-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="af4d3-177">Response</span></span>

<span data-ttu-id="af4d3-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af4d3-178">The following is an example of the response.</span></span>
><span data-ttu-id="af4d3-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af4d3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
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


