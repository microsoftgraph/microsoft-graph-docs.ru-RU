---
title: Список контактов
description: Получите коллекцию контактов из папки контактов по умолчанию пользователя, выполнившего вход.
author: dkershaw10
ms.openlocfilehash: a4fa40b66280ea3447c1d07a531a596a42c14ed2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307499"
---
# <a name="list-contacts"></a><span data-ttu-id="4ba89-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="4ba89-103">List contacts</span></span>

<span data-ttu-id="4ba89-104">Получите коллекцию контактов из папки контактов по умолчанию пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="4ba89-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="4ba89-105">Существует два сценария, где приложения можно получить контактов в папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ba89-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="4ba89-106">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="4ba89-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="4ba89-107">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="4ba89-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="4ba89-108">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="4ba89-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="4ba89-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ba89-109">Permissions</span></span>
<span data-ttu-id="4ba89-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba89-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ba89-112">Permission type</span></span>      | <span data-ttu-id="4ba89-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ba89-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba89-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ba89-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba89-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ba89-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4ba89-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ba89-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba89-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ba89-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4ba89-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ba89-118">Application</span></span> | <span data-ttu-id="4ba89-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ba89-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba89-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ba89-120">HTTP request</span></span>

<span data-ttu-id="4ba89-121">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="4ba89-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="4ba89-122">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="4ba89-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ba89-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ba89-123">Optional query parameters</span></span>
<span data-ttu-id="4ba89-124">Можно использовать `$filter` параметр запроса Фильтрация контактов на основании их адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="4ba89-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="4ba89-125">Обратите внимание, что можно использовать `$filter`, `any`и `eq` оператора только **адреса** подчиненных свойств экземпляров в коллекции **emailAddresses** .</span><span class="sxs-lookup"><span data-stu-id="4ba89-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="4ba89-126">То есть, не может фильтровать по **имени** или других подчиненных свойств экземпляра **emailAddresses**, а также можно применить любой другой оператор или функцию с `filter`, таких как `ne`, `le`, и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="4ba89-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="4ba89-127">Общие сведения о `$filter` параметр запроса, просмотрите [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ba89-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="4ba89-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ba89-128">Request headers</span></span>
| <span data-ttu-id="4ba89-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ba89-129">Header</span></span>       | <span data-ttu-id="4ba89-130">Значение</span><span class="sxs-lookup"><span data-stu-id="4ba89-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ba89-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ba89-131">Authorization</span></span>  | <span data-ttu-id="4ba89-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ba89-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ba89-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ba89-134">Content-Type</span></span>   | <span data-ttu-id="4ba89-135">application/json</span><span class="sxs-lookup"><span data-stu-id="4ba89-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ba89-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ba89-136">Request body</span></span>
<span data-ttu-id="4ba89-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ba89-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba89-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ba89-138">Response</span></span>

<span data-ttu-id="4ba89-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ba89-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ba89-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4ba89-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ba89-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ba89-141">Request</span></span>
<span data-ttu-id="4ba89-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ba89-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="4ba89-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ba89-143">Response</span></span>
<span data-ttu-id="4ba89-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4ba89-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
