---
title: Получение объекта contactFolder
description: Получение папки контактов с помощью ее идентификатора.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5de49776c57789e04dd40723c4eb4f20ac03661
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417972"
---
# <a name="get-contactfolder"></a><span data-ttu-id="6a4e5-103">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="6a4e5-103">Get contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a4e5-104">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="6a4e5-105">Существует два сценария, в которых приложение может получить папку контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="6a4e5-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="6a4e5-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="6a4e5-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6a4e5-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6a4e5-108">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="6a4e5-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="6a4e5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a4e5-109">Permissions</span></span>
<span data-ttu-id="6a4e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a4e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a4e5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a4e5-112">Permission type</span></span>      | <span data-ttu-id="6a4e5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a4e5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a4e5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a4e5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6a4e5-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a4e5-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6a4e5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a4e5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a4e5-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a4e5-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6a4e5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a4e5-118">Application</span></span> | <span data-ttu-id="6a4e5-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a4e5-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a4e5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a4e5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a4e5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a4e5-121">Optional query parameters</span></span>
<span data-ttu-id="6a4e5-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a4e5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a4e5-123">Request headers</span></span>
| <span data-ttu-id="6a4e5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6a4e5-124">Name</span></span>       | <span data-ttu-id="6a4e5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6a4e5-125">Type</span></span> | <span data-ttu-id="6a4e5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6a4e5-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a4e5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a4e5-127">Authorization</span></span>  | <span data-ttu-id="6a4e5-128">string</span><span class="sxs-lookup"><span data-stu-id="6a4e5-128">string</span></span>  | <span data-ttu-id="6a4e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a4e5-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a4e5-131">Request body</span></span>
<span data-ttu-id="6a4e5-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a4e5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a4e5-133">Response</span></span>

<span data-ttu-id="6a4e5-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a4e5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="6a4e5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a4e5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a4e5-136">Request</span></span>
<span data-ttu-id="6a4e5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a4e5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a4e5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a4e5-139">C#</span><span class="sxs-lookup"><span data-stu-id="6a4e5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a4e5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a4e5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a4e5-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6a4e5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a4e5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a4e5-142">Response</span></span>
<span data-ttu-id="6a4e5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a4e5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
