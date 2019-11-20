---
title: Получение Коннектионоператион
description: Получение свойств объекта Коннектионоператион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b09a9ac40cd79a8f543fcb910385d09a3d598dcb
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747525"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="2e8b3-103">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="2e8b3-103">Get connectionOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e8b3-104">Получение свойств объекта [коннектионоператион](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="2e8b3-104">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="2e8b3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e8b3-105">Permissions</span></span>

<span data-ttu-id="2e8b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e8b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e8b3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e8b3-108">Permission type</span></span>                        | <span data-ttu-id="2e8b3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e8b3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e8b3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e8b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e8b3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-111">Not supported.</span></span> |
| <span data-ttu-id="2e8b3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e8b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e8b3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-113">Not supported.</span></span> |
| <span data-ttu-id="2e8b3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e8b3-114">Application</span></span>                            | <span data-ttu-id="2e8b3-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8b3-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e8b3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e8b3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="2e8b3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e8b3-117">Request headers</span></span>

| <span data-ttu-id="2e8b3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2e8b3-118">Name</span></span>          | <span data-ttu-id="2e8b3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2e8b3-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2e8b3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e8b3-120">Authorization</span></span> | <span data-ttu-id="2e8b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e8b3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e8b3-123">Request body</span></span>

<span data-ttu-id="2e8b3-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e8b3-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e8b3-125">Response</span></span>

<span data-ttu-id="2e8b3-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [коннектионоператион](../resources/connectionoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-126">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e8b3-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e8b3-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e8b3-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e8b3-128">Request</span></span>

<span data-ttu-id="2e8b3-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2e8b3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e8b3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e8b3-131">C#</span><span class="sxs-lookup"><span data-stu-id="2e8b3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e8b3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e8b3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e8b3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e8b3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2e8b3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e8b3-134">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2e8b3-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e8b3-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.connectionOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
