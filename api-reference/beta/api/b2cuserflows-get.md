---
title: Получение b2cUserFlows
description: Получение свойств и связей объекта b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5002a13c69f1791a3ba0b5b24030a47dc0d4b4d7
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329764"
---
# <a name="get-b2cuserflow"></a><span data-ttu-id="f55bd-103">Получение b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="f55bd-103">Get b2cUserFlow</span></span>

<span data-ttu-id="f55bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f55bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f55bd-105">Получение свойств и связей объекта [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="f55bd-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f55bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f55bd-106">Permissions</span></span>

<span data-ttu-id="f55bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f55bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f55bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f55bd-109">Permission type</span></span>      | <span data-ttu-id="f55bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f55bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f55bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f55bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f55bd-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f55bd-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f55bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f55bd-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f55bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f55bd-114">Not supported.</span></span>|
|<span data-ttu-id="f55bd-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f55bd-115">Application</span></span>|<span data-ttu-id="f55bd-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f55bd-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f55bd-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f55bd-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f55bd-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f55bd-118">Global administrator</span></span>
* <span data-ttu-id="f55bd-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="f55bd-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f55bd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f55bd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f55bd-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f55bd-121">Optional query parameters</span></span>

<span data-ttu-id="f55bd-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="f55bd-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="f55bd-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f55bd-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f55bd-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f55bd-124">Request headers</span></span>

|<span data-ttu-id="f55bd-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f55bd-125">Name</span></span>|<span data-ttu-id="f55bd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f55bd-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f55bd-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f55bd-127">Authorization</span></span>|<span data-ttu-id="f55bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f55bd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f55bd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f55bd-130">Request body</span></span>

<span data-ttu-id="f55bd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f55bd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f55bd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f55bd-132">Response</span></span>

<span data-ttu-id="f55bd-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [b2cUserFlow](../resources/b2cuserflows.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f55bd-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cUserFlow](../resources/b2cuserflows.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f55bd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f55bd-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f55bd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f55bd-135">Request</span></span>

<span data-ttu-id="f55bd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f55bd-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f55bd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f55bd-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="f55bd-138">C#</span><span class="sxs-lookup"><span data-stu-id="f55bd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f55bd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f55bd-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f55bd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f55bd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f55bd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f55bd-141">Response</span></span>

<span data-ttu-id="f55bd-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f55bd-142">The following is an example of the response.</span></span>

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
