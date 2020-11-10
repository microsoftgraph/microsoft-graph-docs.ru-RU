---
title: Создание Токениссуанцеполици
description: Создание нового Токениссуанцеполици.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92fca850257f7221bd6f83e8906e6b3af1a7ace7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980260"
---
# <a name="create-tokenissuancepolicy"></a><span data-ttu-id="40087-103">Создание Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="40087-103">Create tokenIssuancePolicy</span></span>

<span data-ttu-id="40087-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40087-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40087-105">Создание нового объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="40087-105">Create a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40087-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40087-106">Permissions</span></span>

<span data-ttu-id="40087-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40087-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40087-109">Permission type</span></span>                        | <span data-ttu-id="40087-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40087-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="40087-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40087-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40087-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="40087-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="40087-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40087-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40087-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40087-114">Not supported.</span></span> |
| <span data-ttu-id="40087-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="40087-115">Application</span></span>                            | <span data-ttu-id="40087-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="40087-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="40087-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40087-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="40087-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40087-118">Request headers</span></span>

| <span data-ttu-id="40087-119">Имя</span><span class="sxs-lookup"><span data-stu-id="40087-119">Name</span></span>          | <span data-ttu-id="40087-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40087-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="40087-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40087-121">Authorization</span></span> | <span data-ttu-id="40087-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40087-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40087-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40087-124">Content-type</span></span> | <span data-ttu-id="40087-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40087-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40087-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40087-127">Request body</span></span>

<span data-ttu-id="40087-128">В тексте запроса добавьте представление объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40087-128">In the request body, supply a JSON representation of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="40087-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="40087-129">Response</span></span>

<span data-ttu-id="40087-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40087-130">If successful, this method returns a `201 Created` response code and a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40087-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="40087-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40087-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="40087-132">Request</span></span>

<span data-ttu-id="40087-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40087-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40087-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="40087-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenIssuancePolicies_from_tokenIssuancePolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="40087-135">C#</span><span class="sxs-lookup"><span data-stu-id="40087-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicies-from-tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40087-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40087-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicies-from-tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40087-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40087-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicies-from-tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40087-138">Java</span><span class="sxs-lookup"><span data-stu-id="40087-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenissuancepolicies-from-tokenissuancepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="40087-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="40087-139">Response</span></span>

<span data-ttu-id="40087-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40087-140">The following is an example of the response.</span></span>

> <span data-ttu-id="40087-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40087-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


