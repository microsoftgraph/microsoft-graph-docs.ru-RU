---
title: Получение фотографии
description: Получение свойств и связей объекта фотографии.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 48ba8ef11dedc266a24cb84dc29dd4de1bd9af81
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730066"
---
# <a name="get-photo"></a><span data-ttu-id="8f04f-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="8f04f-103">Get photo</span></span>

<span data-ttu-id="8f04f-104">Получение свойств и связей объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="8f04f-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f04f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f04f-105">Permissions</span></span>
<span data-ttu-id="8f04f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f04f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f04f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f04f-108">Permission type</span></span>      | <span data-ttu-id="8f04f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f04f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f04f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f04f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f04f-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="8f04f-111">Files.Read</span></span>    |
|<span data-ttu-id="8f04f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f04f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f04f-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="8f04f-113">Files.Read</span></span>    |
|<span data-ttu-id="8f04f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f04f-114">Application</span></span> | <span data-ttu-id="8f04f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f04f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f04f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f04f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8f04f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f04f-117">Optional query parameters</span></span>
<span data-ttu-id="8f04f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f04f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f04f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f04f-119">Request headers</span></span>
| <span data-ttu-id="8f04f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8f04f-120">Name</span></span>       | <span data-ttu-id="8f04f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8f04f-121">Type</span></span> | <span data-ttu-id="8f04f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8f04f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f04f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f04f-123">Authorization</span></span>  | <span data-ttu-id="8f04f-124">string</span><span class="sxs-lookup"><span data-stu-id="8f04f-124">string</span></span>  | <span data-ttu-id="8f04f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f04f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f04f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f04f-127">Request body</span></span>
<span data-ttu-id="8f04f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f04f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f04f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f04f-129">Response</span></span>

<span data-ttu-id="8f04f-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f04f-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f04f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f04f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f04f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f04f-132">Request</span></span>
<span data-ttu-id="8f04f-133">Ниже приведен пример запроса на получение метаданных фотографий.</span><span class="sxs-lookup"><span data-stu-id="8f04f-133">Here is an example of the request for photo metadata.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f04f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f04f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f04f-135">C#</span><span class="sxs-lookup"><span data-stu-id="8f04f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f04f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f04f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f04f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f04f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f04f-138">Java</span><span class="sxs-lookup"><span data-stu-id="8f04f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f04f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f04f-139">Response</span></span>
<span data-ttu-id="8f04f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f04f-140">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="8f04f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f04f-141">Request</span></span>
<span data-ttu-id="8f04f-142">Ниже приведен пример запроса на получение байтов фотографий.</span><span class="sxs-lookup"><span data-stu-id="8f04f-142">Here is an example of the request for the photo bytes.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f04f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f04f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f04f-144">C#</span><span class="sxs-lookup"><span data-stu-id="8f04f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f04f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f04f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f04f-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f04f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f04f-147">Java</span><span class="sxs-lookup"><span data-stu-id="8f04f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f04f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f04f-148">Response</span></span>
<span data-ttu-id="8f04f-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f04f-149">Here is an example of the response.</span></span>

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
