---
title: Get passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта Без пароляMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c96a20eb7439367e2054213d92be08a609217c24
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963017"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="b17b2-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span><span class="sxs-lookup"><span data-stu-id="b17b2-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="b17b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b17b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b17b2-105">Извлечение пользовательского единого [объекта метода microsoft Authenticator Passwordless Phone Sign-in.](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b17b2-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="b17b2-106">API без пароля Microsoft Authenticator phone is deprecated and will stop returning results on 31 December 2020.</span><span class="sxs-lookup"><span data-stu-id="b17b2-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="b17b2-107">Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="b17b2-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b17b2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b17b2-108">Permissions</span></span>

<span data-ttu-id="b17b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b17b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b17b2-111">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="b17b2-111">Permissions acting on self</span></span>

|<span data-ttu-id="b17b2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b17b2-112">Permission type</span></span>      | <span data-ttu-id="b17b2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b17b2-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b17b2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b17b2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b17b2-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b17b2-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b17b2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b17b2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b17b2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b17b2-117">Not supported.</span></span> |
| <span data-ttu-id="b17b2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b17b2-118">Application</span></span>                            | <span data-ttu-id="b17b2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b17b2-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b17b2-120">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="b17b2-120">Permissions acting on other users</span></span>

|<span data-ttu-id="b17b2-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b17b2-121">Permission type</span></span>      | <span data-ttu-id="b17b2-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b17b2-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b17b2-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b17b2-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="b17b2-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b17b2-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b17b2-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b17b2-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b17b2-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b17b2-126">Not supported.</span></span> |
| <span data-ttu-id="b17b2-127">Application</span><span class="sxs-lookup"><span data-stu-id="b17b2-127">Application</span></span>                            | <span data-ttu-id="b17b2-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b17b2-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b17b2-129">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b17b2-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b17b2-130">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b17b2-130">Global admin</span></span>
* <span data-ttu-id="b17b2-131">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="b17b2-131">Global reader</span></span>
* <span data-ttu-id="b17b2-132">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b17b2-132">Privileged authentication admin</span></span>
* <span data-ttu-id="b17b2-133">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="b17b2-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="b17b2-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b17b2-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b17b2-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b17b2-135">Request headers</span></span>
|<span data-ttu-id="b17b2-136">Имя</span><span class="sxs-lookup"><span data-stu-id="b17b2-136">Name</span></span>|<span data-ttu-id="b17b2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b17b2-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b17b2-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b17b2-138">Authorization</span></span>|<span data-ttu-id="b17b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b17b2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b17b2-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b17b2-141">Request body</span></span>
<span data-ttu-id="b17b2-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b17b2-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b17b2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b17b2-143">Response</span></span>

<span data-ttu-id="b17b2-144">В случае успешной работы этот метод возвращает код ответа и запрашивается без `200 OK` [пароляMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b17b2-144">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b17b2-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="b17b2-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b17b2-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b17b2-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b17b2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b17b2-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="b17b2-148">C#</span><span class="sxs-lookup"><span data-stu-id="b17b2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b17b2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b17b2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b17b2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b17b2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b17b2-151">Java</span><span class="sxs-lookup"><span data-stu-id="b17b2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b17b2-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b17b2-152">Response</span></span>
<span data-ttu-id="b17b2-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b17b2-153">The following is an example of the response.</span></span>

<span data-ttu-id="b17b2-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b17b2-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

