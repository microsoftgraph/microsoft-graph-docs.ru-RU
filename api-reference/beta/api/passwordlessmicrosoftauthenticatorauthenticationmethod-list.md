---
title: Список без паролейMicrosoftAuthenticatorAuthenticationMethods
description: Извлечение списка объектов без пароляMicrosoftAuthenticatorAuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 162ef913cbc69431e40365a447440f77a711dac1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962999"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods-deprecated"></a><span data-ttu-id="5636a-103">Список без паролейMicrosoftAuthenticatorAuthenticationMethods (обесценен)</span><span class="sxs-lookup"><span data-stu-id="5636a-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods (deprecated)</span></span>
<span data-ttu-id="5636a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5636a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5636a-105">Извлечение списка объектов метода регистрации без паролей [Microsoft Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5636a-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!CAUTION]
> <span data-ttu-id="5636a-106">API без пароля Microsoft Authenticator phone is deprecated and will stop returning results on 31 December 2020.</span><span class="sxs-lookup"><span data-stu-id="5636a-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="5636a-107">Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="5636a-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5636a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5636a-108">Permissions</span></span>

<span data-ttu-id="5636a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5636a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="5636a-111">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="5636a-111">Permissions acting on self</span></span>

|<span data-ttu-id="5636a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5636a-112">Permission type</span></span>      | <span data-ttu-id="5636a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5636a-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="5636a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5636a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5636a-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5636a-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="5636a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5636a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5636a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5636a-117">Not supported.</span></span> |
| <span data-ttu-id="5636a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5636a-118">Application</span></span>                            | <span data-ttu-id="5636a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5636a-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="5636a-120">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="5636a-120">Permissions acting on other users</span></span>

|<span data-ttu-id="5636a-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5636a-121">Permission type</span></span>      | <span data-ttu-id="5636a-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5636a-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="5636a-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5636a-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="5636a-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5636a-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="5636a-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5636a-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5636a-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5636a-126">Not supported.</span></span> |
| <span data-ttu-id="5636a-127">Application</span><span class="sxs-lookup"><span data-stu-id="5636a-127">Application</span></span>                            | <span data-ttu-id="5636a-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5636a-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="5636a-129">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="5636a-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="5636a-130">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5636a-130">Global admin</span></span>
* <span data-ttu-id="5636a-131">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="5636a-131">Global reader</span></span>
* <span data-ttu-id="5636a-132">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="5636a-132">Privileged authentication admin</span></span>
* <span data-ttu-id="5636a-133">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="5636a-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="5636a-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5636a-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5636a-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5636a-135">Optional query parameters</span></span>
<span data-ttu-id="5636a-136">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5636a-136">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5636a-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5636a-137">Request headers</span></span>
|<span data-ttu-id="5636a-138">Имя</span><span class="sxs-lookup"><span data-stu-id="5636a-138">Name</span></span>|<span data-ttu-id="5636a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5636a-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5636a-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="5636a-140">Authorization</span></span>|<span data-ttu-id="5636a-141">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5636a-141">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5636a-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5636a-142">Request body</span></span>
<span data-ttu-id="5636a-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5636a-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5636a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5636a-144">Response</span></span>

<span data-ttu-id="5636a-145">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` без паролейMicrosoftAuthenticatorAuthenticationMethod в теле отклика. [](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="5636a-145">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5636a-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="5636a-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5636a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="5636a-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5636a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="5636a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="5636a-149">C#</span><span class="sxs-lookup"><span data-stu-id="5636a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5636a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5636a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5636a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5636a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5636a-152">Java</span><span class="sxs-lookup"><span data-stu-id="5636a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5636a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5636a-153">Response</span></span>
<span data-ttu-id="5636a-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5636a-154">The following is an example of the response.</span></span>

<span data-ttu-id="5636a-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5636a-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
    },
    {
      "id": "J18B378Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJGM1",
      "displayName": "My tablet",
      "creationDateTime": "2020-09-02T03:36:19Z"
    }
  ]
}
```

