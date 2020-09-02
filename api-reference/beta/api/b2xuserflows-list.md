---
title: Список b2xUserFlows
description: Получение списка объектов b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 135ce0d335be077e5673c39979f1fa198f97b440
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329468"
---
# <a name="list-b2xuserflows"></a><span data-ttu-id="9a7ec-103">Список b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="9a7ec-103">List b2xUserFlows</span></span>

<span data-ttu-id="9a7ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a7ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a7ec-105">Получение списка объектов [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="9a7ec-105">Retrieve a list of [b2xUserFlow](../resources/b2xuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a7ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a7ec-106">Permissions</span></span>

<span data-ttu-id="9a7ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a7ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a7ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a7ec-109">Permission type</span></span>      | <span data-ttu-id="9a7ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a7ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a7ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a7ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a7ec-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9a7ec-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9a7ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a7ec-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9a7ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-114">Not supported.</span></span>|
|<span data-ttu-id="9a7ec-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9a7ec-115">Application</span></span>|<span data-ttu-id="9a7ec-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9a7ec-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9a7ec-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="9a7ec-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9a7ec-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9a7ec-118">Global administrator</span></span>
* <span data-ttu-id="9a7ec-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="9a7ec-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9a7ec-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a7ec-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a7ec-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a7ec-121">Optional query parameters</span></span>

<span data-ttu-id="9a7ec-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="9a7ec-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9a7ec-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a7ec-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a7ec-124">Request headers</span></span>

|<span data-ttu-id="9a7ec-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9a7ec-125">Name</span></span>|<span data-ttu-id="9a7ec-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9a7ec-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9a7ec-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a7ec-127">Authorization</span></span>|<span data-ttu-id="9a7ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a7ec-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a7ec-130">Request body</span></span>

<span data-ttu-id="9a7ec-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a7ec-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a7ec-132">Response</span></span>

<span data-ttu-id="9a7ec-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [b2xUserFlow](../resources/b2xuserflows.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-133">If successful, this method returns a `200 OK` response code and a collection of [b2xUserFlow](../resources/b2xuserflows.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a7ec-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a7ec-134">Examples</span></span>

### <a name="example-1-list-all-b2xuserflows"></a><span data-ttu-id="9a7ec-135">Пример 1: List All ALL b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="9a7ec-135">Example 1: List all b2xUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="9a7ec-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a7ec-136">Request</span></span>

<span data-ttu-id="9a7ec-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a7ec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a7ec-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows
```
# <a name="c"></a>[<span data-ttu-id="9a7ec-139">C#</span><span class="sxs-lookup"><span data-stu-id="9a7ec-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a7ec-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a7ec-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a7ec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a7ec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a7ec-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a7ec-142">Response</span></span>

<span data-ttu-id="9a7ec-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-143">The following is an example of the response.</span></span>

<span data-ttu-id="9a7ec-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2xuserflows-and-expand-identityproviders"></a><span data-ttu-id="9a7ec-145">Пример 2: List All b2xUserFlows and Expand Идентитипровидерс</span><span class="sxs-lookup"><span data-stu-id="9a7ec-145">Example 2: List all b2xUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="9a7ec-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a7ec-146">Request</span></span>

<span data-ttu-id="9a7ec-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a7ec-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a7ec-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="9a7ec-149">C#</span><span class="sxs-lookup"><span data-stu-id="9a7ec-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a7ec-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a7ec-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a7ec-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a7ec-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a7ec-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a7ec-152">Response</span></span>

<span data-ttu-id="9a7ec-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-153">The following is an example of the response.</span></span>

<span data-ttu-id="9a7ec-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a7ec-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows(identityProviders)",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List b2xUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2xUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2xUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
