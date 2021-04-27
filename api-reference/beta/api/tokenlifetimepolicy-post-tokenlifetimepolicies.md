---
title: Создание tokenLifetimePolicy
description: Создайте новый tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d14b289f640c7ab2ca0b7e335d6f7b87c22eb536
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051762"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="9be37-103">Создание tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="9be37-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="9be37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be37-105">Создайте новый [объект tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9be37-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9be37-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9be37-106">Permissions</span></span>

<span data-ttu-id="9be37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9be37-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9be37-109">Permission type</span></span>                        | <span data-ttu-id="9be37-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9be37-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9be37-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9be37-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be37-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="9be37-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="9be37-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9be37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be37-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9be37-114">Not supported.</span></span> |
| <span data-ttu-id="9be37-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9be37-115">Application</span></span>                            | <span data-ttu-id="9be37-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="9be37-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="9be37-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9be37-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9be37-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9be37-118">Request headers</span></span>

| <span data-ttu-id="9be37-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9be37-119">Name</span></span>          | <span data-ttu-id="9be37-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9be37-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9be37-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9be37-121">Authorization</span></span> | <span data-ttu-id="9be37-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9be37-122">Bearer {token}</span></span> |
| <span data-ttu-id="9be37-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9be37-123">Content-type</span></span> | <span data-ttu-id="9be37-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9be37-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9be37-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9be37-125">Request body</span></span>

<span data-ttu-id="9be37-126">В теле запроса поставляем JSON-представление [объекта tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9be37-126">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9be37-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9be37-127">Response</span></span>

<span data-ttu-id="9be37-128">В случае успешной работы этот метод возвращает код отклика и `201 Created` новый [объект tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9be37-128">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9be37-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="9be37-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9be37-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9be37-130">Request</span></span>

<span data-ttu-id="9be37-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9be37-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9be37-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be37-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9be37-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9be37-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9be37-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9be37-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9be37-135">C#</span><span class="sxs-lookup"><span data-stu-id="9be37-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9be37-136">Java</span><span class="sxs-lookup"><span data-stu-id="9be37-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9be37-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9be37-137">Response</span></span>

<span data-ttu-id="9be37-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9be37-138">The following is an example of the response.</span></span>

> <span data-ttu-id="9be37-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9be37-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


