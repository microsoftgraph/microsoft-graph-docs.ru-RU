---
title: Обновление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Обновление свойств объекта passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adcafc9c37ad13dfab88ccdbabb668016569fd0b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873425"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="decdd-103">Обновление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration (неподдерживаемая версия)</span><span class="sxs-lookup"><span data-stu-id="decdd-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="decdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="decdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="decdd-105">Обновление свойств объекта [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности без пароля Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="decdd-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="decdd-106">API политики проверки подлинности для телефона без пароля Microsoft Authenticator является неподготовленным и больше не возвращает результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="decdd-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="decdd-107">Используйте новую политику метода [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="decdd-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="decdd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="decdd-108">Permissions</span></span>
<span data-ttu-id="decdd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="decdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="decdd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="decdd-111">Permission type</span></span>|<span data-ttu-id="decdd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="decdd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="decdd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="decdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="decdd-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="decdd-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="decdd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="decdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="decdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decdd-116">Not supported.</span></span>|
|<span data-ttu-id="decdd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="decdd-117">Application</span></span>|<span data-ttu-id="decdd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decdd-118">Not supported.</span></span>|

<span data-ttu-id="decdd-119">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="decdd-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="decdd-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="decdd-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="decdd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="decdd-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="decdd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="decdd-122">Request headers</span></span>
|<span data-ttu-id="decdd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="decdd-123">Name</span></span>|<span data-ttu-id="decdd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="decdd-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="decdd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="decdd-125">Authorization</span></span>|<span data-ttu-id="decdd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="decdd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="decdd-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="decdd-128">Content-Type</span></span>|<span data-ttu-id="decdd-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="decdd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="decdd-131">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="decdd-131">Request body</span></span>
<span data-ttu-id="decdd-132">В теле запроса необходимо предоставить представление объекта без [пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) в JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="decdd-132">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="decdd-133">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="decdd-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="decdd-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="decdd-134">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="decdd-135">Список свойств см. в записи [без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration.](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="decdd-135">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="decdd-136">**Примечание.** Свойство `@odata.type` со значением должно `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="decdd-136">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="decdd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="decdd-137">Response</span></span>

<span data-ttu-id="decdd-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="decdd-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="decdd-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="decdd-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="decdd-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="decdd-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "state": "enabled"
}
```


### <a name="response"></a><span data-ttu-id="decdd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="decdd-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

