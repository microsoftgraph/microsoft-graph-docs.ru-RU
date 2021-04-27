---
title: Убрать tokenIssuancePolicy
description: Удалите маркерIssuancePolicy из приложения.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2dfd8014f276b7a147a1741c85824d2ebbe6bcbf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048150"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="59fff-103">Убрать tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="59fff-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="59fff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59fff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59fff-105">Удалите [маркерIssuancePolicy](../resources/tokenissuancepolicy.md) из [приложения.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="59fff-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="59fff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59fff-106">Permissions</span></span>

<span data-ttu-id="59fff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59fff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59fff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59fff-109">Permission type</span></span>                        | <span data-ttu-id="59fff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59fff-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59fff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59fff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="59fff-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fff-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="59fff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59fff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59fff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59fff-114">Not supported.</span></span> |
| <span data-ttu-id="59fff-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="59fff-115">Application</span></span>                            | <span data-ttu-id="59fff-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fff-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59fff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59fff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="59fff-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59fff-118">Request headers</span></span>

| <span data-ttu-id="59fff-119">Имя</span><span class="sxs-lookup"><span data-stu-id="59fff-119">Name</span></span>          | <span data-ttu-id="59fff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59fff-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="59fff-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59fff-121">Authorization</span></span> | <span data-ttu-id="59fff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59fff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59fff-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59fff-124">Request body</span></span>

<span data-ttu-id="59fff-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59fff-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59fff-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="59fff-126">Response</span></span>

<span data-ttu-id="59fff-127">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="59fff-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="59fff-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="59fff-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59fff-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="59fff-129">Request</span></span>

<span data-ttu-id="59fff-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59fff-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="59fff-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="59fff-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="59fff-132">C#</span><span class="sxs-lookup"><span data-stu-id="59fff-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59fff-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59fff-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59fff-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59fff-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59fff-135">Java</span><span class="sxs-lookup"><span data-stu-id="59fff-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenissuancepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59fff-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="59fff-136">Response</span></span>

<span data-ttu-id="59fff-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="59fff-137">The following is an example of the response.</span></span>

> <span data-ttu-id="59fff-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59fff-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



