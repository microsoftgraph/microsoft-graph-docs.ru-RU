---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 318f72b56c057c13cb4e3a96a969a164f97b3007
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031501"
---
# <a name="create-contact"></a><span data-ttu-id="926f8-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="926f8-103">Create Contact</span></span>

<span data-ttu-id="926f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="926f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="926f8-105">Добавление контакта в корневую папку с контактами или конечную точку contacts другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="926f8-105">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="926f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="926f8-106">Permissions</span></span>
<span data-ttu-id="926f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="926f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="926f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="926f8-109">Permission type</span></span>      | <span data-ttu-id="926f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="926f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="926f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="926f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="926f8-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="926f8-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="926f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="926f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="926f8-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="926f8-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="926f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="926f8-115">Application</span></span> | <span data-ttu-id="926f8-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="926f8-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="926f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="926f8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="926f8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="926f8-118">Request headers</span></span>
| <span data-ttu-id="926f8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="926f8-119">Header</span></span>       | <span data-ttu-id="926f8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="926f8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="926f8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="926f8-121">Authorization</span></span>  | <span data-ttu-id="926f8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="926f8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="926f8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="926f8-124">Content-Type</span></span>  | <span data-ttu-id="926f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="926f8-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="926f8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="926f8-126">Request body</span></span>
<span data-ttu-id="926f8-127">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="926f8-127">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="926f8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="926f8-128">Response</span></span>

<span data-ttu-id="926f8-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="926f8-129">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="926f8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="926f8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="926f8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="926f8-131">Request</span></span>
<span data-ttu-id="926f8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="926f8-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="926f8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="926f8-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="926f8-134">C#</span><span class="sxs-lookup"><span data-stu-id="926f8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="926f8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="926f8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="926f8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="926f8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="926f8-137">Java</span><span class="sxs-lookup"><span data-stu-id="926f8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="926f8-138">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="926f8-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="926f8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="926f8-139">Response</span></span>
<span data-ttu-id="926f8-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="926f8-140">Here is an example of the response.</span></span> <span data-ttu-id="926f8-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="926f8-141">Note: The response object shown here might be shortened for readability.</span></span>
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

