---
title: Получение b2xUserFlows
description: Получение свойств и связей объекта b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f96fef3b8e18e82e50609eabeecd6309129beb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991399"
---
# <a name="get-b2xuserflow"></a><span data-ttu-id="0b06d-103">Получение b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="0b06d-103">Get b2xUserFlow</span></span>

<span data-ttu-id="0b06d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b06d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b06d-105">Получение свойств и связей объекта [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="0b06d-105">Retrieve the properties and relationships of a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b06d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b06d-106">Permissions</span></span>

<span data-ttu-id="0b06d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b06d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b06d-109">Permission type</span></span>      | <span data-ttu-id="0b06d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b06d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b06d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b06d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b06d-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b06d-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0b06d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b06d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0b06d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b06d-114">Not supported.</span></span>|
|<span data-ttu-id="0b06d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b06d-115">Application</span></span>|<span data-ttu-id="0b06d-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b06d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0b06d-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0b06d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0b06d-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0b06d-118">Global administrator</span></span>
* <span data-ttu-id="0b06d-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="0b06d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0b06d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b06d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b06d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b06d-121">Optional query parameters</span></span>

<span data-ttu-id="0b06d-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="0b06d-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="0b06d-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0b06d-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b06d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b06d-124">Request headers</span></span>

|<span data-ttu-id="0b06d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0b06d-125">Name</span></span>|<span data-ttu-id="0b06d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0b06d-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0b06d-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b06d-127">Authorization</span></span>|<span data-ttu-id="0b06d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b06d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b06d-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b06d-130">Request body</span></span>

<span data-ttu-id="0b06d-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b06d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b06d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b06d-132">Response</span></span>

<span data-ttu-id="0b06d-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [усерфловаттрибуте](../resources/b2xuserflows.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b06d-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [userFlowAttribute](../resources/b2xuserflows.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b06d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0b06d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b06d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b06d-135">Request</span></span>

<span data-ttu-id="0b06d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b06d-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b06d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b06d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b06d-138">C#</span><span class="sxs-lookup"><span data-stu-id="0b06d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b06d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b06d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b06d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b06d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b06d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b06d-141">Response</span></span>

<span data-ttu-id="0b06d-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0b06d-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2X_1_PartnerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


