---
title: Обновление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Обновление свойств объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8536e70f264775a073830aeac77d3fc27810e5f0
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418494"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="cb92f-103">Обновление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cb92f-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="cb92f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb92f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb92f-105">Обновите свойства объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , который представляет политику метода проверки подлинности входа с помощью пароля Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cb92f-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="cb92f-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="cb92f-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="cb92f-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="cb92f-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb92f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb92f-108">Permissions</span></span>
<span data-ttu-id="cb92f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb92f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb92f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb92f-111">Permission type</span></span>|<span data-ttu-id="cb92f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb92f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb92f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb92f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb92f-114">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb92f-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="cb92f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb92f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb92f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb92f-116">Not supported.</span></span>|
|<span data-ttu-id="cb92f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb92f-117">Application</span></span>|<span data-ttu-id="cb92f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb92f-118">Not supported.</span></span>|

<span data-ttu-id="cb92f-119">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="cb92f-119">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="cb92f-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="cb92f-120">Global admin</span></span>
* <span data-ttu-id="cb92f-121">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="cb92f-121">Global reader</span></span>
* <span data-ttu-id="cb92f-122">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="cb92f-122">Privileged authentication admin</span></span>
* <span data-ttu-id="cb92f-123">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="cb92f-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cb92f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb92f-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="cb92f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb92f-125">Request headers</span></span>
|<span data-ttu-id="cb92f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="cb92f-126">Name</span></span>|<span data-ttu-id="cb92f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="cb92f-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb92f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb92f-128">Authorization</span></span>|<span data-ttu-id="cb92f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb92f-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cb92f-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb92f-131">Content-Type</span></span>|<span data-ttu-id="cb92f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb92f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb92f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb92f-134">Request body</span></span>
<span data-ttu-id="cb92f-135">В тексте запроса добавьте представление объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) в формате JSON со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cb92f-135">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="cb92f-136">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="cb92f-136">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cb92f-137">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cb92f-137">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="cb92f-138">Список свойств приведен в разделе [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb92f-138">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="cb92f-139">**Примечание:** `@odata.type` Свойство со значением `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` должно быть включено в текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="cb92f-139">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="cb92f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb92f-140">Response</span></span>

<span data-ttu-id="cb92f-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb92f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb92f-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb92f-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb92f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb92f-144">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="cb92f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb92f-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

