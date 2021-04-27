---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 27e765335b2ae9c4e81668adfb090746773b4282
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047072"
---
# <a name="create-contact"></a><span data-ttu-id="7dde4-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="7dde4-103">Create Contact</span></span>

<span data-ttu-id="7dde4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dde4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dde4-105">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="7dde4-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7dde4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dde4-106">Permissions</span></span>
<span data-ttu-id="7dde4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dde4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dde4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dde4-109">Permission type</span></span>      | <span data-ttu-id="7dde4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dde4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dde4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dde4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dde4-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dde4-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7dde4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dde4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dde4-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dde4-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7dde4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dde4-115">Application</span></span> | <span data-ttu-id="7dde4-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dde4-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dde4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dde4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="7dde4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dde4-118">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="7dde4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dde4-119">Request headers</span></span>
| <span data-ttu-id="7dde4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dde4-120">Header</span></span>       | <span data-ttu-id="7dde4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7dde4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7dde4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dde4-122">Authorization</span></span>  | <span data-ttu-id="7dde4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dde4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7dde4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7dde4-125">Content-Type</span></span>  | <span data-ttu-id="7dde4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dde4-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7dde4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7dde4-128">Request body</span></span>
<span data-ttu-id="7dde4-129">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dde4-129">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7dde4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dde4-130">Response</span></span>

<span data-ttu-id="7dde4-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7dde4-131">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dde4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7dde4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7dde4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dde4-133">Request</span></span>
<span data-ttu-id="7dde4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dde4-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dde4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dde4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7dde4-136">C#</span><span class="sxs-lookup"><span data-stu-id="7dde4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dde4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dde4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dde4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dde4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dde4-139">Java</span><span class="sxs-lookup"><span data-stu-id="7dde4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7dde4-140">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dde4-140">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7dde4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dde4-141">Response</span></span>
<span data-ttu-id="7dde4-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dde4-142">Here is an example of the response.</span></span> <span data-ttu-id="7dde4-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7dde4-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

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


