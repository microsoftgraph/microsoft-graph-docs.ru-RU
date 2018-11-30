---
title: Список контактов
description: Получение контактов в почтовом ящике пользователя.
ms.openlocfilehash: 2554836607705138702e5b04a60cf4a77a8e53f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075399"
---
# <a name="list-contacts"></a><span data-ttu-id="7655b-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="7655b-103">List contacts</span></span>

> <span data-ttu-id="7655b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7655b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7655b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7655b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7655b-106">Получение контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="7655b-106">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="7655b-107">Существует два сценария, где приложения можно получить контактов в папке контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7655b-107">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="7655b-108">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="7655b-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7655b-109">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя, и другой пользователь общей папке контактов с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="7655b-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7655b-110">В разделе [сведения и примеры](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="7655b-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="7655b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7655b-111">Permissions</span></span>
<span data-ttu-id="7655b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7655b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7655b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7655b-114">Permission type</span></span>      | <span data-ttu-id="7655b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7655b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7655b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7655b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7655b-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7655b-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7655b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7655b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7655b-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7655b-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7655b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7655b-120">Application</span></span> | <span data-ttu-id="7655b-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7655b-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7655b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7655b-122">HTTP request</span></span>

<span data-ttu-id="7655b-123">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="7655b-123">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="7655b-124">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="7655b-124">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7655b-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7655b-125">Optional query parameters</span></span>
<span data-ttu-id="7655b-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7655b-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7655b-127">Например, с помощью параметра запроса `$filter` можно фильтровать контакты на основе домена, указанного в адресе электронной почты:</span><span class="sxs-lookup"><span data-stu-id="7655b-127">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`

## <a name="request-headers"></a><span data-ttu-id="7655b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7655b-128">Request headers</span></span>
| <span data-ttu-id="7655b-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7655b-129">Header</span></span>       | <span data-ttu-id="7655b-130">Значение</span><span class="sxs-lookup"><span data-stu-id="7655b-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7655b-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7655b-131">Authorization</span></span>  | <span data-ttu-id="7655b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7655b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7655b-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7655b-134">Request body</span></span>
<span data-ttu-id="7655b-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7655b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7655b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7655b-136">Response</span></span>

<span data-ttu-id="7655b-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [контактов](../resources/contact.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7655b-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7655b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7655b-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7655b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7655b-139">Request</span></span>
<span data-ttu-id="7655b-140">Следующий пример возвращает свойства **displayName** и **emailAddresses** контактов пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="7655b-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="7655b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="7655b-141">Response</span></span>
<span data-ttu-id="7655b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7655b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
