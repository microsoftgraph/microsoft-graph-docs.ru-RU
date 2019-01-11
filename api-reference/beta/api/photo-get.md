---
title: Получение фотографии
description: Получение свойств и связей объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: ff46fca695140cabf363f9bccfcc61bc4fb50279
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824467"
---
# <a name="get-photo"></a><span data-ttu-id="43c6e-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="43c6e-103">Get photo</span></span>

> <span data-ttu-id="43c6e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43c6e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43c6e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43c6e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43c6e-106">Получение свойств и связей объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="43c6e-106">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="43c6e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43c6e-107">Permissions</span></span>
<span data-ttu-id="43c6e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43c6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43c6e-110">Permission type</span></span>      | <span data-ttu-id="43c6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43c6e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43c6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43c6e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="43c6e-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="43c6e-113">Files.Read</span></span>    |
|<span data-ttu-id="43c6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43c6e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43c6e-115">Files.Read</span><span class="sxs-lookup"><span data-stu-id="43c6e-115">Files.Read</span></span>    |
|<span data-ttu-id="43c6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43c6e-116">Application</span></span> | <span data-ttu-id="43c6e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43c6e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43c6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43c6e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="43c6e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43c6e-119">Optional query parameters</span></span>
<span data-ttu-id="43c6e-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43c6e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43c6e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43c6e-121">Request headers</span></span>
| <span data-ttu-id="43c6e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="43c6e-122">Name</span></span>       | <span data-ttu-id="43c6e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="43c6e-123">Type</span></span> | <span data-ttu-id="43c6e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="43c6e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="43c6e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c6e-125">Authorization</span></span>  | <span data-ttu-id="43c6e-126">string</span><span class="sxs-lookup"><span data-stu-id="43c6e-126">string</span></span>  | <span data-ttu-id="43c6e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43c6e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43c6e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43c6e-129">Request body</span></span>
<span data-ttu-id="43c6e-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43c6e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c6e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c6e-131">Response</span></span>

<span data-ttu-id="43c6e-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43c6e-132">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="43c6e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="43c6e-133">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="43c6e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="43c6e-134">Request</span></span>
<span data-ttu-id="43c6e-135">Ниже приведен пример запроса на получение метаданных фотографий.</span><span class="sxs-lookup"><span data-stu-id="43c6e-135">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="43c6e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c6e-136">Response</span></span>
<span data-ttu-id="43c6e-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="43c6e-137">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="43c6e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="43c6e-138">Request</span></span>
<span data-ttu-id="43c6e-139">Ниже приведен пример запроса на получение байтов фотографий.</span><span class="sxs-lookup"><span data-stu-id="43c6e-139">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="43c6e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="43c6e-140">Response</span></span>
<span data-ttu-id="43c6e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="43c6e-141">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored","@odata.type": "stream" } -->

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
  "tocPath": ""
}-->
