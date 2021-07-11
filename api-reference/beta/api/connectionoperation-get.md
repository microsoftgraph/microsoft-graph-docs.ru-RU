---
title: Get connectionOperation
description: Извлечение свойств подключенияOperation.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f709d05f1b93b3443dffc5171da6deb39dadc187
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366578"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="01168-103">Get connectionOperation</span><span class="sxs-lookup"><span data-stu-id="01168-103">Get connectionOperation</span></span>

<span data-ttu-id="01168-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01168-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01168-105">Извлечение свойств [подключенияOperation](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="01168-105">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01168-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01168-106">Permissions</span></span>

<span data-ttu-id="01168-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01168-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01168-109">Permission type</span></span>                        | <span data-ttu-id="01168-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01168-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01168-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01168-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01168-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01168-112">Not supported.</span></span> |
| <span data-ttu-id="01168-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01168-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01168-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01168-114">Not supported.</span></span> |
| <span data-ttu-id="01168-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01168-115">Application</span></span>                            | <span data-ttu-id="01168-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01168-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01168-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01168-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="01168-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01168-118">Request headers</span></span>

| <span data-ttu-id="01168-119">Имя</span><span class="sxs-lookup"><span data-stu-id="01168-119">Name</span></span>          | <span data-ttu-id="01168-120">Описание</span><span class="sxs-lookup"><span data-stu-id="01168-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="01168-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01168-121">Authorization</span></span> | <span data-ttu-id="01168-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01168-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01168-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01168-124">Request body</span></span>

<span data-ttu-id="01168-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01168-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01168-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="01168-126">Response</span></span>

<span data-ttu-id="01168-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [connectionOperation](../resources/connectionoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="01168-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01168-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="01168-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01168-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="01168-129">Request</span></span>

<span data-ttu-id="01168-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01168-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01168-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="01168-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="01168-132">C#</span><span class="sxs-lookup"><span data-stu-id="01168-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01168-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01168-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01168-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01168-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01168-135">Java</span><span class="sxs-lookup"><span data-stu-id="01168-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectionoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="01168-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="01168-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="01168-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01168-137">The following is an example of the response.</span></span>

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


