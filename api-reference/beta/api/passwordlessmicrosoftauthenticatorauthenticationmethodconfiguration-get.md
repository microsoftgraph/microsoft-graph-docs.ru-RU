---
title: Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c21d1c8601715beef6f056defbf203afa417ac0c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447761"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="2a8cb-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="2a8cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a8cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a8cb-105">Извлечение свойств и связей объекта Без паролейMicrosoftAuthenticatorAuthenticationMethodConfiguration, который представляет политику [](../resources/authenticationmethodspolicies-overview.md) метода проверки подлинности без паролей Microsoft Authenticator Для клиента Azure AD. [](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="2a8cb-106">API политики метода проверки подлинности без паролей Microsoft Authenticator Phone является обесценен и перестал возвращать результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="2a8cb-107">Используйте новую политику метода проверки подлинности [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a8cb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a8cb-108">Permissions</span></span>
<span data-ttu-id="2a8cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a8cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a8cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a8cb-111">Permission type</span></span>|<span data-ttu-id="2a8cb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a8cb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a8cb-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2a8cb-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="2a8cb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a8cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-116">Not supported.</span></span>|
|<span data-ttu-id="2a8cb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a8cb-117">Application</span></span>|<span data-ttu-id="2a8cb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-118">Not supported.</span></span>|

<span data-ttu-id="2a8cb-119">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="2a8cb-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2a8cb-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2a8cb-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="2a8cb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a8cb-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="2a8cb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a8cb-122">Request headers</span></span>
|<span data-ttu-id="2a8cb-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2a8cb-123">Name</span></span>|<span data-ttu-id="2a8cb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2a8cb-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a8cb-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a8cb-125">Authorization</span></span>|<span data-ttu-id="2a8cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a8cb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a8cb-128">Request body</span></span>
<span data-ttu-id="2a8cb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a8cb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a8cb-130">Response</span></span>

<span data-ttu-id="2a8cb-131">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a8cb-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a8cb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a8cb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a8cb-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="2a8cb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a8cb-134">Response</span></span>
<span data-ttu-id="2a8cb-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-135">The following is an example of the response.</span></span>

<span data-ttu-id="2a8cb-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "PasswordlessMicrosoftAuthenticator",
    "state": "enabled",
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
}
```

