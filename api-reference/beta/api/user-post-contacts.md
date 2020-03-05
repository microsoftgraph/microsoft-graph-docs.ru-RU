---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d86f100f3343ffba2b3302927129bdd7a575329
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451710"
---
# <a name="create-contact"></a><span data-ttu-id="3f3d6-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="3f3d6-103">Create Contact</span></span>

<span data-ttu-id="3f3d6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f3d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f3d6-105">Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f3d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f3d6-106">Permissions</span></span>
<span data-ttu-id="3f3d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f3d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f3d6-109">Permission type</span></span>      | <span data-ttu-id="3f3d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f3d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f3d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f3d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f3d6-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f3d6-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3f3d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f3d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f3d6-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f3d6-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3f3d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f3d6-115">Application</span></span> | <span data-ttu-id="3f3d6-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f3d6-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f3d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f3d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="3f3d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f3d6-118">Request headers</span></span>
| <span data-ttu-id="3f3d6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f3d6-119">Header</span></span>       | <span data-ttu-id="3f3d6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3f3d6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f3d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f3d6-121">Authorization</span></span>  | <span data-ttu-id="3f3d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3f3d6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f3d6-124">Content-Type</span></span>  | <span data-ttu-id="3f3d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f3d6-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f3d6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f3d6-126">Request body</span></span>
<span data-ttu-id="3f3d6-127">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-127">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3f3d6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f3d6-128">Response</span></span>

<span data-ttu-id="3f3d6-129">В случае успеха этот метод возвращает `201 Created` код отклика и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-129">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f3d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3f3d6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f3d6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f3d6-131">Request</span></span>
<span data-ttu-id="3f3d6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f3d6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f3d6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@contoso.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "personal"
    },
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "other",
      "otherLabel": "Volunteer work"
    }
  ],
  "phones" : [
    {
      "number": "+1 732 555 0102",
      "type": "business"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="3f3d6-134">C#</span><span class="sxs-lookup"><span data-stu-id="3f3d6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f3d6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f3d6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f3d6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f3d6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3f3d6-137">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-137">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3f3d6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f3d6-138">Response</span></span>
<span data-ttu-id="3f3d6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f3d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T19:56:07Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
            "otherLabel": "Volunteer work",
            "type":"other",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="3f3d6-142">См. также</span><span class="sxs-lookup"><span data-stu-id="3f3d6-142">See also</span></span>

- [<span data-ttu-id="3f3d6-143">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="3f3d6-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3f3d6-144">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3f3d6-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
