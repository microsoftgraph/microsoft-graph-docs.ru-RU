---
title: Перечисление orgContacts
description: Получение списка контактов Организации для этой Организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a98715d76933e0925d9b074a6d25788ee3b85ce6
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352191"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="cc24a-103">Перечисление orgContacts</span><span class="sxs-lookup"><span data-stu-id="cc24a-103">List orgContacts</span></span>

<span data-ttu-id="cc24a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc24a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc24a-105">Получение списка контактов Организации для этой Организации.</span><span class="sxs-lookup"><span data-stu-id="cc24a-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc24a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc24a-106">Permissions</span></span>
<span data-ttu-id="cc24a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc24a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc24a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc24a-109">Permission type</span></span>      | <span data-ttu-id="cc24a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc24a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc24a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc24a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc24a-112">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="cc24a-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc24a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc24a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc24a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc24a-114">Not supported.</span></span>    |
|<span data-ttu-id="cc24a-115">Application</span><span class="sxs-lookup"><span data-stu-id="cc24a-115">Application</span></span> | <span data-ttu-id="cc24a-116">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cc24a-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc24a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc24a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc24a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc24a-118">Optional query parameters</span></span>
<span data-ttu-id="cc24a-p102">Этот метод поддерживает [параметры запроса OData](/graph/query_parameters) для настройки отклика, в том числе `$search`, `$count` и `$filter`. Вы можете использовать параметр `$search` в свойстве **displayName**. Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров запроса `$count` и `$search`. Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="cc24a-p102">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc24a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc24a-123">Request headers</span></span>
| <span data-ttu-id="cc24a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cc24a-124">Name</span></span>       | <span data-ttu-id="cc24a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cc24a-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cc24a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc24a-126">Authorization</span></span>  | <span data-ttu-id="cc24a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc24a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc24a-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="cc24a-129">ConsistencyLevel</span></span> | <span data-ttu-id="cc24a-p104">необязательный. Этот заголовок и `$count` требуются при использовании `$search` или применении `$filter` с параметром запроса `$orderby`. В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="cc24a-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc24a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc24a-133">Request body</span></span>
<span data-ttu-id="cc24a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc24a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc24a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc24a-135">Response</span></span>

<span data-ttu-id="cc24a-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc24a-136">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc24a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc24a-137">Examples</span></span>

### <a name="example-1-get-organizational-contacts-for-an-organization"></a><span data-ttu-id="cc24a-138">Пример 1: получение организационных контактов для Организации</span><span class="sxs-lookup"><span data-stu-id="cc24a-138">Example 1: Get organizational contacts for an organization</span></span>

#### <a name="request"></a><span data-ttu-id="cc24a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc24a-139">Request</span></span>

<span data-ttu-id="cc24a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc24a-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc24a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc24a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="cc24a-142">C#</span><span class="sxs-lookup"><span data-stu-id="cc24a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc24a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc24a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc24a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc24a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc24a-145">Java</span><span class="sxs-lookup"><span data-stu-id="cc24a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cc24a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc24a-146">Response</span></span>

<span data-ttu-id="cc24a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc24a-147">Here is an example of the response.</span></span> 
><span data-ttu-id="cc24a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc24a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-organizational-contacts"></a><span data-ttu-id="cc24a-150">Пример 2: получение только количества контактов Организации</span><span class="sxs-lookup"><span data-stu-id="cc24a-150">Example 2: Get only a count of organizational contacts</span></span>

#### <a name="request"></a><span data-ttu-id="cc24a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc24a-151">Request</span></span>

<span data-ttu-id="cc24a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc24a-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cc24a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc24a-153">Response</span></span>

<span data-ttu-id="cc24a-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc24a-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="cc24a-155">893</span><span class="sxs-lookup"><span data-stu-id="cc24a-155">893</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-organizational-contact-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="cc24a-156">Пример 3: использование $filter и $top для получения одного организационного контакта с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="cc24a-156">Example 3: Use $filter and $top to get one organizational contact with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cc24a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc24a-157">Request</span></span>

<span data-ttu-id="cc24a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc24a-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cc24a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc24a-159">Response</span></span>

<span data-ttu-id="cc24a-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc24a-160">The following is an example of the response.</span></span>
><span data-ttu-id="cc24a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc24a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-organizational-contacts-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="cc24a-163">Пример 4: использование $search для получения организационных контактов с отображаемыми именами, содержащими "WA", в том числе от количества возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="cc24a-163">Example 4: Use $search to get organizational contacts with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cc24a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc24a-164">Request</span></span>

<span data-ttu-id="cc24a-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc24a-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_phone_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts?$search="displayName:wa"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cc24a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc24a-166">Response</span></span>

<span data-ttu-id="cc24a-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc24a-167">The following is an example of the response.</span></span>
><span data-ttu-id="cc24a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc24a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


