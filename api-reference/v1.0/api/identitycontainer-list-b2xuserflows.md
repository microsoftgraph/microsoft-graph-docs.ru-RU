---
title: Список b2xIdentityUserFlows
description: Извлечение списка объектов b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 65d592129e3475a55226199b0c246ad436a0af71
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920145"
---
# <a name="list-b2xidentityuserflows"></a><span data-ttu-id="71ce8-103">Список b2xIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="71ce8-103">List b2xIdentityUserFlows</span></span>

<span data-ttu-id="71ce8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71ce8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71ce8-105">Извлечение списка [объектов b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="71ce8-105">Retrieve a list of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="71ce8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71ce8-106">Permissions</span></span>

<span data-ttu-id="71ce8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ce8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71ce8-109">Permission type</span></span>      | <span data-ttu-id="71ce8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71ce8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71ce8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71ce8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71ce8-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ce8-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="71ce8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71ce8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="71ce8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71ce8-114">Not supported.</span></span>|
|<span data-ttu-id="71ce8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71ce8-115">Application</span></span>|<span data-ttu-id="71ce8-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ce8-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="71ce8-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="71ce8-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="71ce8-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="71ce8-118">Global administrator</span></span>
* <span data-ttu-id="71ce8-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="71ce8-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="71ce8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71ce8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71ce8-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71ce8-121">Optional query parameters</span></span>

<span data-ttu-id="71ce8-122">Вы можете использовать для расширения определенных свойств потока пользователей, которые не `$expand` расширяются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="71ce8-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="71ce8-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="71ce8-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="71ce8-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71ce8-124">Request headers</span></span>

|<span data-ttu-id="71ce8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="71ce8-125">Name</span></span>|<span data-ttu-id="71ce8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="71ce8-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="71ce8-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71ce8-127">Authorization</span></span>|<span data-ttu-id="71ce8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71ce8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ce8-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71ce8-130">Request body</span></span>

<span data-ttu-id="71ce8-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71ce8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71ce8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ce8-132">Response</span></span>

<span data-ttu-id="71ce8-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71ce8-133">If successful, this method returns a `200 OK` response code and a collection of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71ce8-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="71ce8-134">Examples</span></span>

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a><span data-ttu-id="71ce8-135">Пример 1. Список всех объектов b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="71ce8-135">Example 1: List all b2xIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="71ce8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="71ce8-136">Request</span></span>

<span data-ttu-id="71ce8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71ce8-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="71ce8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ce8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows
```
# <a name="c"></a>[<span data-ttu-id="71ce8-139">C#</span><span class="sxs-lookup"><span data-stu-id="71ce8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71ce8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ce8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71ce8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ce8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71ce8-142">Java</span><span class="sxs-lookup"><span data-stu-id="71ce8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71ce8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ce8-143">Response</span></span>

<span data-ttu-id="71ce8-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71ce8-144">The following is an example of the response.</span></span>

<span data-ttu-id="71ce8-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71ce8-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows",
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

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="71ce8-146">Пример 2. Список всех объектов b2xIdentityUserFlow и расширение identityProviders</span><span class="sxs-lookup"><span data-stu-id="71ce8-146">Example 2: List all b2xIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="71ce8-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="71ce8-147">Request</span></span>

<span data-ttu-id="71ce8-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71ce8-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="71ce8-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ce8-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="71ce8-150">C#</span><span class="sxs-lookup"><span data-stu-id="71ce8-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71ce8-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ce8-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71ce8-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ce8-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71ce8-153">Java</span><span class="sxs-lookup"><span data-stu-id="71ce8-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2xuserflows-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71ce8-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ce8-154">Response</span></span>

<span data-ttu-id="71ce8-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71ce8-155">The following is an example of the response.</span></span>

<span data-ttu-id="71ce8-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71ce8-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows(identityProviders)",
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
