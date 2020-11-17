---
title: Получение Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Чтение свойств и связей объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e47045c6eb34c393cffb89d004fb1c7a27efc49d
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086762"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="52189-103">Получение Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="52189-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="52189-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52189-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52189-105">Получение свойств и связей объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , который представляет [политику метода проверки подлинности](../resources/authenticationmethodspolicies-overview.md) входа с помощью пароля Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="52189-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="52189-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="52189-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="52189-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="52189-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="52189-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52189-108">Permissions</span></span>
<span data-ttu-id="52189-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52189-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52189-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52189-111">Permission type</span></span>|<span data-ttu-id="52189-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52189-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52189-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52189-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52189-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="52189-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="52189-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52189-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52189-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52189-116">Not supported.</span></span>|
|<span data-ttu-id="52189-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52189-117">Application</span></span>|<span data-ttu-id="52189-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52189-118">Not supported.</span></span>|

<span data-ttu-id="52189-119">Для делегированных сценариев администратору требуется следующая [роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="52189-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="52189-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="52189-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="52189-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52189-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="52189-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52189-122">Request headers</span></span>
|<span data-ttu-id="52189-123">Имя</span><span class="sxs-lookup"><span data-stu-id="52189-123">Name</span></span>|<span data-ttu-id="52189-124">Описание</span><span class="sxs-lookup"><span data-stu-id="52189-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="52189-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52189-125">Authorization</span></span>|<span data-ttu-id="52189-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52189-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52189-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52189-128">Request body</span></span>
<span data-ttu-id="52189-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52189-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52189-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="52189-130">Response</span></span>

<span data-ttu-id="52189-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52189-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52189-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="52189-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52189-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="52189-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="52189-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="52189-134">Response</span></span>
<span data-ttu-id="52189-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="52189-135">The following is an example of the response.</span></span>

<span data-ttu-id="52189-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="52189-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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

