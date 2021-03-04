---
title: Get userFlow
description: Извлечение свойств и связей объекта пользовательского потока.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 143b86109eb0f7cfd14d3366a66fd712f6406262
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435324"
---
# <a name="get-userflow"></a><span data-ttu-id="f7a86-103">Get userFlow</span><span class="sxs-lookup"><span data-stu-id="f7a86-103">Get userFlow</span></span>

<span data-ttu-id="f7a86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7a86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7a86-105">Извлечение свойств и ассоциаций для [объекта userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f7a86-105">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7a86-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7a86-106">Permissions</span></span>

<span data-ttu-id="f7a86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7a86-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7a86-109">Permission type</span></span>                        | <span data-ttu-id="f7a86-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7a86-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7a86-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7a86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7a86-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7a86-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="f7a86-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7a86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7a86-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7a86-114">Not supported.</span></span> |
| <span data-ttu-id="f7a86-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f7a86-115">Application</span></span>                            | <span data-ttu-id="f7a86-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7a86-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7a86-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7a86-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7a86-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7a86-118">Request headers</span></span>

| <span data-ttu-id="f7a86-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f7a86-119">Name</span></span>      |<span data-ttu-id="f7a86-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a86-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7a86-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7a86-121">Authorization</span></span> | <span data-ttu-id="f7a86-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7a86-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7a86-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7a86-124">Content-type</span></span> | <span data-ttu-id="f7a86-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7a86-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7a86-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7a86-127">Request body</span></span>

<span data-ttu-id="f7a86-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7a86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7a86-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7a86-129">Response</span></span>

<span data-ttu-id="f7a86-130">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [пользовательского потока](../resources/identityuserflow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f7a86-130">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7a86-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7a86-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7a86-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7a86-132">Request</span></span>

<span data-ttu-id="f7a86-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7a86-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7a86-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7a86-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="c"></a>[<span data-ttu-id="f7a86-135">C#</span><span class="sxs-lookup"><span data-stu-id="f7a86-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7a86-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7a86-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7a86-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7a86-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7a86-138">Java</span><span class="sxs-lookup"><span data-stu-id="f7a86-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7a86-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7a86-139">Response</span></span>

<span data-ttu-id="f7a86-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7a86-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f7a86-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7a86-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
   "suppressions": [
    "Error: get_identityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


