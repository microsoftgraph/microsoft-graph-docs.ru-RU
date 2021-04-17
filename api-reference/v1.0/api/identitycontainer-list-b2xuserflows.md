---
title: Список b2xIdentityUserFlows
description: Извлечение списка объектов b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36b0399c7fd45a90b5bbfb95084f46a15ff65296
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883031"
---
# <a name="list-b2xidentityuserflows"></a><span data-ttu-id="22762-103">Список b2xIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="22762-103">List b2xIdentityUserFlows</span></span>

<span data-ttu-id="22762-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22762-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22762-105">Извлечение списка [объектов b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="22762-105">Retrieve a list of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="22762-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22762-106">Permissions</span></span>

<span data-ttu-id="22762-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22762-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22762-109">Permission type</span></span>      | <span data-ttu-id="22762-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22762-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22762-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22762-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22762-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22762-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="22762-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22762-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="22762-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22762-114">Not supported.</span></span>|
|<span data-ttu-id="22762-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22762-115">Application</span></span>|<span data-ttu-id="22762-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22762-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="22762-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="22762-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="22762-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="22762-118">Global administrator</span></span>
* <span data-ttu-id="22762-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="22762-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="22762-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22762-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22762-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22762-121">Optional query parameters</span></span>

<span data-ttu-id="22762-122">Вы можете использовать для расширения определенных свойств потока пользователей, которые не `$expand` расширяются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="22762-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="22762-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="22762-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22762-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22762-124">Request headers</span></span>

|<span data-ttu-id="22762-125">Имя</span><span class="sxs-lookup"><span data-stu-id="22762-125">Name</span></span>|<span data-ttu-id="22762-126">Описание</span><span class="sxs-lookup"><span data-stu-id="22762-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="22762-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22762-127">Authorization</span></span>|<span data-ttu-id="22762-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22762-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22762-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22762-130">Request body</span></span>

<span data-ttu-id="22762-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22762-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22762-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="22762-132">Response</span></span>

<span data-ttu-id="22762-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22762-133">If successful, this method returns a `200 OK` response code and a collection of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22762-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="22762-134">Examples</span></span>

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a><span data-ttu-id="22762-135">Пример 1. Список всех объектов b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="22762-135">Example 1: List all b2xIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="22762-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="22762-136">Request</span></span>

<span data-ttu-id="22762-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22762-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows
```

#### <a name="response"></a><span data-ttu-id="22762-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="22762-138">Response</span></span>

<span data-ttu-id="22762-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22762-139">The following is an example of the response.</span></span>

<span data-ttu-id="22762-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22762-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="22762-141">Пример 2. Список всех объектов b2xIdentityUserFlow и расширение identityProviders</span><span class="sxs-lookup"><span data-stu-id="22762-141">Example 2: List all b2xIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="22762-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="22762-142">Request</span></span>

<span data-ttu-id="22762-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22762-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows?$expand=identityProviders
```

#### <a name="response"></a><span data-ttu-id="22762-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="22762-144">Response</span></span>

<span data-ttu-id="22762-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22762-145">The following is an example of the response.</span></span>

<span data-ttu-id="22762-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22762-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
