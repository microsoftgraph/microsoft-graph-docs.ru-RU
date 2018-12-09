---
title: Список контактов
description: Получение контактов в почтовом ящике пользователя.
ms.openlocfilehash: 649adacf88b13e080ae02ca67986b448f3426cac
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209742"
---
# <a name="list-contacts"></a><span data-ttu-id="ab2e8-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="ab2e8-103">List contacts</span></span>

> <span data-ttu-id="ab2e8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab2e8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab2e8-106">Получение контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-106">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="ab2e8-107">Существует два сценария, где приложения можно получить контактов в папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-107">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="ab2e8-108">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="ab2e8-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ab2e8-109">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ab2e8-110">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="ab2e8-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="ab2e8-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab2e8-111">Permissions</span></span>
<span data-ttu-id="ab2e8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab2e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab2e8-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab2e8-114">Permission type</span></span>      | <span data-ttu-id="ab2e8-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab2e8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab2e8-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab2e8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ab2e8-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab2e8-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ab2e8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab2e8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab2e8-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab2e8-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ab2e8-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab2e8-120">Application</span></span> | <span data-ttu-id="ab2e8-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab2e8-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab2e8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab2e8-122">HTTP request</span></span>

<span data-ttu-id="ab2e8-123">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="ab2e8-123">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="ab2e8-124">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="ab2e8-124">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab2e8-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab2e8-125">Optional query parameters</span></span>
<span data-ttu-id="ab2e8-126">Можно использовать `$filter` параметр запроса Фильтрация контактов на основании их адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="ab2e8-126">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="ab2e8-127">Обратите внимание, что можно использовать `$filter`, `any`и `eq` оператора только **адреса** подчиненных свойств экземпляров в коллекции **emailAddresses** .</span><span class="sxs-lookup"><span data-stu-id="ab2e8-127">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="ab2e8-128">То есть, не может фильтровать по **имени** или других подчиненных свойств экземпляра **emailAddresses**, а также можно применить любой другой оператор или функцию с `filter`, таких как `ne`, `le`, и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-128">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="ab2e8-129">Общие сведения о `$filter` параметр запроса, просмотрите [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab2e8-129">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab2e8-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab2e8-130">Request headers</span></span>
| <span data-ttu-id="ab2e8-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab2e8-131">Header</span></span>       | <span data-ttu-id="ab2e8-132">Значение</span><span class="sxs-lookup"><span data-stu-id="ab2e8-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab2e8-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab2e8-133">Authorization</span></span>  | <span data-ttu-id="ab2e8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab2e8-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab2e8-136">Request body</span></span>
<span data-ttu-id="ab2e8-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab2e8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab2e8-138">Response</span></span>

<span data-ttu-id="ab2e8-139">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [контактов](../resources/contact.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-139">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab2e8-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ab2e8-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab2e8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab2e8-141">Request</span></span>
<span data-ttu-id="ab2e8-142">Следующий пример возвращает свойства **displayName** и **emailAddresses** контактов пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-142">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="ab2e8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab2e8-143">Response</span></span>
<span data-ttu-id="ab2e8-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab2e8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
