---
title: Удаление activityBasedTimeoutPolicy
description: Удаление activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a541d32fe57a2734b9e744c6c306a656c3a9fe46
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442637"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="f1491-103">Удаление activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="f1491-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="f1491-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1491-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f1491-105">Удаление [объекта activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f1491-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1491-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1491-106">Permissions</span></span>

<span data-ttu-id="f1491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1491-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1491-109">Permission type</span></span>                        | <span data-ttu-id="f1491-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1491-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1491-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1491-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1491-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1491-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f1491-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1491-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1491-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1491-114">Not supported.</span></span> |
| <span data-ttu-id="f1491-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1491-115">Application</span></span>                            | <span data-ttu-id="f1491-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1491-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1491-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1491-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1491-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1491-118">Request headers</span></span>

| <span data-ttu-id="f1491-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1491-119">Name</span></span>          | <span data-ttu-id="f1491-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f1491-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1491-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1491-121">Authorization</span></span> | <span data-ttu-id="f1491-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1491-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1491-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1491-124">Request body</span></span>

<span data-ttu-id="f1491-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1491-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1491-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1491-126">Response</span></span>

<span data-ttu-id="f1491-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1491-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f1491-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1491-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1491-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1491-129">Request</span></span>

<span data-ttu-id="f1491-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1491-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f1491-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1491-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="f1491-132">C#</span><span class="sxs-lookup"><span data-stu-id="f1491-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1491-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1491-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1491-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1491-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1491-135">Java</span><span class="sxs-lookup"><span data-stu-id="f1491-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1491-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1491-136">Response</span></span>

<span data-ttu-id="f1491-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f1491-137">The following is an example of the response.</span></span>

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

