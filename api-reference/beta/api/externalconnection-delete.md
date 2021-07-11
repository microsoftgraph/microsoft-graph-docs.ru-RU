---
title: Удаление externalConnection
description: Удаление externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a50d9f900d0cece20a3c3088a303b41a2ba7999b
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366900"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="cfc6c-103">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="cfc6c-103">Delete externalConnection</span></span>

<span data-ttu-id="cfc6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfc6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfc6c-105">Удаление [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="cfc6c-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfc6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfc6c-106">Permissions</span></span>

<span data-ttu-id="cfc6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfc6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfc6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfc6c-109">Permission type</span></span>                        | <span data-ttu-id="cfc6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfc6c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfc6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfc6c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfc6c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-112">Not supported.</span></span> |
| <span data-ttu-id="cfc6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfc6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfc6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-114">Not supported.</span></span> |
| <span data-ttu-id="cfc6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfc6c-115">Application</span></span>                            | <span data-ttu-id="cfc6c-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfc6c-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfc6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfc6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfc6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfc6c-118">Request headers</span></span>

| <span data-ttu-id="cfc6c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cfc6c-119">Name</span></span>          | <span data-ttu-id="cfc6c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cfc6c-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cfc6c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfc6c-121">Authorization</span></span> | <span data-ttu-id="cfc6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfc6c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfc6c-124">Request body</span></span>

<span data-ttu-id="cfc6c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfc6c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfc6c-126">Response</span></span>

<span data-ttu-id="cfc6c-p103">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfc6c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="cfc6c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfc6c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfc6c-130">Request</span></span>

<span data-ttu-id="cfc6c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfc6c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc6c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="cfc6c-133">C#</span><span class="sxs-lookup"><span data-stu-id="cfc6c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfc6c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc6c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfc6c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc6c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfc6c-136">Java</span><span class="sxs-lookup"><span data-stu-id="cfc6c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="cfc6c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfc6c-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="cfc6c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cfc6c-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete externalConnection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


