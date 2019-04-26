---
title: Получение фотографии
description: Получение свойств и связей объекта фотографии.
localization_priority: Normal
ms.openlocfilehash: 095461082e3574b9be4d8ae839fa9d2ebc533202
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332565"
---
# <a name="get-photo"></a><span data-ttu-id="ae9af-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="ae9af-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae9af-104">Получение свойств и связей объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="ae9af-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae9af-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae9af-105">Permissions</span></span>
<span data-ttu-id="ae9af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae9af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae9af-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae9af-108">Permission type</span></span>      | <span data-ttu-id="ae9af-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae9af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae9af-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae9af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae9af-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="ae9af-111">Files.Read</span></span>    |
|<span data-ttu-id="ae9af-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae9af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae9af-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="ae9af-113">Files.Read</span></span>    |
|<span data-ttu-id="ae9af-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae9af-114">Application</span></span> | <span data-ttu-id="ae9af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae9af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae9af-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae9af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae9af-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae9af-117">Optional query parameters</span></span>
<span data-ttu-id="ae9af-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae9af-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae9af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae9af-119">Request headers</span></span>
| <span data-ttu-id="ae9af-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ae9af-120">Name</span></span>       | <span data-ttu-id="ae9af-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ae9af-121">Type</span></span> | <span data-ttu-id="ae9af-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ae9af-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae9af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae9af-123">Authorization</span></span>  | <span data-ttu-id="ae9af-124">string</span><span class="sxs-lookup"><span data-stu-id="ae9af-124">string</span></span>  | <span data-ttu-id="ae9af-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae9af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae9af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae9af-127">Request body</span></span>
<span data-ttu-id="ae9af-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae9af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae9af-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae9af-129">Response</span></span>

<span data-ttu-id="ae9af-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae9af-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="ae9af-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae9af-131">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="ae9af-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae9af-132">Request</span></span>
<span data-ttu-id="ae9af-133">Ниже приведен пример запроса на получение метаданных фотографий.</span><span class="sxs-lookup"><span data-stu-id="ae9af-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="ae9af-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae9af-134">Response</span></span>
<span data-ttu-id="ae9af-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae9af-135">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="ae9af-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae9af-136">Request</span></span>
<span data-ttu-id="ae9af-137">Ниже приведен пример запроса на получение байтов фотографий.</span><span class="sxs-lookup"><span data-stu-id="ae9af-137">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="ae9af-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae9af-138">Response</span></span>
<span data-ttu-id="ae9af-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae9af-139">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
