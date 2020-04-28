---
title: Удаление Активитибаседтимеаутполици
description: Удаление Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 19947e753b9444f9efd13061f1faaedbc843d109
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916376"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="86a70-103">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="86a70-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="86a70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a70-105">Удаление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="86a70-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86a70-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86a70-106">Permissions</span></span>

<span data-ttu-id="86a70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86a70-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86a70-109">Permission type</span></span>                        | <span data-ttu-id="86a70-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86a70-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86a70-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86a70-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86a70-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="86a70-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="86a70-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86a70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86a70-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a70-114">Not supported.</span></span> |
| <span data-ttu-id="86a70-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86a70-115">Application</span></span>                            | <span data-ttu-id="86a70-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="86a70-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="86a70-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86a70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="86a70-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86a70-118">Request headers</span></span>

| <span data-ttu-id="86a70-119">Имя</span><span class="sxs-lookup"><span data-stu-id="86a70-119">Name</span></span>          | <span data-ttu-id="86a70-120">Описание</span><span class="sxs-lookup"><span data-stu-id="86a70-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="86a70-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86a70-121">Authorization</span></span> | <span data-ttu-id="86a70-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="86a70-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86a70-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86a70-123">Request body</span></span>

<span data-ttu-id="86a70-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86a70-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86a70-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="86a70-125">Response</span></span>

<span data-ttu-id="86a70-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="86a70-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="86a70-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="86a70-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86a70-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="86a70-128">Request</span></span>

<span data-ttu-id="86a70-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86a70-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86a70-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="86a70-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="86a70-131">C#</span><span class="sxs-lookup"><span data-stu-id="86a70-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86a70-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86a70-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86a70-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86a70-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86a70-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a70-134">Response</span></span>

<span data-ttu-id="86a70-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="86a70-135">The following is an example of the response.</span></span>

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
