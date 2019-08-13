---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a216f6392356cb2f3219ccb61103edbd65f269b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346382"
---
# <a name="create-contact"></a><span data-ttu-id="1b2c0-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="1b2c0-103">Create Contact</span></span>

<span data-ttu-id="1b2c0-104">Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b2c0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b2c0-105">Permissions</span></span>
<span data-ttu-id="1b2c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b2c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b2c0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b2c0-108">Permission type</span></span>      | <span data-ttu-id="1b2c0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b2c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b2c0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b2c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b2c0-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b2c0-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b2c0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b2c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b2c0-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b2c0-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b2c0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b2c0-114">Application</span></span> | <span data-ttu-id="1b2c0-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b2c0-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b2c0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b2c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="1b2c0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b2c0-117">Request headers</span></span>
| <span data-ttu-id="1b2c0-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b2c0-118">Header</span></span>       | <span data-ttu-id="1b2c0-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1b2c0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b2c0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b2c0-120">Authorization</span></span>  | <span data-ttu-id="1b2c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b2c0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b2c0-123">Content-Type</span></span>  | <span data-ttu-id="1b2c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b2c0-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b2c0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b2c0-125">Request body</span></span>
<span data-ttu-id="1b2c0-126">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b2c0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b2c0-127">Response</span></span>

<span data-ttu-id="1b2c0-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-128">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b2c0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1b2c0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b2c0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b2c0-130">Request</span></span>
<span data-ttu-id="1b2c0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b2c0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b2c0-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b2c0-133">C#</span><span class="sxs-lookup"><span data-stu-id="1b2c0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b2c0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b2c0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b2c0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b2c0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b2c0-136">Java</span><span class="sxs-lookup"><span data-stu-id="1b2c0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1b2c0-137">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-137">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="1b2c0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b2c0-138">Response</span></span>
<span data-ttu-id="1b2c0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b2c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
