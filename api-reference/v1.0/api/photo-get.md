---
title: Получение фотографии
description: Получение свойств и связей объекта фотографии.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: ab055019a467f8783e8d62e8c660bfa32e03bc4c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808741"
---
# <a name="get-photo"></a><span data-ttu-id="e5abd-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="e5abd-103">Get photo</span></span>

<span data-ttu-id="e5abd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5abd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5abd-105">Получение свойств и связей объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="e5abd-105">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5abd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5abd-106">Permissions</span></span>
<span data-ttu-id="e5abd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5abd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5abd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5abd-109">Permission type</span></span>      | <span data-ttu-id="e5abd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5abd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5abd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5abd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5abd-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e5abd-112">Files.Read</span></span>    |
|<span data-ttu-id="e5abd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5abd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5abd-114">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e5abd-114">Files.Read</span></span>    |
|<span data-ttu-id="e5abd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5abd-115">Application</span></span> | <span data-ttu-id="e5abd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5abd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5abd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5abd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5abd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5abd-118">Optional query parameters</span></span>
<span data-ttu-id="e5abd-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5abd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5abd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5abd-120">Request headers</span></span>
| <span data-ttu-id="e5abd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e5abd-121">Name</span></span>       | <span data-ttu-id="e5abd-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e5abd-122">Type</span></span> | <span data-ttu-id="e5abd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e5abd-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e5abd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5abd-124">Authorization</span></span>  | <span data-ttu-id="e5abd-125">string</span><span class="sxs-lookup"><span data-stu-id="e5abd-125">string</span></span>  | <span data-ttu-id="e5abd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5abd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5abd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5abd-128">Request body</span></span>
<span data-ttu-id="e5abd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5abd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5abd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5abd-130">Response</span></span>

<span data-ttu-id="e5abd-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5abd-131">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5abd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e5abd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5abd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5abd-133">Request</span></span>
<span data-ttu-id="e5abd-134">Ниже приведен пример запроса на получение метаданных фотографий.</span><span class="sxs-lookup"><span data-stu-id="e5abd-134">Here is an example of the request for photo metadata.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5abd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5abd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="e5abd-136">C#</span><span class="sxs-lookup"><span data-stu-id="e5abd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5abd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5abd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5abd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5abd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5abd-139">Java</span><span class="sxs-lookup"><span data-stu-id="e5abd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5abd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5abd-140">Response</span></span>
<span data-ttu-id="e5abd-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5abd-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="request"></a><span data-ttu-id="e5abd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5abd-142">Request</span></span>
<span data-ttu-id="e5abd-143">Ниже приведен пример запроса на получение байтов фотографий.</span><span class="sxs-lookup"><span data-stu-id="e5abd-143">Here is an example of the request for the photo bytes.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5abd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5abd-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
# <a name="c"></a>[<span data-ttu-id="e5abd-145">C#</span><span class="sxs-lookup"><span data-stu-id="e5abd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5abd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5abd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5abd-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5abd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5abd-148">Java</span><span class="sxs-lookup"><span data-stu-id="e5abd-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5abd-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5abd-149">Response</span></span>
<span data-ttu-id="e5abd-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5abd-150">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Edm.Stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
