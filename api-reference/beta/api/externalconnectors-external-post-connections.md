---
title: Создание подключения
description: Используйте этот API для создания нового externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c4415c33e759bde7a95eb37ec6254762a925058e
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467709"
---
# <a name="create-connection"></a><span data-ttu-id="dde1b-103">Создание подключения</span><span class="sxs-lookup"><span data-stu-id="dde1b-103">Create connection</span></span>

<span data-ttu-id="dde1b-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="dde1b-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dde1b-105">Создание нового [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="dde1b-105">Create a new [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dde1b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dde1b-106">Permissions</span></span>

<span data-ttu-id="dde1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dde1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dde1b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dde1b-109">Permission type</span></span>                        | <span data-ttu-id="dde1b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dde1b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dde1b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dde1b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dde1b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dde1b-112">Not supported.</span></span> |
| <span data-ttu-id="dde1b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dde1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dde1b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dde1b-114">Not supported.</span></span> |
| <span data-ttu-id="dde1b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dde1b-115">Application</span></span>                            | <span data-ttu-id="dde1b-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="dde1b-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="dde1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dde1b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="dde1b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dde1b-118">Request headers</span></span>

| <span data-ttu-id="dde1b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dde1b-119">Name</span></span>          | <span data-ttu-id="dde1b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dde1b-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="dde1b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dde1b-121">Authorization</span></span> | <span data-ttu-id="dde1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dde1b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dde1b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dde1b-124">Content-Type</span></span>  | <span data-ttu-id="dde1b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dde1b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dde1b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dde1b-127">Request body</span></span>

<span data-ttu-id="dde1b-128">В теле запроса поставляем представление JSON объекта [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="dde1b-128">In the request body, supply a JSON representation of an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dde1b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dde1b-129">Response</span></span>

<span data-ttu-id="dde1b-130">В случае успеха этот метод возвращает код отклика и `201 Created` новый объект [externalConnection](../resources/externalconnectors-externalconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dde1b-130">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dde1b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="dde1b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dde1b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dde1b-132">Request</span></span>

<span data-ttu-id="dde1b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dde1b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dde1b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dde1b-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dde1b-135">C#</span><span class="sxs-lookup"><span data-stu-id="dde1b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dde1b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dde1b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dde1b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dde1b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dde1b-138">Java</span><span class="sxs-lookup"><span data-stu-id="dde1b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connection-from-external-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="dde1b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dde1b-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="dde1b-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dde1b-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "state": "draft",
  "configuration": {
    "authorizedAppIds": [
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


