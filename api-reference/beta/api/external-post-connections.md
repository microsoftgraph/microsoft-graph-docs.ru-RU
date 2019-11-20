---
title: Создание подключения
description: Используйте этот API для создания нового Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8dc7ce7bd7a253f0a9696d9987062bc5ceaa7ce6
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747201"
---
# <a name="create-connection"></a><span data-ttu-id="a24b7-103">Создание подключения</span><span class="sxs-lookup"><span data-stu-id="a24b7-103">Create connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a24b7-104">Создание нового [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="a24b7-104">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="a24b7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a24b7-105">Permissions</span></span>

<span data-ttu-id="a24b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a24b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a24b7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a24b7-108">Permission type</span></span>                        | <span data-ttu-id="a24b7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a24b7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a24b7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a24b7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a24b7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24b7-111">Not supported.</span></span> |
| <span data-ttu-id="a24b7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a24b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a24b7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24b7-113">Not supported.</span></span> |
| <span data-ttu-id="a24b7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a24b7-114">Application</span></span>                            | <span data-ttu-id="a24b7-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a24b7-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a24b7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a24b7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="a24b7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a24b7-117">Request headers</span></span>

| <span data-ttu-id="a24b7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a24b7-118">Name</span></span>          | <span data-ttu-id="a24b7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a24b7-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="a24b7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a24b7-120">Authorization</span></span> | <span data-ttu-id="a24b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a24b7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a24b7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a24b7-123">Content-Type</span></span>  | <span data-ttu-id="a24b7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a24b7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a24b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a24b7-126">Request body</span></span>

<span data-ttu-id="a24b7-127">В тексте запроса добавьте представление объекта [екстерналконнектион](../resources/externalconnection.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a24b7-127">In the request body, supply a JSON representation of a [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a24b7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a24b7-128">Response</span></span>

<span data-ttu-id="a24b7-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [екстерналконнектион](../resources/externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a24b7-129">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a24b7-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a24b7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a24b7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a24b7-131">Request</span></span>

<span data-ttu-id="a24b7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a24b7-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a24b7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a24b7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connection_from_external"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a24b7-134">C#</span><span class="sxs-lookup"><span data-stu-id="a24b7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a24b7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a24b7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a24b7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a24b7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="a24b7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a24b7-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="a24b7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a24b7-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
