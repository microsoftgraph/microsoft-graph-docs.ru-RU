---
title: Обновление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Обновление свойств объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91c158137406da47cddfaaa2384ed951d326358f
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086636"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="b7cad-103">Обновление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b7cad-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="b7cad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7cad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7cad-105">Обновите свойства объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , который представляет политику метода проверки подлинности входа с помощью пароля Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7cad-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="b7cad-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="b7cad-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="b7cad-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="b7cad-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7cad-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7cad-108">Permissions</span></span>
<span data-ttu-id="b7cad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7cad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7cad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7cad-111">Permission type</span></span>|<span data-ttu-id="b7cad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7cad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7cad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7cad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7cad-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b7cad-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="b7cad-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7cad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7cad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7cad-116">Not supported.</span></span>|
|<span data-ttu-id="b7cad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7cad-117">Application</span></span>|<span data-ttu-id="b7cad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7cad-118">Not supported.</span></span>|

<span data-ttu-id="b7cad-119">Для делегированных сценариев администратору требуется следующая [роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="b7cad-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b7cad-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b7cad-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="b7cad-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7cad-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="b7cad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7cad-122">Request headers</span></span>
|<span data-ttu-id="b7cad-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b7cad-123">Name</span></span>|<span data-ttu-id="b7cad-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b7cad-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7cad-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7cad-125">Authorization</span></span>|<span data-ttu-id="b7cad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7cad-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b7cad-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7cad-128">Content-Type</span></span>|<span data-ttu-id="b7cad-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7cad-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7cad-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7cad-131">Request body</span></span>
<span data-ttu-id="b7cad-132">В тексте запроса добавьте представление объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) в формате JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b7cad-132">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="b7cad-133">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="b7cad-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b7cad-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b7cad-134">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="b7cad-135">Список свойств приведен в разделе [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7cad-135">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="b7cad-136">**Примечание:** `@odata.type` Свойство со значением `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` должно быть включено в текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="b7cad-136">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="b7cad-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7cad-137">Response</span></span>

<span data-ttu-id="b7cad-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b7cad-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7cad-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="b7cad-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7cad-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7cad-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="b7cad-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7cad-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

