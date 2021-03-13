---
title: Перечисление orgContacts
description: Извлечение списка организационных контактов для этой организации.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4919459f6501974970edbdafe51bb97bececd42f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761586"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="0b8b1-103">Перечисление orgContacts</span><span class="sxs-lookup"><span data-stu-id="0b8b1-103">List orgContacts</span></span>

<span data-ttu-id="0b8b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b8b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b8b1-105">Получите список [организационных контактов](../resources/orgcontact.md) для этой организации.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b8b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b8b1-106">Permissions</span></span>
<span data-ttu-id="0b8b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b8b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b8b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b8b1-109">Permission type</span></span>      | <span data-ttu-id="0b8b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b8b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b8b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b8b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b8b1-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b8b1-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b8b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b8b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b8b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-114">Not supported.</span></span>    |
|<span data-ttu-id="0b8b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b8b1-115">Application</span></span> | <span data-ttu-id="0b8b1-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8b1-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b8b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b8b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b8b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b8b1-118">Optional query parameters</span></span>
<span data-ttu-id="0b8b1-119">Этот метод поддерживает [параметры запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$expand` `$filter` `$search` `$select` `$top` .</span><span class="sxs-lookup"><span data-stu-id="0b8b1-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$expand`, `$filter`, `$search`,`$select`, and `$top`.</span></span> <span data-ttu-id="0b8b1-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="0b8b1-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0b8b1-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b8b1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b8b1-123">Request headers</span></span>
| <span data-ttu-id="0b8b1-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b8b1-124">Header</span></span>       | <span data-ttu-id="0b8b1-125">Значение</span><span class="sxs-lookup"><span data-stu-id="0b8b1-125">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="0b8b1-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b8b1-126">Authorization</span></span>  |<span data-ttu-id="0b8b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b8b1-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="0b8b1-129">ConsistencyLevel</span></span> | <span data-ttu-id="0b8b1-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-130">eventual.</span></span> <span data-ttu-id="0b8b1-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="0b8b1-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b8b1-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b8b1-133">Request body</span></span>
<span data-ttu-id="0b8b1-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b8b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8b1-135">Response</span></span>

<span data-ttu-id="0b8b1-136">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b8b1-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b8b1-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="0b8b1-138">Пример 1. Получить организационные контакты для организации</span><span class="sxs-lookup"><span data-stu-id="0b8b1-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="0b8b1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b8b1-139">Request</span></span>

<span data-ttu-id="0b8b1-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b8b1-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8b1-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="0b8b1-142">C#</span><span class="sxs-lookup"><span data-stu-id="0b8b1-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b8b1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b8b1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b8b1-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b8b1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b8b1-145">Java</span><span class="sxs-lookup"><span data-stu-id="0b8b1-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0b8b1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8b1-146">Response</span></span>

<span data-ttu-id="0b8b1-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-147">The following is an example of the response.</span></span>

><span data-ttu-id="0b8b1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "companyName": "Contoso",
      "department": "Marketing",
      "displayName": "Eric S",
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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="0b8b1-150">Пример 2. Получить только количество организационных контактов</span><span class="sxs-lookup"><span data-stu-id="0b8b1-150">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="0b8b1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b8b1-151">Request</span></span>

<span data-ttu-id="0b8b1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b8b1-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8b1-153">Response</span></span>

<span data-ttu-id="0b8b1-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0b8b1-155">Пример 3. Использование $filter и $top для получения одного организационного контакта с именем отображения, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="0b8b1-155">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0b8b1-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b8b1-156">Request</span></span>

<span data-ttu-id="0b8b1-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b8b1-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8b1-158">Response</span></span>

<span data-ttu-id="0b8b1-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-159">The following is an example of the response.</span></span>

><span data-ttu-id="0b8b1-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="0b8b1-162">Пример 4. Использование $search для получения организационных контактов с именами отображения, которые содержат буквы "wa", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="0b8b1-162">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0b8b1-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b8b1-163">Request</span></span>

<span data-ttu-id="0b8b1-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b8b1-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8b1-165">Response</span></span>

<span data-ttu-id="0b8b1-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-166">The following is an example of the response.</span></span>

><span data-ttu-id="0b8b1-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b8b1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
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

