---
title: Удаление Екстерналконнектион
description: Удаление Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 809175827de2347d473607fa701647d0db5c9c4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422294"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="89312-103">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="89312-103">Delete externalConnection</span></span>

<span data-ttu-id="89312-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89312-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89312-105">Удаление [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="89312-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="89312-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89312-106">Permissions</span></span>

<span data-ttu-id="89312-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89312-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89312-109">Permission type</span></span>                        | <span data-ttu-id="89312-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89312-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89312-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89312-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89312-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89312-112">Not supported.</span></span> |
| <span data-ttu-id="89312-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89312-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89312-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89312-114">Not supported.</span></span> |
| <span data-ttu-id="89312-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89312-115">Application</span></span>                            | <span data-ttu-id="89312-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89312-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89312-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89312-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89312-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89312-118">Request headers</span></span>

| <span data-ttu-id="89312-119">Имя</span><span class="sxs-lookup"><span data-stu-id="89312-119">Name</span></span>          | <span data-ttu-id="89312-120">Описание</span><span class="sxs-lookup"><span data-stu-id="89312-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="89312-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89312-121">Authorization</span></span> | <span data-ttu-id="89312-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89312-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89312-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89312-124">Request body</span></span>

<span data-ttu-id="89312-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89312-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89312-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="89312-126">Response</span></span>

<span data-ttu-id="89312-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="89312-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89312-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="89312-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89312-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="89312-130">Request</span></span>

<span data-ttu-id="89312-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89312-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89312-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="89312-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="89312-133">C#</span><span class="sxs-lookup"><span data-stu-id="89312-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89312-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89312-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89312-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89312-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="89312-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="89312-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="89312-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="89312-137">The following is an example of the response.</span></span>

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
