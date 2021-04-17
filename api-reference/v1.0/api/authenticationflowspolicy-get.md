---
title: Получение authenticationFlowsPolicy
description: Прочтение свойств и связей объекта authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7f96ffc150ef5ac2eefc759059e163560a6c8841
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883366"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="77217-103">Получение authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="77217-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="77217-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77217-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77217-105">Прочтение свойств и связей объекта [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="77217-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77217-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77217-106">Permissions</span></span>

<span data-ttu-id="77217-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77217-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77217-109">Permission type</span></span>|<span data-ttu-id="77217-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77217-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77217-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77217-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77217-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="77217-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="77217-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77217-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77217-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="77217-114">Not Supported</span></span>|
|<span data-ttu-id="77217-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77217-115">Application</span></span>|<span data-ttu-id="77217-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="77217-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="77217-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77217-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="77217-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77217-118">Request headers</span></span>

|<span data-ttu-id="77217-119">Имя</span><span class="sxs-lookup"><span data-stu-id="77217-119">Name</span></span>|<span data-ttu-id="77217-120">Описание</span><span class="sxs-lookup"><span data-stu-id="77217-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="77217-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77217-121">Authorization</span></span>|<span data-ttu-id="77217-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77217-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77217-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77217-124">Request body</span></span>

<span data-ttu-id="77217-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77217-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77217-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="77217-126">Response</span></span>

<span data-ttu-id="77217-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77217-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77217-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="77217-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77217-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="77217-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
```

### <a name="response"></a><span data-ttu-id="77217-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="77217-130">Response</span></span>

<span data-ttu-id="77217-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77217-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authenticationFlowsPolicy/$entity",
    "id": "authenticationFlowsPolicy",
    "displayName": "Authentication flows policy",
    "description": "Authentication flows policy allows modification of settings related to authentication flows in AAD tenant, such as self-service sign up configuration.",
    "selfServiceSignUp": {
        "isEnabled": true
    }
}
```
