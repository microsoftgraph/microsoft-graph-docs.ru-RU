---
title: Получение b2xIdentityUserFlow
description: Получение свойств и связей объекта b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 164e289bc61dbedc233a9f7270cd6450a53ed9ac
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406367"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="5ca01-103">Получение b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="5ca01-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="5ca01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ca01-105">Получение свойств и связей объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="5ca01-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ca01-106">Permissions</span></span>

<span data-ttu-id="5ca01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ca01-109">Permission type</span></span>      | <span data-ttu-id="5ca01-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ca01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ca01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ca01-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5ca01-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5ca01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ca01-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5ca01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ca01-114">Not supported.</span></span>|
|<span data-ttu-id="5ca01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ca01-115">Application</span></span>|<span data-ttu-id="5ca01-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5ca01-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5ca01-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="5ca01-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5ca01-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5ca01-118">Global administrator</span></span>
* <span data-ttu-id="5ca01-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="5ca01-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5ca01-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ca01-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ca01-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ca01-121">Optional query parameters</span></span>

<span data-ttu-id="5ca01-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="5ca01-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="5ca01-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5ca01-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ca01-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ca01-124">Request headers</span></span>

|<span data-ttu-id="5ca01-125">Имя</span><span class="sxs-lookup"><span data-stu-id="5ca01-125">Name</span></span>|<span data-ttu-id="5ca01-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5ca01-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5ca01-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ca01-127">Authorization</span></span>|<span data-ttu-id="5ca01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ca01-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ca01-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ca01-130">Request body</span></span>

<span data-ttu-id="5ca01-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ca01-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca01-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ca01-132">Response</span></span>

<span data-ttu-id="5ca01-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ca01-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca01-134">Пример</span><span class="sxs-lookup"><span data-stu-id="5ca01-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ca01-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ca01-135">Request</span></span>

<span data-ttu-id="5ca01-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ca01-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ca01-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca01-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="5ca01-138">C#</span><span class="sxs-lookup"><span data-stu-id="5ca01-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ca01-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ca01-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ca01-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ca01-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ca01-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ca01-141">Response</span></span>

<span data-ttu-id="5ca01-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5ca01-142">The following is an example of the response.</span></span>

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


