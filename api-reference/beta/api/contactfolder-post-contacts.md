---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e36ad905d07b76ba3ba7010438305b0a7b1d2e2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863174"
---
# <a name="create-contact"></a><span data-ttu-id="558b5-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="558b5-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="558b5-104">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="558b5-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="558b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="558b5-105">Permissions</span></span>
<span data-ttu-id="558b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="558b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="558b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="558b5-108">Permission type</span></span>      | <span data-ttu-id="558b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="558b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="558b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="558b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="558b5-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="558b5-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="558b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="558b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="558b5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="558b5-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="558b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="558b5-114">Application</span></span> | <span data-ttu-id="558b5-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="558b5-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="558b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="558b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="558b5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="558b5-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="558b5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="558b5-118">Request headers</span></span>
| <span data-ttu-id="558b5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="558b5-119">Header</span></span>       | <span data-ttu-id="558b5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="558b5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="558b5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="558b5-121">Authorization</span></span>  | <span data-ttu-id="558b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="558b5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="558b5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="558b5-124">Content-Type</span></span>  | <span data-ttu-id="558b5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="558b5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="558b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="558b5-127">Request body</span></span>
<span data-ttu-id="558b5-128">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="558b5-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="558b5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="558b5-129">Response</span></span>

<span data-ttu-id="558b5-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="558b5-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="558b5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="558b5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="558b5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="558b5-132">Request</span></span>
<span data-ttu-id="558b5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="558b5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="558b5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="558b5-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="558b5-135">C#</span><span class="sxs-lookup"><span data-stu-id="558b5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="558b5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="558b5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="558b5-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="558b5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="558b5-138">Java</span><span class="sxs-lookup"><span data-stu-id="558b5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="558b5-139">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="558b5-139">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="558b5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="558b5-140">Response</span></span>
<span data-ttu-id="558b5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="558b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
