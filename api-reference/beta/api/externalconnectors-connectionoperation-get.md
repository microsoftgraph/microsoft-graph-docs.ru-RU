---
title: Get connectionOperation
description: Извлечение свойств подключенияOperation.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 1592c1fc4a47195d51f1a744884680a4467b171b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467714"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="636a0-103">Get connectionOperation</span><span class="sxs-lookup"><span data-stu-id="636a0-103">Get connectionOperation</span></span>

<span data-ttu-id="636a0-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="636a0-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="636a0-105">Извлечение свойств [подключенияOperation](../resources/externalconnectors-connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="636a0-105">Retrieve the properties of a [connectionOperation](../resources/externalconnectors-connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="636a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="636a0-106">Permissions</span></span>

<span data-ttu-id="636a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="636a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="636a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="636a0-109">Permission type</span></span>                        | <span data-ttu-id="636a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="636a0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="636a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="636a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="636a0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636a0-112">Not supported.</span></span> |
| <span data-ttu-id="636a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="636a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="636a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636a0-114">Not supported.</span></span> |
| <span data-ttu-id="636a0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="636a0-115">Application</span></span>                            | <span data-ttu-id="636a0-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="636a0-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="636a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="636a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="636a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="636a0-118">Request headers</span></span>

| <span data-ttu-id="636a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="636a0-119">Name</span></span>          | <span data-ttu-id="636a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="636a0-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="636a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="636a0-121">Authorization</span></span> | <span data-ttu-id="636a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="636a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="636a0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="636a0-124">Request body</span></span>

<span data-ttu-id="636a0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="636a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="636a0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="636a0-126">Response</span></span>

<span data-ttu-id="636a0-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [connectionOperation](../resources/externalconnectors-connectionoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="636a0-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/externalconnectors-connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="636a0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="636a0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="636a0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="636a0-129">Request</span></span>

<span data-ttu-id="636a0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="636a0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="636a0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="636a0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="636a0-132">C#</span><span class="sxs-lookup"><span data-stu-id="636a0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="636a0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="636a0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="636a0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="636a0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="636a0-135">Java</span><span class="sxs-lookup"><span data-stu-id="636a0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectionoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="636a0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="636a0-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="636a0-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="636a0-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation"
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
