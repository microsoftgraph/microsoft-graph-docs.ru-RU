---
title: Список Оргконтактс
description: Получение списка контактов Организации для этой Организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a44c82b6eef63863577bfd64e44e3ab020fc67a0
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336784"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="51afb-103">Список Оргконтактс</span><span class="sxs-lookup"><span data-stu-id="51afb-103">List orgContacts</span></span>

<span data-ttu-id="51afb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51afb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51afb-105">Получение списка контактов Организации для этой Организации.</span><span class="sxs-lookup"><span data-stu-id="51afb-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="51afb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51afb-106">Permissions</span></span>
<span data-ttu-id="51afb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51afb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51afb-109">Permission type</span></span>      | <span data-ttu-id="51afb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51afb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51afb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51afb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="51afb-112">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="51afb-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51afb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51afb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51afb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51afb-114">Not supported.</span></span>    |
|<span data-ttu-id="51afb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51afb-115">Application</span></span> | <span data-ttu-id="51afb-116">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="51afb-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51afb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51afb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="51afb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51afb-118">Optional query parameters</span></span>
<span data-ttu-id="51afb-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="51afb-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="51afb-120">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="51afb-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="51afb-121">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="51afb-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="51afb-122">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="51afb-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51afb-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51afb-123">Request headers</span></span>
| <span data-ttu-id="51afb-124">Имя</span><span class="sxs-lookup"><span data-stu-id="51afb-124">Name</span></span>       | <span data-ttu-id="51afb-125">Описание</span><span class="sxs-lookup"><span data-stu-id="51afb-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="51afb-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51afb-126">Authorization</span></span>  | <span data-ttu-id="51afb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51afb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51afb-129">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="51afb-129">ConsistencyLevel</span></span> | <span data-ttu-id="51afb-130">закончить.</span><span class="sxs-lookup"><span data-stu-id="51afb-130">eventual.</span></span> <span data-ttu-id="51afb-131">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="51afb-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="51afb-132">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="51afb-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51afb-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51afb-133">Request body</span></span>
<span data-ttu-id="51afb-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51afb-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51afb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="51afb-135">Response</span></span>

<span data-ttu-id="51afb-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51afb-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51afb-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="51afb-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="51afb-138">Пример 1: получение организационных контактов для Организации</span><span class="sxs-lookup"><span data-stu-id="51afb-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="51afb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="51afb-139">Request</span></span>

<span data-ttu-id="51afb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51afb-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51afb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="51afb-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="51afb-142">C#</span><span class="sxs-lookup"><span data-stu-id="51afb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51afb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51afb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51afb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51afb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="51afb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="51afb-145">Response</span></span>

<span data-ttu-id="51afb-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51afb-146">Here is an example of the response.</span></span> 
><span data-ttu-id="51afb-147">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="51afb-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51afb-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51afb-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="51afb-149">Пример 2: получение только количества контактов Организации</span><span class="sxs-lookup"><span data-stu-id="51afb-149">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="51afb-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="51afb-150">Request</span></span>

<span data-ttu-id="51afb-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51afb-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51afb-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="51afb-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="51afb-153">C#</span><span class="sxs-lookup"><span data-stu-id="51afb-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51afb-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51afb-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51afb-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51afb-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51afb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="51afb-156">Response</span></span>

<span data-ttu-id="51afb-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51afb-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="51afb-158">893</span><span class="sxs-lookup"><span data-stu-id="51afb-158">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="51afb-159">Пример 3: использование $filter и $top для получения одного организационного контакта с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="51afb-159">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="51afb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="51afb-160">Request</span></span>

<span data-ttu-id="51afb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51afb-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51afb-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="51afb-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="51afb-163">C#</span><span class="sxs-lookup"><span data-stu-id="51afb-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51afb-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51afb-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51afb-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51afb-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51afb-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="51afb-166">Response</span></span>

<span data-ttu-id="51afb-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51afb-167">The following is an example of the response.</span></span>
><span data-ttu-id="51afb-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51afb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="51afb-170">Пример 4: использование $search для получения организационных контактов с отображаемыми именами, содержащими "WA", в том числе от количества возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="51afb-170">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="51afb-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="51afb-171">Request</span></span>

<span data-ttu-id="51afb-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51afb-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51afb-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="51afb-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="51afb-174">C#</span><span class="sxs-lookup"><span data-stu-id="51afb-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phone-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51afb-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51afb-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phone-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51afb-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51afb-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phone-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51afb-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="51afb-177">Response</span></span>

<span data-ttu-id="51afb-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51afb-178">The following is an example of the response.</span></span>
><span data-ttu-id="51afb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51afb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
