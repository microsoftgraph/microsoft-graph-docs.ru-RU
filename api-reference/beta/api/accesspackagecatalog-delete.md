---
title: Удаление accessPackageCatalog
description: Удаление accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ad2dd60c9e2f104987edeef0bac46dcf940a14cd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439606"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="6bbe6-103">Удаление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="6bbe6-103">Delete accessPackageCatalog</span></span>

<span data-ttu-id="6bbe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bbe6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bbe6-105">Удаление [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="6bbe6-105">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bbe6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bbe6-106">Permissions</span></span>

<span data-ttu-id="6bbe6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bbe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bbe6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bbe6-109">Permission type</span></span>                        | <span data-ttu-id="6bbe6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bbe6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6bbe6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bbe6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bbe6-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bbe6-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6bbe6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bbe6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bbe6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-114">Not supported.</span></span> |
| <span data-ttu-id="6bbe6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6bbe6-115">Application</span></span>                            | <span data-ttu-id="6bbe6-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bbe6-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bbe6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bbe6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6bbe6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bbe6-118">Request headers</span></span>

| <span data-ttu-id="6bbe6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6bbe6-119">Name</span></span>          | <span data-ttu-id="6bbe6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6bbe6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6bbe6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bbe6-121">Authorization</span></span> | <span data-ttu-id="6bbe6-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-122">Bearer \{token\}.</span></span> <span data-ttu-id="6bbe6-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bbe6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bbe6-124">Request body</span></span>

<span data-ttu-id="6bbe6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bbe6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bbe6-126">Response</span></span>

<span data-ttu-id="6bbe6-127">В случае успешной работы этот метод возвращает код ответа из 200 серий.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-127">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="6bbe6-128">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bbe6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6bbe6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6bbe6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bbe6-130">Request</span></span>

<span data-ttu-id="6bbe6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6bbe6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bbe6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="6bbe6-133">C#</span><span class="sxs-lookup"><span data-stu-id="6bbe6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bbe6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bbe6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bbe6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bbe6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bbe6-136">Java</span><span class="sxs-lookup"><span data-stu-id="6bbe6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bbe6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bbe6-137">Response</span></span>

<span data-ttu-id="6bbe6-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6bbe6-138">The following is an example of the response.</span></span>

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


