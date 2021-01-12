---
title: Удаление без пароляMicrosoftAuthenticatorAuthenticationMethod
description: Удаляет объект Без пароляMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e894cd8332969e708c8a7d8d1a53ca7c17be2dc
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796565"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="66279-103">Удаление без пароляMicrosoftAuthenticatorAuthenticationMethod (неподготовлено)</span><span class="sxs-lookup"><span data-stu-id="66279-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="66279-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66279-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66279-105">Удаляет объект метода для пользователя [Microsoft Authenticator Без](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) пароля для телефона для входов в учетную запись.</span><span class="sxs-lookup"><span data-stu-id="66279-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="66279-106">API метода microsoft Authenticator Без пароля для телефона является неподготовленным и перестает возвращать результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="66279-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="66279-107">Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="66279-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66279-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66279-108">Permissions</span></span>

<span data-ttu-id="66279-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66279-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="66279-111">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="66279-111">Permissions acting on self</span></span>

|<span data-ttu-id="66279-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66279-112">Permission type</span></span>      | <span data-ttu-id="66279-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66279-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="66279-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66279-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="66279-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66279-115">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="66279-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66279-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66279-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66279-117">Not supported.</span></span> |
| <span data-ttu-id="66279-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66279-118">Application</span></span>                            | <span data-ttu-id="66279-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66279-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="66279-120">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="66279-120">Permissions acting on other users</span></span>

|<span data-ttu-id="66279-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66279-121">Permission type</span></span>      | <span data-ttu-id="66279-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66279-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="66279-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66279-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="66279-124">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66279-124">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="66279-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66279-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66279-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66279-126">Not supported.</span></span> |
| <span data-ttu-id="66279-127">Приложение</span><span class="sxs-lookup"><span data-stu-id="66279-127">Application</span></span>                            | <span data-ttu-id="66279-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66279-128">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="66279-129">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="66279-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="66279-130">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="66279-130">Global admin</span></span>
* <span data-ttu-id="66279-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="66279-131">Privileged authentication admin</span></span>
* <span data-ttu-id="66279-132">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="66279-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="66279-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66279-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66279-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66279-134">Request headers</span></span>
|<span data-ttu-id="66279-135">Имя</span><span class="sxs-lookup"><span data-stu-id="66279-135">Name</span></span>|<span data-ttu-id="66279-136">Описание</span><span class="sxs-lookup"><span data-stu-id="66279-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="66279-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66279-137">Authorization</span></span>|<span data-ttu-id="66279-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66279-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66279-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66279-140">Request body</span></span>
<span data-ttu-id="66279-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66279-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66279-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="66279-142">Response</span></span>

<span data-ttu-id="66279-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="66279-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66279-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="66279-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66279-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="66279-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="66279-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="66279-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="66279-148">C#</span><span class="sxs-lookup"><span data-stu-id="66279-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66279-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66279-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66279-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66279-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66279-151">Java</span><span class="sxs-lookup"><span data-stu-id="66279-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="66279-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="66279-152">Response</span></span>
<span data-ttu-id="66279-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="66279-153">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

