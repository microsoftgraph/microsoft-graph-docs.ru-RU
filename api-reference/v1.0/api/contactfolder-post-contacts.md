---
title: Создание контакта
description: Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cf20b2b9388dea809214e5978737c098892812b0
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061870"
---
# <a name="create-contact"></a><span data-ttu-id="0d3e8-103">Создание контакта</span><span class="sxs-lookup"><span data-stu-id="0d3e8-103">Create contact</span></span>

<span data-ttu-id="0d3e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d3e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d3e8-105">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d3e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d3e8-106">Permissions</span></span>

<span data-ttu-id="0d3e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d3e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d3e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d3e8-109">Permission type</span></span>      | <span data-ttu-id="0d3e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d3e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d3e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d3e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d3e8-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d3e8-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d3e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d3e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d3e8-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d3e8-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d3e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d3e8-115">Application</span></span> | <span data-ttu-id="0d3e8-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d3e8-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d3e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d3e8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="0d3e8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d3e8-118">Request headers</span></span>

| <span data-ttu-id="0d3e8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d3e8-119">Header</span></span>       | <span data-ttu-id="0d3e8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0d3e8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d3e8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d3e8-121">Authorization</span></span>  | <span data-ttu-id="0d3e8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d3e8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d3e8-124">Content-Type</span></span>  | <span data-ttu-id="0d3e8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d3e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d3e8-127">Request body</span></span>
<span data-ttu-id="0d3e8-128">В теле запроса представьте объект [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-128">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0d3e8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d3e8-129">Response</span></span>

<span data-ttu-id="0d3e8-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-130">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d3e8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0d3e8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d3e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d3e8-132">Request</span></span>

<span data-ttu-id="0d3e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d3e8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d3e8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="c"></a>[<span data-ttu-id="0d3e8-135">C#</span><span class="sxs-lookup"><span data-stu-id="0d3e8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d3e8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d3e8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d3e8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d3e8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d3e8-138">Java</span><span class="sxs-lookup"><span data-stu-id="0d3e8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="0d3e8-139">В теле запроса представьте объект [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-139">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="0d3e8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d3e8-140">Response</span></span>

<span data-ttu-id="0d3e8-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="0d3e8-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0d3e8-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

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

