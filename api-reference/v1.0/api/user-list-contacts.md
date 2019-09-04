---
title: Список контактов
description: Получение коллекции контактов из папки контактов по умолчанию для выполнившего вход пользователя.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b8defe631b70e42cd7613eb0ab0e46b144ec76b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729065"
---
# <a name="list-contacts"></a><span data-ttu-id="09158-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="09158-103">List contacts</span></span>

<span data-ttu-id="09158-104">Получение коллекции контактов из папки контактов по умолчанию для выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="09158-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="09158-105">Существует два сценария, с помощью которых приложение может получить контакты из папки контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="09158-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="09158-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="09158-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="09158-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="09158-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="09158-108">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="09158-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="09158-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09158-109">Permissions</span></span>
<span data-ttu-id="09158-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09158-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09158-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09158-112">Permission type</span></span>      | <span data-ttu-id="09158-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09158-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09158-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09158-114">Delegated (work or school account)</span></span> | <span data-ttu-id="09158-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09158-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="09158-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09158-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09158-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09158-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="09158-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09158-118">Application</span></span> | <span data-ttu-id="09158-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09158-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="09158-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09158-120">HTTP request</span></span>

<span data-ttu-id="09158-121">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="09158-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="09158-122">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="09158-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09158-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="09158-123">Optional query parameters</span></span>
<span data-ttu-id="09158-124">С помощью параметра запроса `$filter` можно фильтровать контакты на основе адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="09158-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="09158-125">Обратите внимание, что вы можете использовать оператор `$filter`, `any`, и `eq` только для дочернего свойства **address** для экземпляров коллекции **emailAddresses**.</span><span class="sxs-lookup"><span data-stu-id="09158-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="09158-126">Т.е. вы не можете выполнять фильтрацию с помощью дочернего свойства **name** или другого дочернего свойства экземпляра **emailAddresses**, как и не можете применять другие операторы или функции с `filter`, такие как `ne`, `le` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="09158-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="09158-127">Общие сведения о параметре запроса `$filter` см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="09158-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="09158-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09158-128">Request headers</span></span>
| <span data-ttu-id="09158-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09158-129">Header</span></span>       | <span data-ttu-id="09158-130">Значение</span><span class="sxs-lookup"><span data-stu-id="09158-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09158-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09158-131">Authorization</span></span>  | <span data-ttu-id="09158-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09158-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09158-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09158-134">Content-Type</span></span>   | <span data-ttu-id="09158-135">application/json</span><span class="sxs-lookup"><span data-stu-id="09158-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09158-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09158-136">Request body</span></span>
<span data-ttu-id="09158-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09158-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09158-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="09158-138">Response</span></span>

<span data-ttu-id="09158-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09158-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09158-140">Пример</span><span class="sxs-lookup"><span data-stu-id="09158-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09158-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="09158-141">Request</span></span>
<span data-ttu-id="09158-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09158-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="09158-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="09158-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09158-144">C#</span><span class="sxs-lookup"><span data-stu-id="09158-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09158-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09158-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09158-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09158-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="09158-147">Java</span><span class="sxs-lookup"><span data-stu-id="09158-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="09158-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="09158-148">Response</span></span>
<span data-ttu-id="09158-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09158-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
