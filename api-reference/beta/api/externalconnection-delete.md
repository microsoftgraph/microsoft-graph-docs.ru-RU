---
title: Удаление externalConnection
description: Удаление внешнего подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 37b46e3cd6de8a12d6a77106abbe81a8a5da090f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943614"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="e8945-103">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="e8945-103">Delete externalConnection</span></span>

<span data-ttu-id="e8945-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8945-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8945-105">Удаление [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="e8945-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="e8945-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8945-106">Permissions</span></span>

<span data-ttu-id="e8945-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8945-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8945-109">Permission type</span></span>                        | <span data-ttu-id="e8945-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8945-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8945-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8945-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8945-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8945-112">Not supported.</span></span> |
| <span data-ttu-id="e8945-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8945-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8945-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8945-114">Not supported.</span></span> |
| <span data-ttu-id="e8945-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8945-115">Application</span></span>                            | <span data-ttu-id="e8945-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8945-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8945-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8945-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8945-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8945-118">Request headers</span></span>

| <span data-ttu-id="e8945-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8945-119">Name</span></span>          | <span data-ttu-id="e8945-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8945-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e8945-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8945-121">Authorization</span></span> | <span data-ttu-id="e8945-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8945-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8945-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8945-124">Request body</span></span>

<span data-ttu-id="e8945-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8945-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8945-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8945-126">Response</span></span>

<span data-ttu-id="e8945-p103">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e8945-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8945-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8945-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8945-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8945-130">Request</span></span>

<span data-ttu-id="e8945-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8945-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8945-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8945-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="e8945-133">C#</span><span class="sxs-lookup"><span data-stu-id="e8945-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8945-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8945-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8945-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8945-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8945-136">Java</span><span class="sxs-lookup"><span data-stu-id="e8945-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="e8945-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8945-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="e8945-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8945-138">The following is an example of the response.</span></span>

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


