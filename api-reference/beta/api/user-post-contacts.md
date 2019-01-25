---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dbac25f4cf86074876fd1be4f0632a5afdb08dc1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520167"
---
# <a name="create-contact"></a><span data-ttu-id="7c256-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="7c256-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c256-104">Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="7c256-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c256-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c256-105">Permissions</span></span>
<span data-ttu-id="7c256-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c256-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c256-108">Permission type</span></span>      | <span data-ttu-id="7c256-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c256-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c256-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c256-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c256-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c256-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7c256-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c256-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c256-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c256-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7c256-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c256-114">Application</span></span> | <span data-ttu-id="7c256-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c256-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c256-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c256-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="7c256-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c256-117">Request headers</span></span>
| <span data-ttu-id="7c256-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c256-118">Header</span></span>       | <span data-ttu-id="7c256-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7c256-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c256-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c256-120">Authorization</span></span>  | <span data-ttu-id="7c256-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c256-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7c256-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c256-123">Content-Type</span></span>  | <span data-ttu-id="7c256-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c256-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c256-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c256-125">Request body</span></span>
<span data-ttu-id="7c256-126">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c256-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7c256-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c256-127">Response</span></span>

<span data-ttu-id="7c256-128">Успешно завершена, этот метод возвращает `201 Created` объект [пользователя](../resources/contact.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7c256-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c256-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7c256-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c256-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c256-130">Request</span></span>
<span data-ttu-id="7c256-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c256-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="7c256-132">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c256-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="7c256-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c256-133">Response</span></span>
<span data-ttu-id="7c256-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7c256-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7c256-137">См. также</span><span class="sxs-lookup"><span data-stu-id="7c256-137">See also</span></span>

- [<span data-ttu-id="7c256-138">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7c256-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7c256-139">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7c256-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
