---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 7f412310bac1f8767fdb62857d050ebcdc236fc5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846986"
---
# <a name="create-contact"></a><span data-ttu-id="99c09-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="99c09-103">Create Contact</span></span>

> <span data-ttu-id="99c09-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99c09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99c09-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99c09-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99c09-106">Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="99c09-106">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="99c09-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99c09-107">Permissions</span></span>
<span data-ttu-id="99c09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99c09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c09-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99c09-110">Permission type</span></span>      | <span data-ttu-id="99c09-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99c09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99c09-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99c09-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99c09-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99c09-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="99c09-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99c09-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99c09-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99c09-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="99c09-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99c09-116">Application</span></span> | <span data-ttu-id="99c09-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99c09-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99c09-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99c09-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="99c09-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99c09-119">Request headers</span></span>
| <span data-ttu-id="99c09-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99c09-120">Header</span></span>       | <span data-ttu-id="99c09-121">Значение</span><span class="sxs-lookup"><span data-stu-id="99c09-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99c09-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99c09-122">Authorization</span></span>  | <span data-ttu-id="99c09-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99c09-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="99c09-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99c09-125">Content-Type</span></span>  | <span data-ttu-id="99c09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99c09-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99c09-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99c09-127">Request body</span></span>
<span data-ttu-id="99c09-128">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99c09-128">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="99c09-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="99c09-129">Response</span></span>

<span data-ttu-id="99c09-130">Успешно завершена, этот метод возвращает `201 Created` объект [пользователя](../resources/contact.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="99c09-130">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c09-131">Пример</span><span class="sxs-lookup"><span data-stu-id="99c09-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99c09-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="99c09-132">Request</span></span>
<span data-ttu-id="99c09-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99c09-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="99c09-134">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99c09-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="99c09-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="99c09-135">Response</span></span>
<span data-ttu-id="99c09-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="99c09-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="99c09-139">См. также</span><span class="sxs-lookup"><span data-stu-id="99c09-139">See also</span></span>

- [<span data-ttu-id="99c09-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="99c09-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="99c09-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="99c09-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
