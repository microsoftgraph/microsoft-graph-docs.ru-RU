---
title: Удаление conditionalAccessPolicy
description: Удаление conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 71a084f2c79db27a6f6418cddbbecd1835a8f5c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437627"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="53b34-103">Удаление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="53b34-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="53b34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b34-105">Удаление [объекта conditionalAccessPolicy.](../resources/conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53b34-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b34-106">Permissions</span></span>

<span data-ttu-id="53b34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b34-109">Permission type</span></span>                        | <span data-ttu-id="53b34-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b34-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="53b34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b34-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53b34-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="53b34-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="53b34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b34-114">Not supported.</span></span> |
|<span data-ttu-id="53b34-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="53b34-115">Application</span></span>                            | <span data-ttu-id="53b34-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="53b34-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="53b34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b34-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53b34-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53b34-118">Request headers</span></span>

| <span data-ttu-id="53b34-119">Имя</span><span class="sxs-lookup"><span data-stu-id="53b34-119">Name</span></span>          | <span data-ttu-id="53b34-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53b34-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53b34-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53b34-121">Authorization</span></span> | <span data-ttu-id="53b34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b34-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53b34-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53b34-124">Request body</span></span>

<span data-ttu-id="53b34-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53b34-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53b34-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b34-126">Response</span></span>

<span data-ttu-id="53b34-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53b34-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53b34-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="53b34-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53b34-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="53b34-130">Request</span></span>

<span data-ttu-id="53b34-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53b34-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53b34-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b34-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="53b34-133">C#</span><span class="sxs-lookup"><span data-stu-id="53b34-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53b34-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b34-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53b34-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b34-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53b34-136">Java</span><span class="sxs-lookup"><span data-stu-id="53b34-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conditionalaccesspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53b34-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b34-137">Response</span></span>

<span data-ttu-id="53b34-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53b34-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


