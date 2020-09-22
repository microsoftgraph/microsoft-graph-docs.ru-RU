---
title: Создание Токенлифетимеполици
description: Создание нового Токенлифетимеполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74040c954d9dc01a398943b566324b909f988aea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062244"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="359db-103">Создание Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="359db-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="359db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="359db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="359db-105">Создание нового объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="359db-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="359db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="359db-106">Permissions</span></span>

<span data-ttu-id="359db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="359db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="359db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="359db-109">Permission type</span></span>                        | <span data-ttu-id="359db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="359db-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="359db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="359db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="359db-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="359db-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="359db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="359db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="359db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="359db-114">Not supported.</span></span> |
| <span data-ttu-id="359db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="359db-115">Application</span></span>                            | <span data-ttu-id="359db-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="359db-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="359db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="359db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="359db-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="359db-118">Request headers</span></span>

| <span data-ttu-id="359db-119">Имя</span><span class="sxs-lookup"><span data-stu-id="359db-119">Name</span></span>          | <span data-ttu-id="359db-120">Описание</span><span class="sxs-lookup"><span data-stu-id="359db-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="359db-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="359db-121">Authorization</span></span> | <span data-ttu-id="359db-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="359db-122">Bearer {token}</span></span> |
| <span data-ttu-id="359db-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="359db-123">Content-type</span></span> | <span data-ttu-id="359db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="359db-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="359db-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="359db-125">Request body</span></span>

<span data-ttu-id="359db-126">В тексте запроса добавьте представление объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="359db-126">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="359db-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="359db-127">Response</span></span>

<span data-ttu-id="359db-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="359db-128">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="359db-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="359db-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="359db-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="359db-130">Request</span></span>

<span data-ttu-id="359db-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="359db-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="359db-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="359db-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="359db-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="359db-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="359db-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="359db-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="359db-135">C#</span><span class="sxs-lookup"><span data-stu-id="359db-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="359db-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="359db-136">Response</span></span>

<span data-ttu-id="359db-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="359db-137">The following is an example of the response.</span></span>

> <span data-ttu-id="359db-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="359db-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


