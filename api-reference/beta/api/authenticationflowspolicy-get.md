---
title: Получение Аусентикатионфловсполици
description: Чтение свойств и связей объекта Аусентикатионфловсполици.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 348b375d022eaacfabfa2d5f37af69004eb82b98
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680924"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="2cf3e-103">Получение Аусентикатионфловсполици</span><span class="sxs-lookup"><span data-stu-id="2cf3e-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="2cf3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cf3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2cf3e-105">Чтение свойств и связей объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="2cf3e-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cf3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cf3e-106">Permissions</span></span>
<span data-ttu-id="2cf3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cf3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cf3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cf3e-109">Permission type</span></span>|<span data-ttu-id="2cf3e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cf3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cf3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cf3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2cf3e-112">Policy. Read. ALL, Policy. ReadWrite. Аусентикатионфловс</span><span class="sxs-lookup"><span data-stu-id="2cf3e-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="2cf3e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cf3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cf3e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2cf3e-114">Not Supported</span></span>|
|<span data-ttu-id="2cf3e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cf3e-115">Application</span></span>|<span data-ttu-id="2cf3e-116">Policy. Read. ALL, Policy. ReadWrite. Аусентикатионфловс</span><span class="sxs-lookup"><span data-stu-id="2cf3e-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cf3e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cf3e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="2cf3e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cf3e-118">Request headers</span></span>
|<span data-ttu-id="2cf3e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2cf3e-119">Name</span></span>|<span data-ttu-id="2cf3e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2cf3e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2cf3e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cf3e-121">Authorization</span></span>|<span data-ttu-id="2cf3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cf3e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cf3e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cf3e-124">Request body</span></span>
<span data-ttu-id="2cf3e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cf3e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cf3e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cf3e-126">Response</span></span>

<span data-ttu-id="2cf3e-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2cf3e-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cf3e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2cf3e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2cf3e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cf3e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2cf3e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cf3e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```
# <a name="c"></a>[<span data-ttu-id="2cf3e-131">C#</span><span class="sxs-lookup"><span data-stu-id="2cf3e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cf3e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cf3e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cf3e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cf3e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2cf3e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cf3e-134">Response</span></span>
<span data-ttu-id="2cf3e-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cf3e-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
