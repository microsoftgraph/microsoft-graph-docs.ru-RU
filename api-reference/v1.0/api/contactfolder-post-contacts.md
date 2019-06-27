---
title: Создание контакта
description: Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 213d60a3dacb976d1bcc06509982ffe5a38a6359
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273894"
---
# <a name="create-contact"></a><span data-ttu-id="875aa-103">Создание контакта</span><span class="sxs-lookup"><span data-stu-id="875aa-103">Create contact</span></span>

<span data-ttu-id="875aa-104">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="875aa-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="875aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="875aa-105">Permissions</span></span>

<span data-ttu-id="875aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="875aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="875aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="875aa-108">Permission type</span></span>      | <span data-ttu-id="875aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="875aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="875aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="875aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="875aa-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="875aa-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="875aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="875aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="875aa-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="875aa-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="875aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="875aa-114">Application</span></span> | <span data-ttu-id="875aa-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="875aa-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="875aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="875aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="875aa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="875aa-117">Request headers</span></span>

| <span data-ttu-id="875aa-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="875aa-118">Header</span></span>       | <span data-ttu-id="875aa-119">Значение</span><span class="sxs-lookup"><span data-stu-id="875aa-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="875aa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="875aa-120">Authorization</span></span>  | <span data-ttu-id="875aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="875aa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="875aa-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="875aa-123">Content-Type</span></span>  | <span data-ttu-id="875aa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="875aa-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="875aa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="875aa-126">Request body</span></span>
<span data-ttu-id="875aa-127">В теле запроса представьте объект [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="875aa-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="875aa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="875aa-128">Response</span></span>

<span data-ttu-id="875aa-129">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="875aa-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="875aa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="875aa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="875aa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="875aa-131">Request</span></span>

<span data-ttu-id="875aa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="875aa-132">Here is an example of the request.</span></span>

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

<br/>

<span data-ttu-id="875aa-133">В теле запроса представьте объект [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="875aa-133">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="875aa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="875aa-134">Response</span></span>

<span data-ttu-id="875aa-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="875aa-135">Here is an example of the response.</span></span> <span data-ttu-id="875aa-136">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="875aa-136">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="875aa-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="875aa-137">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="875aa-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="875aa-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="875aa-139">C#</span><span class="sxs-lookup"><span data-stu-id="875aa-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="875aa-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="875aa-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="875aa-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="875aa-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contact_from_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/v1.0/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contactfolder-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
