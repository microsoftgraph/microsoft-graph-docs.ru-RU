---
title: Список b2cIdentityUserFlows
description: Получение списка объектов b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dfb17696d6a46e151f5dd2f6479395404d2b063f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406451"
---
# <a name="list-b2cidentityuserflows"></a><span data-ttu-id="c2124-103">Список b2cIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="c2124-103">List b2cIdentityUserFlows</span></span>

<span data-ttu-id="c2124-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2124-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2124-105">Получение списка объектов [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="c2124-105">Retrieve a list of [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2124-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2124-106">Permissions</span></span>

<span data-ttu-id="c2124-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2124-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2124-109">Permission type</span></span>      | <span data-ttu-id="c2124-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2124-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2124-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2124-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2124-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2124-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c2124-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2124-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c2124-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2124-114">Not supported.</span></span>|
|<span data-ttu-id="c2124-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2124-115">Application</span></span>|<span data-ttu-id="c2124-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2124-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c2124-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c2124-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c2124-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c2124-118">Global administrator</span></span>
* <span data-ttu-id="c2124-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="c2124-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c2124-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2124-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2124-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2124-121">Optional query parameters</span></span>

<span data-ttu-id="c2124-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="c2124-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="c2124-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c2124-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2124-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2124-124">Request headers</span></span>

|<span data-ttu-id="c2124-125">Имя</span><span class="sxs-lookup"><span data-stu-id="c2124-125">Name</span></span>|<span data-ttu-id="c2124-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c2124-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c2124-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2124-127">Authorization</span></span>|<span data-ttu-id="c2124-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2124-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2124-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2124-130">Request body</span></span>

<span data-ttu-id="c2124-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2124-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2124-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2124-132">Response</span></span>

<span data-ttu-id="c2124-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)  в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2124-133">If successful, this method returns a `200 OK` response code and a collection of [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2124-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2124-134">Examples</span></span>

### <a name="example-1-list-all-b2cidentityuserflow-objects"></a><span data-ttu-id="c2124-135">Пример 1: список всех объектов b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="c2124-135">Example 1: List all b2cIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="c2124-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2124-136">Request</span></span>

<span data-ttu-id="c2124-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2124-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c2124-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2124-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```
# <a name="c"></a>[<span data-ttu-id="c2124-139">C#</span><span class="sxs-lookup"><span data-stu-id="c2124-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2124-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2124-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2124-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2124-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2124-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2124-142">Response</span></span>

<span data-ttu-id="c2124-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2124-143">The following is an example of the response.</span></span>

<span data-ttu-id="c2124-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2124-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows",
    "value": [
      {
          "id": "B2C_1_CustomerSignUp",
          "userFlowType": "signUp",
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2cidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="c2124-145">Пример 2: список всех объектов b2cIdentityUserFlow и разверните узел Идентитипровидерс</span><span class="sxs-lookup"><span data-stu-id="c2124-145">Example 2: List all b2cIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="c2124-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2124-146">Request</span></span>

<span data-ttu-id="c2124-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2124-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c2124-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2124-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="c2124-149">C#</span><span class="sxs-lookup"><span data-stu-id="c2124-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2124-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2124-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2124-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2124-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2124-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2124-152">Response</span></span>

<span data-ttu-id="c2124-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2124-153">The following is an example of the response.</span></span>

<span data-ttu-id="c2124-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2124-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows",
    "value": [
      {
          "id": "B2C_1_CustomerSignUp",
          "userFlowType": "signUp",
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
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
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
  "description": "List b2cUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2cUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2cUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


