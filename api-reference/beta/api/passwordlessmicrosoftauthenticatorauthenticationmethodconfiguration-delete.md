---
title: Удаление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Удаление объекта passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 01c95eabb3d888b03b1024d25364b3bd6474deef
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472474"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="e3d7b-103">Удаление без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span><span class="sxs-lookup"><span data-stu-id="e3d7b-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="e3d7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3d7b-105">Удалите изменения, внесенные в политику метода проверки подлинности в microsoft [Authenticator Phone,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) возвращая политику в конфигурацию по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!CAUTION]
> <span data-ttu-id="e3d7b-106">API политики метода проверки подлинности без паролей Microsoft Authenticator Phone является обесценен и перестал возвращать результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="e3d7b-107">Используйте новую политику метода проверки подлинности [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3d7b-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3d7b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3d7b-108">Permissions</span></span>
<span data-ttu-id="e3d7b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3d7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3d7b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3d7b-111">Permission type</span></span>|<span data-ttu-id="e3d7b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3d7b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3d7b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3d7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3d7b-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e3d7b-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e3d7b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3d7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3d7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-116">Not supported.</span></span>|
|<span data-ttu-id="e3d7b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3d7b-117">Application</span></span>|<span data-ttu-id="e3d7b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-118">Not supported.</span></span>|

<span data-ttu-id="e3d7b-119">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e3d7b-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="e3d7b-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e3d7b-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="e3d7b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3d7b-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="e3d7b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3d7b-122">Request headers</span></span>
|<span data-ttu-id="e3d7b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e3d7b-123">Name</span></span>|<span data-ttu-id="e3d7b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d7b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3d7b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3d7b-125">Authorization</span></span>|<span data-ttu-id="e3d7b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3d7b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3d7b-128">Request body</span></span>
<span data-ttu-id="e3d7b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3d7b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3d7b-130">Response</span></span>

<span data-ttu-id="e3d7b-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3d7b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e3d7b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3d7b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3d7b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3d7b-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e3d7b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3d7b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="e3d7b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e3d7b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3d7b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3d7b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3d7b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3d7b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3d7b-138">Java</span><span class="sxs-lookup"><span data-stu-id="e3d7b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e3d7b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3d7b-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

