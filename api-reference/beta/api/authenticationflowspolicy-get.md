---
title: Получение authenticationFlowsPolicy
description: Прочтение свойств и связей объекта authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db6e3da6d4df403fe5da71247ae6ae54f46d44b4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961401"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="c304b-103">Получение authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c304b-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="c304b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c304b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c304b-105">Прочтение свойств и связей объекта [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c304b-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c304b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c304b-106">Permissions</span></span>
<span data-ttu-id="c304b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c304b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c304b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c304b-109">Permission type</span></span>|<span data-ttu-id="c304b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c304b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c304b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c304b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c304b-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="c304b-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="c304b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c304b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c304b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c304b-114">Not Supported</span></span>|
|<span data-ttu-id="c304b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c304b-115">Application</span></span>|<span data-ttu-id="c304b-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="c304b-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="c304b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c304b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="c304b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c304b-118">Request headers</span></span>
|<span data-ttu-id="c304b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c304b-119">Name</span></span>|<span data-ttu-id="c304b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c304b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c304b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c304b-121">Authorization</span></span>|<span data-ttu-id="c304b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c304b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c304b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c304b-124">Request body</span></span>
<span data-ttu-id="c304b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c304b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c304b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c304b-126">Response</span></span>

<span data-ttu-id="c304b-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c304b-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c304b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c304b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c304b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c304b-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c304b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c304b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```
# <a name="c"></a>[<span data-ttu-id="c304b-131">C#</span><span class="sxs-lookup"><span data-stu-id="c304b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c304b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c304b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c304b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c304b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c304b-134">Java</span><span class="sxs-lookup"><span data-stu-id="c304b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationflowspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c304b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c304b-135">Response</span></span>
<span data-ttu-id="c304b-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c304b-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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


