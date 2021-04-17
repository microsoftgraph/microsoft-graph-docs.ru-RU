---
title: Get b2xIdentityUserFlow
description: Извлечение свойств и связей объекта b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: a498e4a6ab1d652dca3c90afc33649f0c0ada908
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882461"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="3fa60-103">Get b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3fa60-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="3fa60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fa60-105">Извлечение свойств и связей объекта [b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3fa60-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa60-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa60-106">Permissions</span></span>

<span data-ttu-id="3fa60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fa60-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa60-109">Permission type</span></span>      | <span data-ttu-id="3fa60-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fa60-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fa60-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa60-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa60-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa60-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3fa60-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa60-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3fa60-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa60-114">Not supported.</span></span>|
|<span data-ttu-id="3fa60-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fa60-115">Application</span></span>|<span data-ttu-id="3fa60-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa60-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3fa60-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3fa60-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3fa60-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3fa60-118">Global administrator</span></span>
* <span data-ttu-id="3fa60-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="3fa60-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3fa60-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa60-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fa60-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3fa60-121">Optional query parameters</span></span>

<span data-ttu-id="3fa60-122">Вы можете использовать для расширения определенных свойств потока пользователей, которые не `$expand` расширяются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3fa60-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="3fa60-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3fa60-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fa60-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fa60-124">Request headers</span></span>

|<span data-ttu-id="3fa60-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3fa60-125">Name</span></span>|<span data-ttu-id="3fa60-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa60-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3fa60-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fa60-127">Authorization</span></span>|<span data-ttu-id="3fa60-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa60-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa60-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fa60-130">Request body</span></span>

<span data-ttu-id="3fa60-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fa60-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fa60-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa60-132">Response</span></span>

<span data-ttu-id="3fa60-133">В случае успеха этот метод возвращает код отклика и `200 OK` представление [JSON b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3fa60-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa60-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa60-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa60-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa60-135">Request</span></span>

<span data-ttu-id="3fa60-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fa60-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp
```

### <a name="response"></a><span data-ttu-id="3fa60-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa60-137">Response</span></span>

<span data-ttu-id="3fa60-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3fa60-138">The following is an example of the response.</span></span>

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
