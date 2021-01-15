---
title: Удаление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Удаление объекта passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7b7cb8cc0eca09dde9e4ecb56a570bf1faf92b05
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873453"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="b0b64-103">Удаление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration (неподдерживаемая)</span><span class="sxs-lookup"><span data-stu-id="b0b64-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="b0b64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0b64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0b64-105">Удалите изменения, внесенные в политику метода проверки подлинности на телефоне [Microsoft Authenticator,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) вернув политику к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0b64-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!CAUTION]
> <span data-ttu-id="b0b64-106">API политики проверки подлинности для телефона без пароля Microsoft Authenticator является неподготовленным и больше не возвращает результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="b0b64-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="b0b64-107">Используйте новую политику метода [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0b64-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0b64-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0b64-108">Permissions</span></span>
<span data-ttu-id="b0b64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0b64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0b64-111">Permission type</span></span>|<span data-ttu-id="b0b64-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0b64-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0b64-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0b64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0b64-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0b64-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="b0b64-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0b64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0b64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0b64-116">Not supported.</span></span>|
|<span data-ttu-id="b0b64-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0b64-117">Application</span></span>|<span data-ttu-id="b0b64-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0b64-118">Not supported.</span></span>|

<span data-ttu-id="b0b64-119">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b0b64-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b0b64-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b0b64-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="b0b64-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0b64-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="b0b64-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0b64-122">Request headers</span></span>
|<span data-ttu-id="b0b64-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b0b64-123">Name</span></span>|<span data-ttu-id="b0b64-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b64-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b0b64-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0b64-125">Authorization</span></span>|<span data-ttu-id="b0b64-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0b64-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0b64-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0b64-128">Request body</span></span>
<span data-ttu-id="b0b64-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0b64-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0b64-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0b64-130">Response</span></span>

<span data-ttu-id="b0b64-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b0b64-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b0b64-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0b64-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0b64-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0b64-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="b0b64-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0b64-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

