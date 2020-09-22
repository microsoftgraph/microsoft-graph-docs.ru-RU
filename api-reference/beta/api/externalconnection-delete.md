---
title: Удаление Екстерналконнектион
description: Удаление Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 14bbecb760768a0b2af984b737aaa9e3f1a28e10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006918"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="dac78-103">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="dac78-103">Delete externalConnection</span></span>

<span data-ttu-id="dac78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dac78-105">Удаление [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="dac78-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="dac78-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dac78-106">Permissions</span></span>

<span data-ttu-id="dac78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dac78-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dac78-109">Permission type</span></span>                        | <span data-ttu-id="dac78-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dac78-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dac78-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dac78-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dac78-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dac78-112">Not supported.</span></span> |
| <span data-ttu-id="dac78-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dac78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac78-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dac78-114">Not supported.</span></span> |
| <span data-ttu-id="dac78-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dac78-115">Application</span></span>                            | <span data-ttu-id="dac78-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac78-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac78-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dac78-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dac78-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dac78-118">Request headers</span></span>

| <span data-ttu-id="dac78-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dac78-119">Name</span></span>          | <span data-ttu-id="dac78-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dac78-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dac78-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dac78-121">Authorization</span></span> | <span data-ttu-id="dac78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dac78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dac78-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dac78-124">Request body</span></span>

<span data-ttu-id="dac78-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dac78-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dac78-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac78-126">Response</span></span>

<span data-ttu-id="dac78-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dac78-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dac78-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="dac78-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dac78-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dac78-130">Request</span></span>

<span data-ttu-id="dac78-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dac78-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dac78-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dac78-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="dac78-133">C#</span><span class="sxs-lookup"><span data-stu-id="dac78-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dac78-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dac78-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dac78-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dac78-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="dac78-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac78-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="dac78-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dac78-137">The following is an example of the response.</span></span>

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


