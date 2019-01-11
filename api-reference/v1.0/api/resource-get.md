---
title: Получение ресурса
description: Получение двоичных данных объекта resource файла или изображения.
localization_priority: Normal
ms.openlocfilehash: ec28daacf61e18f16e5c6598d036759eac1fb131
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884793"
---
# <a name="get-resource"></a><span data-ttu-id="3edf5-103">Получение ресурса</span><span class="sxs-lookup"><span data-stu-id="3edf5-103">Get resource</span></span>

<span data-ttu-id="3edf5-104">Получение двоичных данных объекта [resource](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="3edf5-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3edf5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3edf5-105">Permissions</span></span>
<span data-ttu-id="3edf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3edf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3edf5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3edf5-108">Permission type</span></span>      | <span data-ttu-id="3edf5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3edf5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3edf5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3edf5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3edf5-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3edf5-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3edf5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3edf5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3edf5-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3edf5-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3edf5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3edf5-114">Application</span></span> | <span data-ttu-id="3edf5-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3edf5-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3edf5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3edf5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="3edf5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3edf5-117">Request headers</span></span>
| <span data-ttu-id="3edf5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3edf5-118">Name</span></span>       | <span data-ttu-id="3edf5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3edf5-119">Type</span></span> | <span data-ttu-id="3edf5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3edf5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3edf5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3edf5-121">Authorization</span></span>  | <span data-ttu-id="3edf5-122">string</span><span class="sxs-lookup"><span data-stu-id="3edf5-122">string</span></span>  | <span data-ttu-id="3edf5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3edf5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3edf5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3edf5-125">Request body</span></span>
<span data-ttu-id="3edf5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3edf5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3edf5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3edf5-127">Response</span></span>

<span data-ttu-id="3edf5-128">При успешном выполнении это метод возвращает код отклика `200 OK` и двоичные данные изображения или файла в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3edf5-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="3edf5-129">Примечание. Изображения не будут отображаться непосредственно в браузере, так как для их получения необходима авторизация (как и для остальной части содержимого страницы).</span><span class="sxs-lookup"><span data-stu-id="3edf5-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="3edf5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3edf5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3edf5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3edf5-131">Request</span></span>
<span data-ttu-id="3edf5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3edf5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="3edf5-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="3edf5-133">Response</span></span>
<span data-ttu-id="3edf5-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3edf5-134">Here is an example of the response.</span></span>
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
