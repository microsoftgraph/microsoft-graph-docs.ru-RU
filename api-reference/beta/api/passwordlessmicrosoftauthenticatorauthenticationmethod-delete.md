---
title: Удаление без пароляMicrosoftAuthenticatorAuthenticationMethod
description: Удаляет объект PasswordlessMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5bd76dcb0652fdea395592ff916cd37eac789384
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515968"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="1174d-103">Удаление без пароляMicrosoftAuthenticatorAuthenticationMethod (обесценен)</span><span class="sxs-lookup"><span data-stu-id="1174d-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="1174d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1174d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1174d-105">Удаляет объект метода "Microsoft [Authenticator Passwordless Phone Sign-in"](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="1174d-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="1174d-106">API без пароля Microsoft Authenticator phone is deprecated and will stop returning results on 31 December 2020.</span><span class="sxs-lookup"><span data-stu-id="1174d-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="1174d-107">Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="1174d-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1174d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1174d-108">Permissions</span></span>

<span data-ttu-id="1174d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1174d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="1174d-111">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="1174d-111">Permissions acting on self</span></span>

|<span data-ttu-id="1174d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1174d-112">Permission type</span></span>      | <span data-ttu-id="1174d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1174d-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="1174d-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1174d-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1174d-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1174d-115">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="1174d-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1174d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1174d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1174d-117">Not supported.</span></span> |
| <span data-ttu-id="1174d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1174d-118">Application</span></span>                            | <span data-ttu-id="1174d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1174d-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="1174d-120">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="1174d-120">Permissions acting on other users</span></span>

|<span data-ttu-id="1174d-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1174d-121">Permission type</span></span>      | <span data-ttu-id="1174d-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1174d-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="1174d-123">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1174d-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="1174d-124">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1174d-124">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1174d-125">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1174d-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1174d-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1174d-126">Not supported.</span></span> |
| <span data-ttu-id="1174d-127">Приложение</span><span class="sxs-lookup"><span data-stu-id="1174d-127">Application</span></span>                            | <span data-ttu-id="1174d-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1174d-128">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="1174d-129">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1174d-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="1174d-130">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1174d-130">Global admin</span></span>
* <span data-ttu-id="1174d-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1174d-131">Privileged authentication admin</span></span>
* <span data-ttu-id="1174d-132">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1174d-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1174d-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1174d-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1174d-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1174d-134">Request headers</span></span>
|<span data-ttu-id="1174d-135">Имя</span><span class="sxs-lookup"><span data-stu-id="1174d-135">Name</span></span>|<span data-ttu-id="1174d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1174d-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1174d-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1174d-137">Authorization</span></span>|<span data-ttu-id="1174d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1174d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1174d-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1174d-140">Request body</span></span>
<span data-ttu-id="1174d-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1174d-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1174d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1174d-142">Response</span></span>

<span data-ttu-id="1174d-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1174d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1174d-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="1174d-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1174d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="1174d-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1174d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1174d-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="1174d-148">C#</span><span class="sxs-lookup"><span data-stu-id="1174d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1174d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1174d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1174d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1174d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1174d-151">Java</span><span class="sxs-lookup"><span data-stu-id="1174d-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1174d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1174d-152">Response</span></span>
<span data-ttu-id="1174d-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1174d-153">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

