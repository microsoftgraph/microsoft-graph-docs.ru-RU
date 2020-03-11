---
title: Создание Токениссуанцеполици
description: Создание нового Токениссуанцеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e02230ff52f7e9969d653f65f885de6b782c3f46
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591630"
---
# <a name="create-tokenissuancepolicy"></a><span data-ttu-id="f1a95-103">Создание Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="f1a95-103">Create tokenIssuancePolicy</span></span>

<span data-ttu-id="f1a95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1a95-105">Создание нового объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f1a95-105">Create a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a95-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a95-106">Permissions</span></span>

<span data-ttu-id="f1a95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1a95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a95-109">Permission type</span></span>                        | <span data-ttu-id="f1a95-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a95-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1a95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a95-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1a95-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1a95-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f1a95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a95-114">Not supported.</span></span> |
| <span data-ttu-id="f1a95-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a95-115">Application</span></span>                            | <span data-ttu-id="f1a95-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1a95-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a95-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a95-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f1a95-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1a95-118">Request headers</span></span>

| <span data-ttu-id="f1a95-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1a95-119">Name</span></span>          | <span data-ttu-id="f1a95-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a95-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1a95-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a95-121">Authorization</span></span> | <span data-ttu-id="f1a95-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a95-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1a95-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1a95-124">Content-type</span></span> | <span data-ttu-id="f1a95-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a95-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a95-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1a95-127">Request body</span></span>

<span data-ttu-id="f1a95-128">В тексте запроса добавьте представление объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1a95-128">In the request body, supply a JSON representation of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f1a95-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a95-129">Response</span></span>

<span data-ttu-id="f1a95-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a95-130">If successful, this method returns a `201 Created` response code and a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1a95-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1a95-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1a95-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a95-132">Request</span></span>

<span data-ttu-id="f1a95-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a95-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1a95-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a95-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f1a95-135">C#</span><span class="sxs-lookup"><span data-stu-id="f1a95-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicies-from-tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a95-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a95-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicies-from-tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1a95-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1a95-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicies-from-tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="f1a95-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a95-138">Response</span></span>

<span data-ttu-id="f1a95-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a95-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f1a95-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a95-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
