---
title: Убрать tokenIssuancePolicy
description: Удаление Токениссуанцеполици из приложения.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb1999c23f16802f71ff7f823b31d352068c1b8f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996971"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="633b1-103">Убрать tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="633b1-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="633b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="633b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="633b1-105">Удаление [токениссуанцеполици](../resources/tokenissuancepolicy.md) из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="633b1-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="633b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="633b1-106">Permissions</span></span>

<span data-ttu-id="633b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="633b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="633b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="633b1-109">Permission type</span></span>                        | <span data-ttu-id="633b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="633b1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="633b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="633b1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="633b1-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="633b1-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="633b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="633b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="633b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="633b1-114">Not supported.</span></span> |
| <span data-ttu-id="633b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="633b1-115">Application</span></span>                            | <span data-ttu-id="633b1-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="633b1-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="633b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="633b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="633b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="633b1-118">Request headers</span></span>

| <span data-ttu-id="633b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="633b1-119">Name</span></span>          | <span data-ttu-id="633b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="633b1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="633b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="633b1-121">Authorization</span></span> | <span data-ttu-id="633b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="633b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="633b1-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="633b1-124">Request body</span></span>

<span data-ttu-id="633b1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="633b1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="633b1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="633b1-126">Response</span></span>

<span data-ttu-id="633b1-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="633b1-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="633b1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="633b1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="633b1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="633b1-129">Request</span></span>

<span data-ttu-id="633b1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="633b1-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="633b1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="633b1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="633b1-132">C#</span><span class="sxs-lookup"><span data-stu-id="633b1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="633b1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="633b1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="633b1-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="633b1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="633b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="633b1-135">Response</span></span>

<span data-ttu-id="633b1-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="633b1-136">The following is an example of the response.</span></span>

> <span data-ttu-id="633b1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="633b1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


