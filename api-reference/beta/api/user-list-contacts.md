---
title: Список контактов
description: Получение контактов в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a1eaeac682f511bf9b895e06e6a19b3bc728a38c
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026012"
---
# <a name="list-contacts"></a><span data-ttu-id="a9d82-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="a9d82-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9d82-104">Получение контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a9d82-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="a9d82-105">Существует два сценария, в которых приложение может получать контакты в папке контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="a9d82-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="a9d82-106">если у приложения есть разрешения для приложений;</span><span class="sxs-lookup"><span data-stu-id="a9d82-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a9d82-107">Если приложение имеет соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь предоставил доступ к папке контактов для этого пользователя или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="a9d82-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a9d82-108">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="a9d82-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="a9d82-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9d82-109">Permissions</span></span>
<span data-ttu-id="a9d82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9d82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9d82-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9d82-112">Permission type</span></span>      | <span data-ttu-id="a9d82-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9d82-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9d82-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9d82-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a9d82-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9d82-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a9d82-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9d82-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9d82-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9d82-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a9d82-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9d82-118">Application</span></span> | <span data-ttu-id="a9d82-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9d82-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9d82-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9d82-120">HTTP request</span></span>

<span data-ttu-id="a9d82-121">Для получения всех контактов в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="a9d82-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="a9d82-122">Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="a9d82-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9d82-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9d82-123">Optional query parameters</span></span>
<span data-ttu-id="a9d82-124">С помощью параметра `$filter` запроса можно фильтровать контакты на основе их адресов электронной почты:</span><span class="sxs-lookup"><span data-stu-id="a9d82-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="a9d82-125">Обратите внимание, что `$filter`вы `any`можете использовать, `eq` и оператор, только для вложенного свойства **Address** экземпляров в коллекции **EmailAddresses** .</span><span class="sxs-lookup"><span data-stu-id="a9d82-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="a9d82-126">То есть невозможно выполнить фильтрацию по **имени** или другому подсвойству экземпляра **EmailAddresses**, а также к любому другому оператору или функции с `filter`помощью, например `ne`, `le`, и. `startswith()`</span><span class="sxs-lookup"><span data-stu-id="a9d82-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="a9d82-127">Общие сведения о параметре `$filter` запроса можно узнать в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9d82-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9d82-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9d82-128">Request headers</span></span>
| <span data-ttu-id="a9d82-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9d82-129">Header</span></span>       | <span data-ttu-id="a9d82-130">Значение</span><span class="sxs-lookup"><span data-stu-id="a9d82-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9d82-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9d82-131">Authorization</span></span>  | <span data-ttu-id="a9d82-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9d82-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9d82-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9d82-134">Request body</span></span>
<span data-ttu-id="a9d82-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9d82-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9d82-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9d82-136">Response</span></span>

<span data-ttu-id="a9d82-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9d82-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9d82-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a9d82-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9d82-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9d82-139">Request</span></span>
<span data-ttu-id="a9d82-140">В следующем примере возвращаются свойства **DisplayName** и **EmailAddresses** для контактов вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="a9d82-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="a9d82-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9d82-141">Response</span></span>
<span data-ttu-id="a9d82-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9d82-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
