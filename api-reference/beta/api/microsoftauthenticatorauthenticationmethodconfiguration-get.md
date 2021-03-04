---
title: Получите microsoftAuthenticatorAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 32470fb4ebce664fadce95982adb0d2d61bf6f03
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443701"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="ed426-103">Получите microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed426-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="ed426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed426-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed426-105">Извлечение свойств и связей объекта [MicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ed426-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed426-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed426-106">Permissions</span></span>
<span data-ttu-id="ed426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed426-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed426-109">Permission type</span></span>|<span data-ttu-id="ed426-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed426-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed426-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed426-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed426-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ed426-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="ed426-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed426-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed426-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed426-114">Not supported.</span></span>|
|<span data-ttu-id="ed426-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed426-115">Application</span></span>|<span data-ttu-id="ed426-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ed426-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="ed426-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="ed426-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="ed426-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="ed426-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="ed426-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed426-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="ed426-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed426-120">Request headers</span></span>
|<span data-ttu-id="ed426-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ed426-121">Name</span></span>|<span data-ttu-id="ed426-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ed426-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed426-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed426-123">Authorization</span></span>|<span data-ttu-id="ed426-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed426-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed426-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed426-126">Request body</span></span>
<span data-ttu-id="ed426-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed426-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed426-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed426-128">Response</span></span>

<span data-ttu-id="ed426-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ed426-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed426-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed426-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed426-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed426-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="ed426-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed426-132">Response</span></span>
<span data-ttu-id="ed426-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ed426-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "state": "String"
  }
}
```

