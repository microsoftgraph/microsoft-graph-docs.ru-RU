---
title: Получение Аусентикатионфловсполици
description: Чтение свойств и связей объекта Аусентикатионфловсполици.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 843eb458788200a4e2fe6e0248f6966090abe1f0
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556435"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="2d709-103">Получение Аусентикатионфловсполици</span><span class="sxs-lookup"><span data-stu-id="2d709-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="2d709-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d709-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d709-105">Чтение свойств и связей объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="2d709-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d709-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d709-106">Permissions</span></span>
<span data-ttu-id="2d709-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d709-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d709-109">Permission type</span></span>|<span data-ttu-id="2d709-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d709-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d709-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d709-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d709-112">Policy. Read. ALL, Policy. ReadWrite. Аусентикатионфловс</span><span class="sxs-lookup"><span data-stu-id="2d709-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="2d709-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d709-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d709-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2d709-114">Not Supported</span></span>|
|<span data-ttu-id="2d709-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d709-115">Application</span></span>|<span data-ttu-id="2d709-116">Policy. Read. ALL, Policy. ReadWrite. Аусентикатионфловс</span><span class="sxs-lookup"><span data-stu-id="2d709-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d709-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d709-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="2d709-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d709-118">Request headers</span></span>
|<span data-ttu-id="2d709-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2d709-119">Name</span></span>|<span data-ttu-id="2d709-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2d709-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d709-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d709-121">Authorization</span></span>|<span data-ttu-id="2d709-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d709-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d709-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d709-124">Request body</span></span>
<span data-ttu-id="2d709-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d709-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d709-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d709-126">Response</span></span>

<span data-ttu-id="2d709-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d709-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d709-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d709-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d709-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d709-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

### <a name="response"></a><span data-ttu-id="2d709-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d709-130">Response</span></span>
<span data-ttu-id="2d709-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2d709-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationFlowsPolicy/$entity",
    "id": "authenticationFlowsPolicy",
    "displayName": "Authentication flows policy",
    "description": "Authentication flows policy allows modification of settings related to authentication flows in AAD tenant, such as self-service sign up configuration.",
    "selfServiceSignUp": {
        "isEnabled": true
    }
}
```
