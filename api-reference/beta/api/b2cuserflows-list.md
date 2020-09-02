---
title: Список b2cUserFlows
description: Получение списка объектов b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c5dac4c53d9e58dc9b95b4b4c3f7f9205b6563e
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329842"
---
# <a name="list-b2cuserflows"></a><span data-ttu-id="3eee5-103">Список b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="3eee5-103">List b2cUserFlows</span></span>

<span data-ttu-id="3eee5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eee5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eee5-105">Получение списка объектов [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="3eee5-105">Retrieve a list of [b2cUserFlow](../resources/b2cuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eee5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3eee5-106">Permissions</span></span>

<span data-ttu-id="3eee5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eee5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eee5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eee5-109">Permission type</span></span>      | <span data-ttu-id="3eee5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eee5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eee5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eee5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3eee5-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3eee5-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3eee5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eee5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3eee5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eee5-114">Not supported.</span></span>|
|<span data-ttu-id="3eee5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3eee5-115">Application</span></span>|<span data-ttu-id="3eee5-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3eee5-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3eee5-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3eee5-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3eee5-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3eee5-118">Global administrator</span></span>
* <span data-ttu-id="3eee5-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="3eee5-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3eee5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eee5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3eee5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3eee5-121">Optional query parameters</span></span>

<span data-ttu-id="3eee5-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="3eee5-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="3eee5-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3eee5-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3eee5-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3eee5-124">Request headers</span></span>

|<span data-ttu-id="3eee5-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3eee5-125">Name</span></span>|<span data-ttu-id="3eee5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3eee5-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3eee5-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3eee5-127">Authorization</span></span>|<span data-ttu-id="3eee5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eee5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eee5-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eee5-130">Request body</span></span>

<span data-ttu-id="3eee5-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3eee5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eee5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eee5-132">Response</span></span>

<span data-ttu-id="3eee5-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [b2cUserFlow](../resources/b2cuserflows.md)  в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3eee5-133">If successful, this method returns a `200 OK` response code and a collection of [b2cUserFlow](../resources/b2cuserflows.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3eee5-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="3eee5-134">Examples</span></span>

### <a name="example-1-list-all-b2cuserflows"></a><span data-ttu-id="3eee5-135">Пример 1: List All ALL b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="3eee5-135">Example 1: List all b2cUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="3eee5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eee5-136">Request</span></span>

<span data-ttu-id="3eee5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eee5-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3eee5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3eee5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```
# <a name="c"></a>[<span data-ttu-id="3eee5-139">C#</span><span class="sxs-lookup"><span data-stu-id="3eee5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3eee5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3eee5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3eee5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3eee5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3eee5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eee5-142">Response</span></span>

<span data-ttu-id="3eee5-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3eee5-143">The following is an example of the response.</span></span>

<span data-ttu-id="3eee5-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3eee5-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-b2cuserflows-and-expand-identityproviders"></a><span data-ttu-id="3eee5-145">Пример 2: List All b2cUserFlows and Expand Идентитипровидерс</span><span class="sxs-lookup"><span data-stu-id="3eee5-145">Example 2: List all b2cUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="3eee5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eee5-146">Request</span></span>

<span data-ttu-id="3eee5-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eee5-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3eee5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3eee5-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="3eee5-149">C#</span><span class="sxs-lookup"><span data-stu-id="3eee5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3eee5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3eee5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3eee5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3eee5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3eee5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eee5-152">Response</span></span>

<span data-ttu-id="3eee5-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3eee5-153">The following is an example of the response.</span></span>

<span data-ttu-id="3eee5-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3eee5-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
