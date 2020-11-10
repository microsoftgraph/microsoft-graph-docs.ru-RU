---
title: Получение b2cIdentityUserFlow
description: Получение свойств и связей объекта b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ef6d1b45e1f577a6538998eab74a569ff51125e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961225"
---
# <a name="get-b2cidentityuserflow"></a><span data-ttu-id="3eeae-103">Получение b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3eeae-103">Get b2cIdentityUserFlow</span></span>

<span data-ttu-id="3eeae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eeae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eeae-105">Получение свойств и связей объекта [b2cUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="3eeae-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eeae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3eeae-106">Permissions</span></span>

<span data-ttu-id="3eeae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eeae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eeae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eeae-109">Permission type</span></span>      | <span data-ttu-id="3eeae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eeae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eeae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eeae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3eeae-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3eeae-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3eeae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eeae-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3eeae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eeae-114">Not supported.</span></span>|
|<span data-ttu-id="3eeae-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3eeae-115">Application</span></span>|<span data-ttu-id="3eeae-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3eeae-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3eeae-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3eeae-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3eeae-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3eeae-118">Global administrator</span></span>
* <span data-ttu-id="3eeae-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="3eeae-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3eeae-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eeae-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3eeae-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3eeae-121">Optional query parameters</span></span>

<span data-ttu-id="3eeae-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="3eeae-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="3eeae-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3eeae-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3eeae-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3eeae-124">Request headers</span></span>

|<span data-ttu-id="3eeae-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3eeae-125">Name</span></span>|<span data-ttu-id="3eeae-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3eeae-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3eeae-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3eeae-127">Authorization</span></span>|<span data-ttu-id="3eeae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eeae-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eeae-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eeae-130">Request body</span></span>

<span data-ttu-id="3eeae-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3eeae-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eeae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eeae-132">Response</span></span>

<span data-ttu-id="3eeae-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eeae-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eeae-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3eeae-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eeae-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eeae-135">Request</span></span>

<span data-ttu-id="3eeae-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eeae-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3eeae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3eeae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="3eeae-138">C#</span><span class="sxs-lookup"><span data-stu-id="3eeae-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3eeae-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3eeae-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3eeae-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3eeae-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3eeae-141">Java</span><span class="sxs-lookup"><span data-stu-id="3eeae-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3eeae-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eeae-142">Response</span></span>

<span data-ttu-id="3eeae-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3eeae-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_CustomerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


