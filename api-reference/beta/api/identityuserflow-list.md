---
title: Список userFlows
description: Извлечение списка объектов пользовательского потока.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7c60d86c6baa2b18b3957872f81b2069683ea237
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435310"
---
# <a name="list-userflows"></a><span data-ttu-id="e9dfc-103">Список userFlows</span><span class="sxs-lookup"><span data-stu-id="e9dfc-103">List userFlows</span></span>

<span data-ttu-id="e9dfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9dfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9dfc-105">Извлечение списка [пользовательских процессов.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e9dfc-105">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9dfc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9dfc-106">Permissions</span></span>

<span data-ttu-id="e9dfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9dfc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9dfc-109">Permission type</span></span>                        | <span data-ttu-id="e9dfc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9dfc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9dfc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9dfc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9dfc-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dfc-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="e9dfc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9dfc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9dfc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-114">Not supported.</span></span> |
| <span data-ttu-id="e9dfc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e9dfc-115">Application</span></span>                            | <span data-ttu-id="e9dfc-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dfc-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9dfc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9dfc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="e9dfc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9dfc-118">Request headers</span></span>

| <span data-ttu-id="e9dfc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e9dfc-119">Name</span></span>      |<span data-ttu-id="e9dfc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e9dfc-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9dfc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9dfc-121">Authorization</span></span> | <span data-ttu-id="e9dfc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9dfc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9dfc-124">Request body</span></span>

<span data-ttu-id="e9dfc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9dfc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9dfc-126">Response</span></span>

<span data-ttu-id="e9dfc-127">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [пользовательского потока](../resources/identityuserflow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-127">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9dfc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9dfc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9dfc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9dfc-129">Request</span></span>

<span data-ttu-id="e9dfc-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9dfc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9dfc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="c"></a>[<span data-ttu-id="e9dfc-132">C#</span><span class="sxs-lookup"><span data-stu-id="e9dfc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9dfc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9dfc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9dfc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9dfc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9dfc-135">Java</span><span class="sxs-lookup"><span data-stu-id="e9dfc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9dfc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9dfc-136">Response</span></span>

<span data-ttu-id="e9dfc-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e9dfc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9dfc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


