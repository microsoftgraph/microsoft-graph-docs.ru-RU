---
title: Удаление Екстерналконнектион
description: Удаление Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ab69d1c90b0f3e0767c339dd1d0e4b44020ce4b0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869791"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="1a803-103">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="1a803-103">Delete externalConnection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a803-104">Удаление [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="1a803-104">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="1a803-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a803-105">Permissions</span></span>

<span data-ttu-id="1a803-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a803-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a803-108">Permission type</span></span>                        | <span data-ttu-id="1a803-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a803-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a803-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a803-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a803-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a803-111">Not supported.</span></span> |
| <span data-ttu-id="1a803-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a803-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a803-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a803-113">Not supported.</span></span> |
| <span data-ttu-id="1a803-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="1a803-114">Application</span></span>                            | <span data-ttu-id="1a803-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a803-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a803-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a803-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a803-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a803-117">Request headers</span></span>

| <span data-ttu-id="1a803-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1a803-118">Name</span></span>          | <span data-ttu-id="1a803-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1a803-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1a803-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a803-120">Authorization</span></span> | <span data-ttu-id="1a803-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a803-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a803-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a803-123">Request body</span></span>

<span data-ttu-id="1a803-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a803-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a803-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a803-125">Response</span></span>

<span data-ttu-id="1a803-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1a803-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a803-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a803-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a803-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a803-129">Request</span></span>

<span data-ttu-id="1a803-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a803-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a803-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a803-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a803-132">C#</span><span class="sxs-lookup"><span data-stu-id="1a803-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a803-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a803-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a803-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a803-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1a803-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a803-135">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="1a803-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1a803-136">The following is an example of the response.</span></span>

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
