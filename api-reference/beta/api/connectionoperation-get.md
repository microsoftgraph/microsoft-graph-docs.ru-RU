---
title: Получение Коннектионоператион
description: Получение свойств объекта Коннектионоператион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e7dca8677b935fb7a5ed83a647815ed435d1e82c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437807"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="94276-103">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="94276-103">Get connectionOperation</span></span>

<span data-ttu-id="94276-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94276-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94276-105">Получение свойств объекта [коннектионоператион](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="94276-105">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="94276-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94276-106">Permissions</span></span>

<span data-ttu-id="94276-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94276-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94276-109">Permission type</span></span>                        | <span data-ttu-id="94276-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94276-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94276-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94276-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94276-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94276-112">Not supported.</span></span> |
| <span data-ttu-id="94276-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94276-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94276-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94276-114">Not supported.</span></span> |
| <span data-ttu-id="94276-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94276-115">Application</span></span>                            | <span data-ttu-id="94276-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94276-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94276-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94276-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="94276-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94276-118">Request headers</span></span>

| <span data-ttu-id="94276-119">Имя</span><span class="sxs-lookup"><span data-stu-id="94276-119">Name</span></span>          | <span data-ttu-id="94276-120">Описание</span><span class="sxs-lookup"><span data-stu-id="94276-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="94276-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94276-121">Authorization</span></span> | <span data-ttu-id="94276-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94276-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94276-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="94276-124">Request body</span></span>

<span data-ttu-id="94276-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94276-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94276-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="94276-126">Response</span></span>

<span data-ttu-id="94276-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [коннектионоператион](../resources/connectionoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94276-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94276-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="94276-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94276-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="94276-129">Request</span></span>

<span data-ttu-id="94276-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94276-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94276-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="94276-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="94276-132">C#</span><span class="sxs-lookup"><span data-stu-id="94276-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94276-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94276-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94276-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94276-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="94276-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="94276-135">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="94276-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94276-136">The following is an example of the response.</span></span>

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
