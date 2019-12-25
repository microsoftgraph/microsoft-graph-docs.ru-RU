---
title: Получение Коннектионоператион
description: Получение свойств объекта Коннектионоператион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 99bd074aed8c24a6d1990c753c8ea5ffe537097f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868067"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="87ae6-103">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="87ae6-103">Get connectionOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87ae6-104">Получение свойств объекта [коннектионоператион](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="87ae6-104">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="87ae6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87ae6-105">Permissions</span></span>

<span data-ttu-id="87ae6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ae6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87ae6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87ae6-108">Permission type</span></span>                        | <span data-ttu-id="87ae6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87ae6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87ae6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87ae6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="87ae6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ae6-111">Not supported.</span></span> |
| <span data-ttu-id="87ae6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87ae6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87ae6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ae6-113">Not supported.</span></span> |
| <span data-ttu-id="87ae6-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="87ae6-114">Application</span></span>                            | <span data-ttu-id="87ae6-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ae6-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87ae6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87ae6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="87ae6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87ae6-117">Request headers</span></span>

| <span data-ttu-id="87ae6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="87ae6-118">Name</span></span>          | <span data-ttu-id="87ae6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="87ae6-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="87ae6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87ae6-120">Authorization</span></span> | <span data-ttu-id="87ae6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87ae6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87ae6-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87ae6-123">Request body</span></span>

<span data-ttu-id="87ae6-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87ae6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ae6-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="87ae6-125">Response</span></span>

<span data-ttu-id="87ae6-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [коннектионоператион](../resources/connectionoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87ae6-126">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87ae6-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="87ae6-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87ae6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="87ae6-128">Request</span></span>

<span data-ttu-id="87ae6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87ae6-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="87ae6-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="87ae6-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87ae6-131">C#</span><span class="sxs-lookup"><span data-stu-id="87ae6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87ae6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87ae6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87ae6-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87ae6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="87ae6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87ae6-134">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="87ae6-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="87ae6-135">The following is an example of the response.</span></span>

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
