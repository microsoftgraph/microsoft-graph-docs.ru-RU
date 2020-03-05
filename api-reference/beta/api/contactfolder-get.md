---
title: Получение объекта contactFolder
description: Получение папки контактов с помощью ее идентификатора.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 78f70919b00b275572efef6287f3fdf3da7995c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436988"
---
# <a name="get-contactfolder"></a><span data-ttu-id="6f335-103">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="6f335-103">Get contactFolder</span></span>

<span data-ttu-id="6f335-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f335-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f335-105">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="6f335-105">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="6f335-106">Существует два сценария, в которых приложение может получить папку контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="6f335-106">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="6f335-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="6f335-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6f335-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="6f335-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6f335-109">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="6f335-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="6f335-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f335-110">Permissions</span></span>
<span data-ttu-id="6f335-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f335-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f335-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f335-113">Permission type</span></span>      | <span data-ttu-id="6f335-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f335-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f335-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f335-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6f335-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f335-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6f335-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f335-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f335-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f335-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6f335-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f335-119">Application</span></span> | <span data-ttu-id="6f335-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f335-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f335-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f335-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f335-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f335-122">Optional query parameters</span></span>
<span data-ttu-id="6f335-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6f335-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6f335-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f335-124">Request headers</span></span>
| <span data-ttu-id="6f335-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6f335-125">Name</span></span>       | <span data-ttu-id="6f335-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6f335-126">Type</span></span> | <span data-ttu-id="6f335-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6f335-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f335-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f335-128">Authorization</span></span>  | <span data-ttu-id="6f335-129">string</span><span class="sxs-lookup"><span data-stu-id="6f335-129">string</span></span>  | <span data-ttu-id="6f335-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f335-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f335-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f335-132">Request body</span></span>
<span data-ttu-id="6f335-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f335-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f335-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f335-134">Response</span></span>

<span data-ttu-id="6f335-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f335-135">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f335-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6f335-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f335-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f335-137">Request</span></span>
<span data-ttu-id="6f335-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f335-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f335-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f335-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="6f335-140">C#</span><span class="sxs-lookup"><span data-stu-id="6f335-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f335-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f335-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f335-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f335-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f335-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f335-143">Response</span></span>
<span data-ttu-id="6f335-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f335-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
