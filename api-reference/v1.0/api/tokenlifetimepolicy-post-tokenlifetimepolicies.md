---
title: Создание tokenLifetimePolicy
description: Создайте новый tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 466290d323d7bc7d64baaf72838b4c2e4f29dac6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439984"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="6cb96-103">Создание tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="6cb96-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="6cb96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb96-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6cb96-105">Создайте новый [объект tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6cb96-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cb96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb96-106">Permissions</span></span>

<span data-ttu-id="6cb96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cb96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb96-109">Permission type</span></span>                        | <span data-ttu-id="6cb96-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cb96-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6cb96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cb96-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cb96-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cb96-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6cb96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cb96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb96-114">Not supported.</span></span> |
| <span data-ttu-id="6cb96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cb96-115">Application</span></span>                            | <span data-ttu-id="6cb96-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cb96-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cb96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cb96-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6cb96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cb96-118">Request headers</span></span>

| <span data-ttu-id="6cb96-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6cb96-119">Name</span></span>          | <span data-ttu-id="6cb96-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6cb96-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6cb96-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cb96-121">Authorization</span></span> | <span data-ttu-id="6cb96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cb96-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cb96-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cb96-124">Content-type</span></span> | <span data-ttu-id="6cb96-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cb96-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cb96-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cb96-127">Request body</span></span>

<span data-ttu-id="6cb96-128">В теле запроса поставляем JSON-представление [объекта tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6cb96-128">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6cb96-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cb96-129">Response</span></span>

<span data-ttu-id="6cb96-130">В случае успешной работы этот метод возвращает код отклика и `201 Created` новый [объект tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6cb96-130">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cb96-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6cb96-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6cb96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cb96-132">Request</span></span>

<span data-ttu-id="6cb96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cb96-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6cb96-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb96-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="6cb96-135">C#</span><span class="sxs-lookup"><span data-stu-id="6cb96-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cb96-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cb96-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cb96-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cb96-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cb96-138">Java</span><span class="sxs-lookup"><span data-stu-id="6cb96-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6cb96-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cb96-139">Response</span></span>

<span data-ttu-id="6cb96-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6cb96-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6cb96-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cb96-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

