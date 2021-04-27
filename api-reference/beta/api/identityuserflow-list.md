---
title: Список userFlows
description: Извлечение списка объектов пользовательского потока.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: db3b83e151abb09f443c703eeda03daa8391560e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040709"
---
# <a name="list-userflows"></a><span data-ttu-id="99b16-103">Список userFlows</span><span class="sxs-lookup"><span data-stu-id="99b16-103">List userFlows</span></span>

<span data-ttu-id="99b16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99b16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99b16-105">Извлечение списка [пользовательских процессов.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="99b16-105">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="99b16-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99b16-106">Permissions</span></span>

<span data-ttu-id="99b16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99b16-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99b16-109">Permission type</span></span>                        | <span data-ttu-id="99b16-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99b16-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99b16-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99b16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="99b16-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b16-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="99b16-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99b16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99b16-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99b16-114">Not supported.</span></span> |
| <span data-ttu-id="99b16-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99b16-115">Application</span></span>                            | <span data-ttu-id="99b16-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b16-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99b16-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99b16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="99b16-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99b16-118">Request headers</span></span>

| <span data-ttu-id="99b16-119">Имя</span><span class="sxs-lookup"><span data-stu-id="99b16-119">Name</span></span>      |<span data-ttu-id="99b16-120">Описание</span><span class="sxs-lookup"><span data-stu-id="99b16-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99b16-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99b16-121">Authorization</span></span> | <span data-ttu-id="99b16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99b16-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99b16-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99b16-124">Request body</span></span>

<span data-ttu-id="99b16-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99b16-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99b16-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="99b16-126">Response</span></span>

<span data-ttu-id="99b16-127">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [пользовательского потока](../resources/identityuserflow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="99b16-127">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99b16-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="99b16-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99b16-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="99b16-129">Request</span></span>

<span data-ttu-id="99b16-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99b16-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99b16-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="99b16-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="c"></a>[<span data-ttu-id="99b16-132">C#</span><span class="sxs-lookup"><span data-stu-id="99b16-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99b16-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99b16-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99b16-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99b16-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99b16-135">Java</span><span class="sxs-lookup"><span data-stu-id="99b16-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99b16-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="99b16-136">Response</span></span>

<span data-ttu-id="99b16-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="99b16-137">The following is an example of the response.</span></span>

> <span data-ttu-id="99b16-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="99b16-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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


