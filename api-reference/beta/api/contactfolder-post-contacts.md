---
title: Создание объекта Contact
description: Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 31c3875354644be14f8902e524f586a86dd99735
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436813"
---
# <a name="create-contact"></a><span data-ttu-id="ffcf5-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="ffcf5-103">Create Contact</span></span>

<span data-ttu-id="ffcf5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ffcf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffcf5-105">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-105">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffcf5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffcf5-106">Permissions</span></span>
<span data-ttu-id="ffcf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffcf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffcf5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffcf5-109">Permission type</span></span>      | <span data-ttu-id="ffcf5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffcf5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffcf5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffcf5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ffcf5-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffcf5-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ffcf5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffcf5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffcf5-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffcf5-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ffcf5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffcf5-115">Application</span></span> | <span data-ttu-id="ffcf5-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffcf5-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffcf5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffcf5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="ffcf5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffcf5-118">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffcf5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffcf5-119">Request headers</span></span>
| <span data-ttu-id="ffcf5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffcf5-120">Header</span></span>       | <span data-ttu-id="ffcf5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ffcf5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffcf5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffcf5-122">Authorization</span></span>  | <span data-ttu-id="ffcf5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ffcf5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ffcf5-125">Content-Type</span></span>  | <span data-ttu-id="ffcf5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ffcf5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffcf5-128">Request body</span></span>
<span data-ttu-id="ffcf5-129">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-129">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ffcf5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffcf5-130">Response</span></span>

<span data-ttu-id="ffcf5-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-131">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffcf5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ffcf5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffcf5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffcf5-133">Request</span></span>
<span data-ttu-id="ffcf5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ffcf5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffcf5-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ffcf5-136">C#</span><span class="sxs-lookup"><span data-stu-id="ffcf5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffcf5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffcf5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffcf5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffcf5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ffcf5-139">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-139">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ffcf5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffcf5-140">Response</span></span>
<span data-ttu-id="ffcf5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffcf5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
