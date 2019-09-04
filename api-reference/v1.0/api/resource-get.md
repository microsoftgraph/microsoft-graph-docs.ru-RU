---
title: Вывод ресурса
description: Получение двоичных данных объекта ресурса файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6bb2afc8e44b5dc64d8d3d509bcdbafe8bd16b9a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727826"
---
# <a name="get-resource"></a><span data-ttu-id="24356-103">Вывод ресурса</span><span class="sxs-lookup"><span data-stu-id="24356-103">Get resource</span></span>

<span data-ttu-id="24356-104">Получение двоичных данных объекта [ресурса](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="24356-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="24356-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24356-105">Permissions</span></span>
<span data-ttu-id="24356-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24356-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24356-108">Permission type</span></span>      | <span data-ttu-id="24356-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24356-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24356-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24356-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24356-111">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24356-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="24356-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24356-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24356-113">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24356-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="24356-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24356-114">Application</span></span> | <span data-ttu-id="24356-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24356-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24356-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24356-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="24356-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24356-117">Request headers</span></span>
| <span data-ttu-id="24356-118">Имя</span><span class="sxs-lookup"><span data-stu-id="24356-118">Name</span></span>       | <span data-ttu-id="24356-119">Тип</span><span class="sxs-lookup"><span data-stu-id="24356-119">Type</span></span> | <span data-ttu-id="24356-120">Описание</span><span class="sxs-lookup"><span data-stu-id="24356-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="24356-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="24356-121">Authorization</span></span>  | <span data-ttu-id="24356-122">string</span><span class="sxs-lookup"><span data-stu-id="24356-122">string</span></span>  | <span data-ttu-id="24356-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24356-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24356-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24356-125">Request body</span></span>
<span data-ttu-id="24356-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24356-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24356-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="24356-127">Response</span></span>

<span data-ttu-id="24356-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные изображения или файла в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24356-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="24356-129">Note: изображения не отображаются непосредственно в браузере, так как им требуется авторизация для их извлечения, как и остальная часть контента страницы.</span><span class="sxs-lookup"><span data-stu-id="24356-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="24356-130">Пример</span><span class="sxs-lookup"><span data-stu-id="24356-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24356-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="24356-131">Request</span></span>
<span data-ttu-id="24356-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24356-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24356-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="24356-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24356-134">C#</span><span class="sxs-lookup"><span data-stu-id="24356-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24356-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24356-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24356-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="24356-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="24356-137">Java</span><span class="sxs-lookup"><span data-stu-id="24356-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="24356-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="24356-138">Response</span></span>
<span data-ttu-id="24356-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24356-139">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
