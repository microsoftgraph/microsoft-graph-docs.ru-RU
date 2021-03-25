---
title: Удаление featureRolloutPolicy
description: Удаление объекта featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b06a82259d2bd0694cf8bf66807a8625d3b1b84
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201377"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="961be-103">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="961be-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="961be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="961be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="961be-105">Удаление [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="961be-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="961be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="961be-106">Permissions</span></span>

<span data-ttu-id="961be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="961be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="961be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="961be-109">Permission type</span></span>                        | <span data-ttu-id="961be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="961be-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="961be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="961be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="961be-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="961be-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="961be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="961be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="961be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="961be-114">Not supported.</span></span> |
| <span data-ttu-id="961be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="961be-115">Application</span></span>                            | <span data-ttu-id="961be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="961be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="961be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="961be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="961be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="961be-118">Request headers</span></span>

| <span data-ttu-id="961be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="961be-119">Name</span></span>          | <span data-ttu-id="961be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="961be-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="961be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="961be-121">Authorization</span></span> | <span data-ttu-id="961be-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="961be-122">Bearer {token}.</span></span> <span data-ttu-id="961be-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="961be-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="961be-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="961be-124">Request body</span></span>

<span data-ttu-id="961be-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="961be-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="961be-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="961be-126">Response</span></span>

<span data-ttu-id="961be-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="961be-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="961be-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="961be-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="961be-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="961be-130">Request</span></span>

<span data-ttu-id="961be-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="961be-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="961be-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="961be-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="961be-133">C#</span><span class="sxs-lookup"><span data-stu-id="961be-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="961be-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="961be-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="961be-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="961be-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="961be-136">Java</span><span class="sxs-lookup"><span data-stu-id="961be-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="961be-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="961be-137">Response</span></span>

<span data-ttu-id="961be-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="961be-138">The following is an example of the response.</span></span>

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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


