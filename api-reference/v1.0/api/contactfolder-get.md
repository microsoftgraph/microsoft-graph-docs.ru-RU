---
title: Получение объекта contactFolder
description: Получение папки контактов с помощью ее идентификатора.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cb1f2e9c7a2e3f8870895eba06b7fe3eba8edf85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462163"
---
# <a name="get-contactfolder"></a><span data-ttu-id="d589c-103">Получение объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="d589c-103">Get contactFolder</span></span>

<span data-ttu-id="d589c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d589c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d589c-105">Получение папки контактов с помощью ее идентификатора.</span><span class="sxs-lookup"><span data-stu-id="d589c-105">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="d589c-106">Существует два сценария, в которых приложение может получить папку контактов другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="d589c-106">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="d589c-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="d589c-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d589c-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="d589c-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d589c-109">См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="d589c-109">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="d589c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d589c-110">Permissions</span></span>
<span data-ttu-id="d589c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d589c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d589c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d589c-113">Permission type</span></span>      | <span data-ttu-id="d589c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d589c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d589c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d589c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d589c-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d589c-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d589c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d589c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d589c-118">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d589c-118">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d589c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d589c-119">Application</span></span> | <span data-ttu-id="d589c-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d589c-120">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d589c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d589c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d589c-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d589c-122">Optional query parameters</span></span>
<span data-ttu-id="d589c-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d589c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d589c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d589c-124">Request headers</span></span>
| <span data-ttu-id="d589c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d589c-125">Name</span></span>       | <span data-ttu-id="d589c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d589c-126">Type</span></span> | <span data-ttu-id="d589c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d589c-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d589c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d589c-128">Authorization</span></span>  | <span data-ttu-id="d589c-129">string</span><span class="sxs-lookup"><span data-stu-id="d589c-129">string</span></span>  | <span data-ttu-id="d589c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d589c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d589c-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d589c-132">Request body</span></span>
<span data-ttu-id="d589c-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d589c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d589c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d589c-134">Response</span></span>

<span data-ttu-id="d589c-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d589c-135">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d589c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d589c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d589c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d589c-137">Request</span></span>
<span data-ttu-id="d589c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d589c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d589c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d589c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="d589c-140">C#</span><span class="sxs-lookup"><span data-stu-id="d589c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d589c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d589c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d589c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d589c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d589c-143">Java</span><span class="sxs-lookup"><span data-stu-id="d589c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d589c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d589c-144">Response</span></span>
<span data-ttu-id="d589c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d589c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
