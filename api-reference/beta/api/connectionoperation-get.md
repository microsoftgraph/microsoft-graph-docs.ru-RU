---
title: Получение Коннектионоператион
description: Получение свойств объекта Коннектионоператион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 53a52e4af74fcf8ee0528dbd3ac31f56a93a3d13
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957554"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="9ab01-103">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="9ab01-103">Get connectionOperation</span></span>

<span data-ttu-id="9ab01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ab01-105">Получение свойств объекта [коннектионоператион](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9ab01-105">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="9ab01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ab01-106">Permissions</span></span>

<span data-ttu-id="9ab01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ab01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ab01-109">Permission type</span></span>                        | <span data-ttu-id="9ab01-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ab01-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ab01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ab01-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ab01-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab01-112">Not supported.</span></span> |
| <span data-ttu-id="9ab01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ab01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ab01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab01-114">Not supported.</span></span> |
| <span data-ttu-id="9ab01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ab01-115">Application</span></span>                            | <span data-ttu-id="9ab01-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab01-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ab01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ab01-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="9ab01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ab01-118">Request headers</span></span>

| <span data-ttu-id="9ab01-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9ab01-119">Name</span></span>          | <span data-ttu-id="9ab01-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab01-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9ab01-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ab01-121">Authorization</span></span> | <span data-ttu-id="9ab01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ab01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ab01-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ab01-124">Request body</span></span>

<span data-ttu-id="9ab01-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ab01-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab01-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab01-126">Response</span></span>

<span data-ttu-id="9ab01-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [коннектионоператион](../resources/connectionoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ab01-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ab01-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ab01-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ab01-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab01-129">Request</span></span>

<span data-ttu-id="9ab01-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ab01-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ab01-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab01-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="9ab01-132">C#</span><span class="sxs-lookup"><span data-stu-id="9ab01-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab01-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab01-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab01-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab01-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ab01-135">Java</span><span class="sxs-lookup"><span data-stu-id="9ab01-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectionoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="9ab01-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab01-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9ab01-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9ab01-137">The following is an example of the response.</span></span>

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


