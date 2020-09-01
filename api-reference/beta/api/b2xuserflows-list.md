---
title: Список b2xUserFlows
description: Получение списка объектов b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cec5cd2bd05d8c2f6b73002bcd779790ffc34b66
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319800"
---
# <a name="list-b2xuserflows"></a><span data-ttu-id="fa2ee-103">Список b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="fa2ee-103">List b2xUserFlows</span></span>

<span data-ttu-id="fa2ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa2ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa2ee-105">Получение списка объектов [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="fa2ee-105">Retrieve a list of [b2xUserFlow](../resources/b2xuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa2ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa2ee-106">Permissions</span></span>

<span data-ttu-id="fa2ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa2ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa2ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa2ee-109">Permission type</span></span>      | <span data-ttu-id="fa2ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa2ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa2ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa2ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa2ee-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa2ee-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fa2ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa2ee-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fa2ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-114">Not supported.</span></span>|
|<span data-ttu-id="fa2ee-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa2ee-115">Application</span></span>|<span data-ttu-id="fa2ee-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa2ee-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fa2ee-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="fa2ee-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fa2ee-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fa2ee-118">Global administrator</span></span>
* <span data-ttu-id="fa2ee-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="fa2ee-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fa2ee-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa2ee-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa2ee-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa2ee-121">Optional query parameters</span></span>

<span data-ttu-id="fa2ee-122">Можно использовать `$expand` для расширения определенных свойств пользовательского пользовательского процесса, которые по умолчанию не развернуты.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="fa2ee-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fa2ee-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa2ee-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa2ee-124">Request headers</span></span>

|<span data-ttu-id="fa2ee-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fa2ee-125">Name</span></span>|<span data-ttu-id="fa2ee-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fa2ee-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fa2ee-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa2ee-127">Authorization</span></span>|<span data-ttu-id="fa2ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa2ee-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa2ee-130">Request body</span></span>

<span data-ttu-id="fa2ee-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa2ee-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa2ee-132">Response</span></span>

<span data-ttu-id="fa2ee-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [b2xUserFlow](../resources/b2xuserflows.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-133">If successful, this method returns a `200 OK` response code and a collection of [b2xUserFlow](../resources/b2xuserflows.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa2ee-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa2ee-134">Examples</span></span>

### <a name="example-1-list-all-b2xuserflows"></a><span data-ttu-id="fa2ee-135">Пример 1: List All ALL b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="fa2ee-135">Example 1: List all b2xUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="fa2ee-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa2ee-136">Request</span></span>

<span data-ttu-id="fa2ee-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows
```

#### <a name="response"></a><span data-ttu-id="fa2ee-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa2ee-138">Response</span></span>

<span data-ttu-id="fa2ee-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-139">The following is an example of the response.</span></span>

<span data-ttu-id="fa2ee-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-b2xuserflows-and-expand-identityproviders"></a><span data-ttu-id="fa2ee-141">Пример 2: List All b2xUserFlows and Expand Идентитипровидерс</span><span class="sxs-lookup"><span data-stu-id="fa2ee-141">Example 2: List all b2xUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="fa2ee-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa2ee-142">Request</span></span>

<span data-ttu-id="fa2ee-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows?$expand=identityProviders
```

#### <a name="response"></a><span data-ttu-id="fa2ee-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa2ee-144">Response</span></span>

<span data-ttu-id="fa2ee-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-145">The following is an example of the response.</span></span>

<span data-ttu-id="fa2ee-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa2ee-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
