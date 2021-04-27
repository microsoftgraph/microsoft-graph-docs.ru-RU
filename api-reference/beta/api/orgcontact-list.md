---
title: Перечисление orgContacts
description: Извлечение списка организационных контактов для этой организации.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: afc6c26238f3f63b71d5c4b1cb0fae28316daa39
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055528"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="47bda-103">Перечисление orgContacts</span><span class="sxs-lookup"><span data-stu-id="47bda-103">List orgContacts</span></span>

<span data-ttu-id="47bda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47bda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47bda-105">Получите список организационных контактов для этой организации.</span><span class="sxs-lookup"><span data-stu-id="47bda-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="47bda-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47bda-106">Permissions</span></span>
<span data-ttu-id="47bda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47bda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bda-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47bda-109">Permission type</span></span>      | <span data-ttu-id="47bda-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47bda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47bda-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47bda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="47bda-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47bda-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47bda-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47bda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47bda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47bda-114">Not supported.</span></span>    |
|<span data-ttu-id="47bda-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="47bda-115">Application</span></span> | <span data-ttu-id="47bda-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47bda-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47bda-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47bda-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="47bda-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47bda-118">Optional query parameters</span></span>
<span data-ttu-id="47bda-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="47bda-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="47bda-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="47bda-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="47bda-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="47bda-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="47bda-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="47bda-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47bda-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47bda-123">Request headers</span></span>
| <span data-ttu-id="47bda-124">Имя</span><span class="sxs-lookup"><span data-stu-id="47bda-124">Name</span></span>       | <span data-ttu-id="47bda-125">Описание</span><span class="sxs-lookup"><span data-stu-id="47bda-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="47bda-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47bda-126">Authorization</span></span>  | <span data-ttu-id="47bda-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47bda-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47bda-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="47bda-129">ConsistencyLevel</span></span> | <span data-ttu-id="47bda-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="47bda-130">eventual.</span></span> <span data-ttu-id="47bda-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="47bda-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="47bda-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="47bda-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47bda-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47bda-133">Request body</span></span>
<span data-ttu-id="47bda-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47bda-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47bda-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="47bda-135">Response</span></span>

<span data-ttu-id="47bda-136">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47bda-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47bda-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="47bda-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="47bda-138">Пример 1. Получить организационные контакты для организации</span><span class="sxs-lookup"><span data-stu-id="47bda-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="47bda-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="47bda-139">Request</span></span>

<span data-ttu-id="47bda-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47bda-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47bda-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="47bda-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="47bda-142">C#</span><span class="sxs-lookup"><span data-stu-id="47bda-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47bda-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47bda-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47bda-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47bda-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47bda-145">Java</span><span class="sxs-lookup"><span data-stu-id="47bda-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="47bda-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="47bda-146">Response</span></span>

<span data-ttu-id="47bda-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47bda-147">Here is an example of the response.</span></span> 
><span data-ttu-id="47bda-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="47bda-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="47bda-149">Пример 2. Получить только количество организационных контактов</span><span class="sxs-lookup"><span data-stu-id="47bda-149">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="47bda-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="47bda-150">Request</span></span>

<span data-ttu-id="47bda-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47bda-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="47bda-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="47bda-152">Response</span></span>

<span data-ttu-id="47bda-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47bda-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="47bda-154">893</span><span class="sxs-lookup"><span data-stu-id="47bda-154">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="47bda-155">Пример 3. Использование $filter и $top для получения одного организационного контакта с именем отображения, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="47bda-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="47bda-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="47bda-156">Request</span></span>

<span data-ttu-id="47bda-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47bda-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="47bda-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="47bda-158">Response</span></span>

<span data-ttu-id="47bda-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47bda-159">The following is an example of the response.</span></span>
><span data-ttu-id="47bda-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="47bda-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="47bda-161">Пример 4. Использование $search для получения организационных контактов с именами отображения, которые содержат буквы "wa", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="47bda-161">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="47bda-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="47bda-162">Request</span></span>

<span data-ttu-id="47bda-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47bda-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="47bda-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="47bda-164">Response</span></span>

<span data-ttu-id="47bda-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47bda-165">The following is an example of the response.</span></span>
><span data-ttu-id="47bda-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="47bda-166">**Note:** The response object shown here might be shortened for readability.</span></span>

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


