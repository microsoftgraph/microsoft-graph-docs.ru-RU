---
title: Список контактов
description: Получение коллекции контактов из папки контактов по умолчанию для выполнившего вход пользователя.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1d5d12fc90bd713ec4df1f96d69a9bf0c74e880b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050222"
---
# <a name="list-contacts"></a><span data-ttu-id="b4ab7-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="b4ab7-103">List contacts</span></span>

<span data-ttu-id="b4ab7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4ab7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4ab7-105">Получение коллекции контактов из папки контактов по умолчанию для выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-105">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="b4ab7-106">Существует два сценария, с помощью которых приложение может получить контакты из папки контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="b4ab7-106">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="b4ab7-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="b4ab7-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b4ab7-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b4ab7-109">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="b4ab7-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="b4ab7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ab7-110">Permissions</span></span>
<span data-ttu-id="b4ab7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ab7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ab7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ab7-113">Permission type</span></span>      | <span data-ttu-id="b4ab7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4ab7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ab7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4ab7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ab7-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ab7-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b4ab7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4ab7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ab7-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ab7-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b4ab7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4ab7-119">Application</span></span> | <span data-ttu-id="b4ab7-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ab7-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ab7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4ab7-121">HTTP request</span></span>

<span data-ttu-id="b4ab7-122">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="b4ab7-122">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="b4ab7-123">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="b4ab7-123">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolders/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4ab7-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4ab7-124">Optional query parameters</span></span>
<span data-ttu-id="b4ab7-125">С помощью параметра запроса `$filter` можно фильтровать контакты на основе адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="b4ab7-125">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="b4ab7-126">Обратите внимание, что вы можете использовать оператор `$filter`, `any`, и `eq` только для дочернего свойства **address** для экземпляров коллекции **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-126">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="b4ab7-127">Т.е. вы не можете выполнять фильтрацию с помощью дочернего свойства **name** или другого дочернего свойства экземпляра **emailAddresses**, как и не можете применять другие операторы или функции с `filter`, такие как `ne`, `le` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-127">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="b4ab7-128">Общие сведения о параметре запроса `$filter` см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b4ab7-128">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="b4ab7-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4ab7-129">Request headers</span></span>
| <span data-ttu-id="b4ab7-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4ab7-130">Header</span></span>       | <span data-ttu-id="b4ab7-131">Значение</span><span class="sxs-lookup"><span data-stu-id="b4ab7-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4ab7-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4ab7-132">Authorization</span></span>  | <span data-ttu-id="b4ab7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b4ab7-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4ab7-135">Content-Type</span></span>   | <span data-ttu-id="b4ab7-136">application/json</span><span class="sxs-lookup"><span data-stu-id="b4ab7-136">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4ab7-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4ab7-137">Request body</span></span>
<span data-ttu-id="b4ab7-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4ab7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ab7-139">Response</span></span>

<span data-ttu-id="b4ab7-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-140">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4ab7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b4ab7-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4ab7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4ab7-142">Request</span></span>
<span data-ttu-id="b4ab7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4ab7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ab7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="c"></a>[<span data-ttu-id="b4ab7-145">C#</span><span class="sxs-lookup"><span data-stu-id="b4ab7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4ab7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ab7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4ab7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4ab7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4ab7-148">Java</span><span class="sxs-lookup"><span data-stu-id="b4ab7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="b4ab7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ab7-149">Response</span></span>
<span data-ttu-id="b4ab7-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-150">Here is an example of the response.</span></span> <span data-ttu-id="b4ab7-151">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4ab7-151">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

