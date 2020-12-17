---
title: Список b2cIdentityUserFlows
description: Получить список объектов b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 454422c09649b97ffbab96c313201ebef0cad23e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705851"
---
# <a name="list-b2cidentityuserflows"></a><span data-ttu-id="62897-103">Список b2cIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="62897-103">List b2cIdentityUserFlows</span></span>

<span data-ttu-id="62897-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62897-105">Получить список объектов [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="62897-105">Retrieve a list of [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="62897-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62897-106">Permissions</span></span>

<span data-ttu-id="62897-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62897-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62897-109">Permission type</span></span>      | <span data-ttu-id="62897-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62897-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62897-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62897-111">Delegated (work or school account)</span></span>|<span data-ttu-id="62897-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62897-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="62897-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62897-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="62897-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62897-114">Not supported.</span></span>|
|<span data-ttu-id="62897-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="62897-115">Application</span></span>|<span data-ttu-id="62897-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62897-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="62897-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="62897-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="62897-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="62897-118">Global administrator</span></span>
* <span data-ttu-id="62897-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="62897-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="62897-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62897-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62897-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62897-121">Optional query parameters</span></span>

<span data-ttu-id="62897-122">Можно использовать `$expand` для расширения определенных свойств пользовательского потока, которые не расширены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="62897-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="62897-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="62897-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62897-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62897-124">Request headers</span></span>

|<span data-ttu-id="62897-125">Имя</span><span class="sxs-lookup"><span data-stu-id="62897-125">Name</span></span>|<span data-ttu-id="62897-126">Описание</span><span class="sxs-lookup"><span data-stu-id="62897-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="62897-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62897-127">Authorization</span></span>|<span data-ttu-id="62897-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62897-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62897-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62897-130">Request body</span></span>

<span data-ttu-id="62897-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62897-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62897-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="62897-132">Response</span></span>

<span data-ttu-id="62897-133">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)  в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="62897-133">If successful, this method returns a `200 OK` response code and a collection of [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62897-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="62897-134">Examples</span></span>

### <a name="example-1-list-all-b2cidentityuserflow-objects"></a><span data-ttu-id="62897-135">Пример 1. Список всех объектов b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="62897-135">Example 1: List all b2cIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="62897-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="62897-136">Request</span></span>

<span data-ttu-id="62897-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62897-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62897-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="62897-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```
# <a name="c"></a>[<span data-ttu-id="62897-139">C#</span><span class="sxs-lookup"><span data-stu-id="62897-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62897-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62897-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62897-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62897-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62897-142">Java</span><span class="sxs-lookup"><span data-stu-id="62897-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="62897-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="62897-143">Response</span></span>

<span data-ttu-id="62897-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62897-144">The following is an example of the response.</span></span>

<span data-ttu-id="62897-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62897-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
          "isLanguageCustomizationEnabled": false,
          "defaultLanguageTag": null
      },
      {
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
          "userFlowTypeVersion": 1,
          "isLanguageCustomizationEnabled": true,
          "defaultLanguageTag": "en"
      },
    ]
}
```

### <a name="example-2-list-all-b2cidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="62897-146">Пример 2. Список всех объектов b2cIdentityUserFlow и расширение identityProviders</span><span class="sxs-lookup"><span data-stu-id="62897-146">Example 2: List all b2cIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="62897-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="62897-147">Request</span></span>

<span data-ttu-id="62897-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62897-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62897-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="62897-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="62897-150">C#</span><span class="sxs-lookup"><span data-stu-id="62897-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62897-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62897-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62897-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62897-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62897-153">Java</span><span class="sxs-lookup"><span data-stu-id="62897-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2cuserflows-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62897-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="62897-154">Response</span></span>

<span data-ttu-id="62897-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62897-155">The following is an example of the response.</span></span>

<span data-ttu-id="62897-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62897-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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
          "isLanguageCustomizationEnabled": false,
          "defaultLanguageTag": null,
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
          "isLanguageCustomizationEnabled": true,
          "defaultLanguageTag": "en",
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


