---
title: Обновление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Обновление свойств объекта без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9093e049eab262df56c914bdb735e9d9600b799d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447670"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="6557b-103">Обновление passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span><span class="sxs-lookup"><span data-stu-id="6557b-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="6557b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6557b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6557b-105">Обновим свойства объекта Без [пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности без пароля Microsoft Authenticator Phone для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6557b-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="6557b-106">API политики метода проверки подлинности без паролей Microsoft Authenticator Phone является обесценен и перестал возвращать результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="6557b-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="6557b-107">Используйте новую политику метода проверки подлинности [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6557b-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6557b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6557b-108">Permissions</span></span>
<span data-ttu-id="6557b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6557b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6557b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6557b-111">Permission type</span></span>|<span data-ttu-id="6557b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6557b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6557b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6557b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6557b-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6557b-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="6557b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6557b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6557b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6557b-116">Not supported.</span></span>|
|<span data-ttu-id="6557b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6557b-117">Application</span></span>|<span data-ttu-id="6557b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6557b-118">Not supported.</span></span>|

<span data-ttu-id="6557b-119">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="6557b-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="6557b-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6557b-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="6557b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6557b-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="6557b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6557b-122">Request headers</span></span>
|<span data-ttu-id="6557b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6557b-123">Name</span></span>|<span data-ttu-id="6557b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6557b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6557b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6557b-125">Authorization</span></span>|<span data-ttu-id="6557b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6557b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6557b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6557b-128">Content-Type</span></span>|<span data-ttu-id="6557b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6557b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6557b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6557b-131">Request body</span></span>
<span data-ttu-id="6557b-132">В корпусе запроса устройте представление JSON без [пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6557b-132">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="6557b-133">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="6557b-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6557b-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6557b-134">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="6557b-135">Список свойств см. в списке [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6557b-135">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="6557b-136">**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` должно быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="6557b-136">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="6557b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6557b-137">Response</span></span>

<span data-ttu-id="6557b-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6557b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6557b-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6557b-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6557b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6557b-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="6557b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6557b-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

