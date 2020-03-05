---
title: Удаление Активитибаседтимеаутполици
description: Удаление Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 86e79482d55b4c487f2e344f44de95aa7ed4a26b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441822"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="1e20c-103">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="1e20c-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="1e20c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1e20c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e20c-105">Удаление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1e20c-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e20c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e20c-106">Permissions</span></span>

<span data-ttu-id="1e20c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e20c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e20c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e20c-109">Permission type</span></span>                        | <span data-ttu-id="1e20c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e20c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1e20c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e20c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e20c-112">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1e20c-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1e20c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e20c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e20c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e20c-114">Not supported.</span></span> |
| <span data-ttu-id="1e20c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e20c-115">Application</span></span>                            | <span data-ttu-id="1e20c-116">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1e20c-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e20c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e20c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e20c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e20c-118">Request headers</span></span>

| <span data-ttu-id="1e20c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1e20c-119">Name</span></span>          | <span data-ttu-id="1e20c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1e20c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1e20c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e20c-121">Authorization</span></span> | <span data-ttu-id="1e20c-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1e20c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e20c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e20c-123">Request body</span></span>

<span data-ttu-id="1e20c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e20c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e20c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e20c-125">Response</span></span>

<span data-ttu-id="1e20c-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1e20c-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1e20c-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="1e20c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e20c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e20c-128">Request</span></span>

<span data-ttu-id="1e20c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e20c-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e20c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e20c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="1e20c-131">C#</span><span class="sxs-lookup"><span data-stu-id="1e20c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e20c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e20c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e20c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e20c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e20c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e20c-134">Response</span></span>

<span data-ttu-id="1e20c-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1e20c-135">The following is an example of the response.</span></span>

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
