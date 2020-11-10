---
title: Удаление Акцесспаккажекаталог
description: Удаление Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75889298f67ca7e751ef400d13902b588afafa04
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951996"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="8aca0-103">Удаление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="8aca0-103">Delete accessPackageCatalog</span></span>

<span data-ttu-id="8aca0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aca0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aca0-105">Удаление [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="8aca0-105">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8aca0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aca0-106">Permissions</span></span>

<span data-ttu-id="8aca0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8aca0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aca0-109">Permission type</span></span>                        | <span data-ttu-id="8aca0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8aca0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8aca0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aca0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8aca0-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aca0-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8aca0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aca0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aca0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aca0-114">Not supported.</span></span> |
| <span data-ttu-id="8aca0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8aca0-115">Application</span></span>                            | <span data-ttu-id="8aca0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aca0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aca0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aca0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8aca0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aca0-118">Request headers</span></span>

| <span data-ttu-id="8aca0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8aca0-119">Name</span></span>          | <span data-ttu-id="8aca0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8aca0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8aca0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8aca0-121">Authorization</span></span> | <span data-ttu-id="8aca0-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="8aca0-122">Bearer \{token\}.</span></span> <span data-ttu-id="8aca0-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8aca0-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aca0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8aca0-124">Request body</span></span>

<span data-ttu-id="8aca0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8aca0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aca0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aca0-126">Response</span></span>

<span data-ttu-id="8aca0-127">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="8aca0-127">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="8aca0-128">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8aca0-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aca0-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8aca0-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aca0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aca0-130">Request</span></span>

<span data-ttu-id="8aca0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8aca0-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8aca0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aca0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="8aca0-133">C#</span><span class="sxs-lookup"><span data-stu-id="8aca0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8aca0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8aca0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8aca0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aca0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8aca0-136">Java</span><span class="sxs-lookup"><span data-stu-id="8aca0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8aca0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aca0-137">Response</span></span>

<span data-ttu-id="8aca0-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8aca0-138">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


