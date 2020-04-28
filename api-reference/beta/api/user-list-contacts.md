---
title: Список контактов
description: Получение контактов в почтовом ящике пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7329fb4e2005b339f3a7baa0f87ce8cc4318f714
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107733"
---
# <a name="list-contacts"></a><span data-ttu-id="40dee-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="40dee-103">List contacts</span></span>

<span data-ttu-id="40dee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40dee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40dee-105">Получение контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="40dee-105">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="40dee-106">Существует два сценария, с помощью которых приложение может получить контакты из папки контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="40dee-106">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="40dee-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="40dee-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="40dee-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="40dee-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="40dee-109">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="40dee-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="40dee-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40dee-110">Permissions</span></span>
<span data-ttu-id="40dee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40dee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40dee-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40dee-113">Permission type</span></span>      | <span data-ttu-id="40dee-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40dee-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40dee-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40dee-115">Delegated (work or school account)</span></span> | <span data-ttu-id="40dee-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40dee-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="40dee-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40dee-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40dee-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40dee-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="40dee-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40dee-119">Application</span></span> | <span data-ttu-id="40dee-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40dee-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="40dee-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40dee-121">HTTP request</span></span>

<span data-ttu-id="40dee-122">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="40dee-122">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="40dee-123">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="40dee-123">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40dee-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40dee-124">Optional query parameters</span></span>
<span data-ttu-id="40dee-125">С помощью параметра запроса `$filter` можно фильтровать контакты на основе адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="40dee-125">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="40dee-126">Обратите внимание, что вы можете использовать оператор `$filter`, `any`, и `eq` только для дочернего свойства **address** для экземпляров коллекции **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="40dee-126">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="40dee-127">Т.е. вы не можете выполнять фильтрацию с помощью дочернего свойства **name** или другого дочернего свойства экземпляра **emailAddresses**, как и не можете применять другие операторы или функции с `filter`, такие как `ne`, `le` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="40dee-127">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="40dee-128">Общие сведения о параметре запроса `$filter` см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="40dee-128">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="40dee-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40dee-129">Request headers</span></span>
| <span data-ttu-id="40dee-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40dee-130">Header</span></span>       | <span data-ttu-id="40dee-131">Значение</span><span class="sxs-lookup"><span data-stu-id="40dee-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40dee-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40dee-132">Authorization</span></span>  | <span data-ttu-id="40dee-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40dee-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40dee-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40dee-135">Request body</span></span>
<span data-ttu-id="40dee-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40dee-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40dee-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="40dee-137">Response</span></span>

<span data-ttu-id="40dee-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40dee-138">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40dee-139">Пример</span><span class="sxs-lookup"><span data-stu-id="40dee-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40dee-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="40dee-140">Request</span></span>
<span data-ttu-id="40dee-141">В следующем примере возвращаются свойства **DisplayName** и **EmailAddresses** для контактов вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="40dee-141">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>

# <a name="http"></a>[<span data-ttu-id="40dee-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="40dee-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```
# <a name="c"></a>[<span data-ttu-id="40dee-143">C#</span><span class="sxs-lookup"><span data-stu-id="40dee-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40dee-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40dee-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40dee-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40dee-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="40dee-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="40dee-146">Response</span></span>
<span data-ttu-id="40dee-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40dee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
