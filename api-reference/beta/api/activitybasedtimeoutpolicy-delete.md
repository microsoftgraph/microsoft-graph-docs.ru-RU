---
title: Удаление Активитибаседтимеаутполици
description: Удаление Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8a8bcd348bf3df72609da431c2ff92aecc1d705f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983447"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="ed4a8-103">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="ed4a8-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="ed4a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed4a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed4a8-105">Удаление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ed4a8-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed4a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed4a8-106">Permissions</span></span>

<span data-ttu-id="ed4a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed4a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed4a8-109">Permission type</span></span>                        | <span data-ttu-id="ed4a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed4a8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed4a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed4a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed4a8-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed4a8-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ed4a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed4a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed4a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed4a8-114">Not supported.</span></span> |
| <span data-ttu-id="ed4a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed4a8-115">Application</span></span>                            | <span data-ttu-id="ed4a8-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed4a8-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed4a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed4a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed4a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed4a8-118">Request headers</span></span>

| <span data-ttu-id="ed4a8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ed4a8-119">Name</span></span>          | <span data-ttu-id="ed4a8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ed4a8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ed4a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed4a8-121">Authorization</span></span> | <span data-ttu-id="ed4a8-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ed4a8-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed4a8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed4a8-123">Request body</span></span>

<span data-ttu-id="ed4a8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed4a8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed4a8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed4a8-125">Response</span></span>

<span data-ttu-id="ed4a8-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed4a8-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ed4a8-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed4a8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed4a8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed4a8-128">Request</span></span>

<span data-ttu-id="ed4a8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed4a8-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed4a8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed4a8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="ed4a8-131">C#</span><span class="sxs-lookup"><span data-stu-id="ed4a8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed4a8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed4a8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed4a8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed4a8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed4a8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed4a8-134">Response</span></span>

<span data-ttu-id="ed4a8-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ed4a8-135">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


