---
title: Вывод ресурса
description: Получение двоичных данных объекта ресурса файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9fe2b1a23f3079022c20ab16e9b8d8efb4a1e759
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453907"
---
# <a name="get-resource"></a><span data-ttu-id="ea3d7-103">Вывод ресурса</span><span class="sxs-lookup"><span data-stu-id="ea3d7-103">Get resource</span></span>

<span data-ttu-id="ea3d7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ea3d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea3d7-105">Получение двоичных данных объекта [ресурса](../resources/onenoteresource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-105">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea3d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea3d7-106">Permissions</span></span>
<span data-ttu-id="ea3d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea3d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea3d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea3d7-109">Permission type</span></span>      | <span data-ttu-id="ea3d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea3d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea3d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea3d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea3d7-112">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ea3d7-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea3d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea3d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea3d7-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea3d7-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ea3d7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea3d7-115">Application</span></span> | <span data-ttu-id="ea3d7-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea3d7-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea3d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea3d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="ea3d7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea3d7-118">Request headers</span></span>
| <span data-ttu-id="ea3d7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ea3d7-119">Name</span></span>       | <span data-ttu-id="ea3d7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ea3d7-120">Type</span></span> | <span data-ttu-id="ea3d7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ea3d7-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea3d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea3d7-122">Authorization</span></span>  | <span data-ttu-id="ea3d7-123">string</span><span class="sxs-lookup"><span data-stu-id="ea3d7-123">string</span></span>  | <span data-ttu-id="ea3d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea3d7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea3d7-126">Request body</span></span>
<span data-ttu-id="ea3d7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea3d7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea3d7-128">Response</span></span>

<span data-ttu-id="ea3d7-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные изображения или файла в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-129">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="ea3d7-130">Note: изображения не отображаются непосредственно в браузере, так как им требуется авторизация для их извлечения, как и остальная часть контента страницы.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-130">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="ea3d7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ea3d7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea3d7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea3d7-132">Request</span></span>
<span data-ttu-id="ea3d7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea3d7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea3d7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
# <a name="c"></a>[<span data-ttu-id="ea3d7-135">C#</span><span class="sxs-lookup"><span data-stu-id="ea3d7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea3d7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea3d7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea3d7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea3d7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea3d7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea3d7-138">Response</span></span>
<span data-ttu-id="ea3d7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea3d7-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
