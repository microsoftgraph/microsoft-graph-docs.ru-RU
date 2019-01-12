---
title: Получение ресурса
description: Получение двоичных данных объекта resource файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9937040d9e53213946df9eb31cf9136bcfda7c71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946065"
---
# <a name="get-resource"></a><span data-ttu-id="70e17-103">Получение ресурса</span><span class="sxs-lookup"><span data-stu-id="70e17-103">Get resource</span></span>

<span data-ttu-id="70e17-104">Получение двоичных данных объекта [resource](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="70e17-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="70e17-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70e17-105">Permissions</span></span>
<span data-ttu-id="70e17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70e17-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70e17-108">Permission type</span></span>      | <span data-ttu-id="70e17-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70e17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70e17-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70e17-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70e17-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e17-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="70e17-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70e17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70e17-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70e17-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="70e17-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70e17-114">Application</span></span> | <span data-ttu-id="70e17-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e17-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70e17-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70e17-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="70e17-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70e17-117">Request headers</span></span>
| <span data-ttu-id="70e17-118">Имя</span><span class="sxs-lookup"><span data-stu-id="70e17-118">Name</span></span>       | <span data-ttu-id="70e17-119">Тип</span><span class="sxs-lookup"><span data-stu-id="70e17-119">Type</span></span> | <span data-ttu-id="70e17-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70e17-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70e17-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70e17-121">Authorization</span></span>  | <span data-ttu-id="70e17-122">строка</span><span class="sxs-lookup"><span data-stu-id="70e17-122">string</span></span>  | <span data-ttu-id="70e17-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70e17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70e17-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70e17-125">Request body</span></span>
<span data-ttu-id="70e17-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70e17-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70e17-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="70e17-127">Response</span></span>

<span data-ttu-id="70e17-128">При успешном выполнении это метод возвращает код отклика `200 OK` и двоичные данные изображения или файла в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="70e17-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="70e17-129">Примечание. Изображения не будут отображаться непосредственно в браузере, так как для их получения необходима авторизация (как и для остальной части содержимого страницы).</span><span class="sxs-lookup"><span data-stu-id="70e17-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="70e17-130">Пример</span><span class="sxs-lookup"><span data-stu-id="70e17-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70e17-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="70e17-131">Request</span></span>
<span data-ttu-id="70e17-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70e17-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="70e17-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="70e17-133">Response</span></span>
<span data-ttu-id="70e17-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70e17-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
