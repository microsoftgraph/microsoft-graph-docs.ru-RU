---
title: Получите microsoftAuthenticatorAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 49cd8ffdf9fa2cda030024b3d2ac687d0da4789f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896608"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="ecc2a-103">Получите microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecc2a-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="ecc2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecc2a-105">Извлечение свойств и связей объекта [MicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода Microsoft Authenticator проверки подлинности для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc2a-106">Permissions</span></span>
<span data-ttu-id="ecc2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecc2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecc2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc2a-109">Permission type</span></span>|<span data-ttu-id="ecc2a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecc2a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecc2a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecc2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecc2a-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ecc2a-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="ecc2a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecc2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecc2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-114">Not supported.</span></span>|
|<span data-ttu-id="ecc2a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecc2a-115">Application</span></span>|<span data-ttu-id="ecc2a-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ecc2a-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="ecc2a-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="ecc2a-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="ecc2a-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="ecc2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecc2a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="ecc2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecc2a-120">Request headers</span></span>
|<span data-ttu-id="ecc2a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ecc2a-121">Name</span></span>|<span data-ttu-id="ecc2a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ecc2a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ecc2a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecc2a-123">Authorization</span></span>|<span data-ttu-id="ecc2a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecc2a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecc2a-126">Request body</span></span>
<span data-ttu-id="ecc2a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc2a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc2a-128">Response</span></span>

<span data-ttu-id="ecc2a-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecc2a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecc2a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecc2a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecc2a-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ecc2a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc2a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="ecc2a-133">C#</span><span class="sxs-lookup"><span data-stu-id="ecc2a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-microsoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecc2a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecc2a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-microsoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecc2a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecc2a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-microsoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecc2a-136">Java</span><span class="sxs-lookup"><span data-stu-id="ecc2a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-microsoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ecc2a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc2a-137">Response</span></span>
<span data-ttu-id="ecc2a-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecc2a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "129ae788-e788-129a-88e7-9a1288e79a12",
    "state": "String",
    "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('MicrosoftAuthenticator')/microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration/includeTargets", 
    "includeTargets": [ 
        { 
            "targetType": "group", 
            "id": "5c6226ca-d325-4972-9fa8-1861c91f74c0", 
            "isRegistrationRequired": false, 
            "authenticationMode": "any", 
            "numberMatchingRequiredState": "default",
            "displayLocationInformationRequiredState": "default",
            "displayAppInformationRequiredState": "default"
        } 
    ] 
  }
}
```

