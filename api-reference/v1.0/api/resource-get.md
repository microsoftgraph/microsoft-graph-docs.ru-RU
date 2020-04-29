---
title: Вывод ресурса
description: Получение двоичных данных объекта ресурса файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c4112be06512ba0f974206721ac5fb186cf7573e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509978"
---
# <a name="get-resource"></a><span data-ttu-id="061f2-103">Вывод ресурса</span><span class="sxs-lookup"><span data-stu-id="061f2-103">Get resource</span></span>

<span data-ttu-id="061f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="061f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="061f2-105">Получение двоичных данных объекта [ресурса](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="061f2-105">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="061f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="061f2-106">Permissions</span></span>
<span data-ttu-id="061f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="061f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="061f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="061f2-109">Permission type</span></span>      | <span data-ttu-id="061f2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="061f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="061f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="061f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="061f2-112">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="061f2-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="061f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="061f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="061f2-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="061f2-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="061f2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="061f2-115">Application</span></span> | <span data-ttu-id="061f2-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="061f2-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="061f2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="061f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="061f2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="061f2-118">Request headers</span></span>
| <span data-ttu-id="061f2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="061f2-119">Name</span></span>       | <span data-ttu-id="061f2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="061f2-120">Type</span></span> | <span data-ttu-id="061f2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="061f2-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="061f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="061f2-122">Authorization</span></span>  | <span data-ttu-id="061f2-123">string</span><span class="sxs-lookup"><span data-stu-id="061f2-123">string</span></span>  | <span data-ttu-id="061f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="061f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="061f2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="061f2-126">Request body</span></span>
<span data-ttu-id="061f2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="061f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="061f2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="061f2-128">Response</span></span>

<span data-ttu-id="061f2-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные изображения или файла в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="061f2-129">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="061f2-130">Note: изображения не отображаются непосредственно в браузере, так как им требуется авторизация для их извлечения, как и остальная часть контента страницы.</span><span class="sxs-lookup"><span data-stu-id="061f2-130">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="061f2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="061f2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="061f2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="061f2-132">Request</span></span>
<span data-ttu-id="061f2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="061f2-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="061f2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="061f2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
# <a name="c"></a>[<span data-ttu-id="061f2-135">C#</span><span class="sxs-lookup"><span data-stu-id="061f2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="061f2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061f2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="061f2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="061f2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="061f2-138">Java</span><span class="sxs-lookup"><span data-stu-id="061f2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="061f2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="061f2-139">Response</span></span>
<span data-ttu-id="061f2-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="061f2-140">Here is an example of the response.</span></span>
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
