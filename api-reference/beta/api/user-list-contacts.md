---
title: Список контактов
description: Получение контактов в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653225d9feb929dc3694ec4a473f890b5485c608
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421038"
---
# <a name="list-contacts"></a><span data-ttu-id="cdadc-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="cdadc-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdadc-104">Получение контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="cdadc-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="cdadc-105">Существует два сценария, с помощью которых приложение может получить контакты из папки контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="cdadc-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="cdadc-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="cdadc-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="cdadc-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="cdadc-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="cdadc-108">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="cdadc-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="cdadc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdadc-109">Permissions</span></span>
<span data-ttu-id="cdadc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdadc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdadc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdadc-112">Permission type</span></span>      | <span data-ttu-id="cdadc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdadc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdadc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdadc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cdadc-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdadc-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cdadc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdadc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdadc-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdadc-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cdadc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdadc-118">Application</span></span> | <span data-ttu-id="cdadc-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdadc-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdadc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdadc-120">HTTP request</span></span>

<span data-ttu-id="cdadc-121">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="cdadc-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="cdadc-122">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="cdadc-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdadc-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdadc-123">Optional query parameters</span></span>
<span data-ttu-id="cdadc-124">С помощью параметра запроса `$filter` можно фильтровать контакты на основе адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="cdadc-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="cdadc-125">Обратите внимание, что вы можете использовать оператор `$filter`, `any`, и `eq` только для дочернего свойства **address** для экземпляров коллекции **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="cdadc-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="cdadc-126">Т.е. вы не можете выполнять фильтрацию с помощью дочернего свойства **name** или другого дочернего свойства экземпляра **emailAddresses**, как и не можете применять другие операторы или функции с `filter`, такие как `ne`, `le` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="cdadc-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="cdadc-127">Общие сведения о параметре запроса `$filter` см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cdadc-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdadc-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdadc-128">Request headers</span></span>
| <span data-ttu-id="cdadc-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdadc-129">Header</span></span>       | <span data-ttu-id="cdadc-130">Значение</span><span class="sxs-lookup"><span data-stu-id="cdadc-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdadc-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdadc-131">Authorization</span></span>  | <span data-ttu-id="cdadc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdadc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdadc-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdadc-134">Request body</span></span>
<span data-ttu-id="cdadc-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdadc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdadc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdadc-136">Response</span></span>

<span data-ttu-id="cdadc-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdadc-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdadc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cdadc-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdadc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdadc-139">Request</span></span>
<span data-ttu-id="cdadc-140">В следующем примере возвращаются свойства **DisplayName** и **EmailAddresses** для контактов вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="cdadc-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cdadc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdadc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cdadc-142">C#</span><span class="sxs-lookup"><span data-stu-id="cdadc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cdadc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdadc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cdadc-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cdadc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="cdadc-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdadc-145">Response</span></span>
<span data-ttu-id="cdadc-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdadc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
