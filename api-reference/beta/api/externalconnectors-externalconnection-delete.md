---
title: Удаление externalConnection
description: Удаление externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a33561b82527ab4494303b3b7cb092f0b7a57a7a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467708"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="5c222-103">Удаление externalConnection</span><span class="sxs-lookup"><span data-stu-id="5c222-103">Delete externalConnection</span></span>

<span data-ttu-id="5c222-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="5c222-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c222-105">Удаление [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="5c222-105">Delete an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c222-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c222-106">Permissions</span></span>

<span data-ttu-id="5c222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c222-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c222-109">Permission type</span></span>                        | <span data-ttu-id="5c222-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c222-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c222-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c222-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c222-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c222-112">Not supported.</span></span> |
| <span data-ttu-id="5c222-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c222-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c222-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c222-114">Not supported.</span></span> |
| <span data-ttu-id="5c222-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5c222-115">Application</span></span>                            | <span data-ttu-id="5c222-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="5c222-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c222-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c222-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5c222-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c222-118">Request headers</span></span>

| <span data-ttu-id="5c222-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c222-119">Name</span></span>          | <span data-ttu-id="5c222-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c222-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5c222-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c222-121">Authorization</span></span> | <span data-ttu-id="5c222-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c222-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c222-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c222-124">Request body</span></span>

<span data-ttu-id="5c222-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c222-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c222-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c222-126">Response</span></span>

<span data-ttu-id="5c222-p103">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5c222-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c222-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c222-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c222-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c222-130">Request</span></span>

<span data-ttu-id="5c222-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c222-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c222-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c222-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="5c222-133">C#</span><span class="sxs-lookup"><span data-stu-id="5c222-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c222-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c222-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c222-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c222-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c222-136">Java</span><span class="sxs-lookup"><span data-stu-id="5c222-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5c222-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c222-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="5c222-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5c222-138">The following is an example of the response.</span></span>

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


