---
title: Удаление Екстерналконнектион
description: Удаление Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 1b3e795c51f6ded27bb9f63706939c5a5ff1fa8b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965670"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="8b329-103">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="8b329-103">Delete externalConnection</span></span>

<span data-ttu-id="8b329-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b329-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b329-105">Удаление [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="8b329-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="8b329-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b329-106">Permissions</span></span>

<span data-ttu-id="8b329-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b329-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b329-109">Permission type</span></span>                        | <span data-ttu-id="8b329-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b329-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b329-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b329-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b329-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b329-112">Not supported.</span></span> |
| <span data-ttu-id="8b329-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b329-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b329-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b329-114">Not supported.</span></span> |
| <span data-ttu-id="8b329-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8b329-115">Application</span></span>                            | <span data-ttu-id="8b329-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b329-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b329-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b329-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b329-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b329-118">Request headers</span></span>

| <span data-ttu-id="8b329-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8b329-119">Name</span></span>          | <span data-ttu-id="8b329-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8b329-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8b329-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b329-121">Authorization</span></span> | <span data-ttu-id="8b329-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b329-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b329-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b329-124">Request body</span></span>

<span data-ttu-id="8b329-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b329-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b329-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b329-126">Response</span></span>

<span data-ttu-id="8b329-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8b329-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b329-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b329-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b329-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b329-130">Request</span></span>

<span data-ttu-id="8b329-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b329-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b329-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b329-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="8b329-133">C#</span><span class="sxs-lookup"><span data-stu-id="8b329-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b329-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b329-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b329-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b329-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b329-136">Java</span><span class="sxs-lookup"><span data-stu-id="8b329-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8b329-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b329-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="8b329-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8b329-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
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


