---
title: Список без пароляMicrosoftAuthenticatorAuthenticationMethods
description: Получить список объектов Без пароляMicrosoftAuthenticatorAuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4947304335ff59839dda00b9da554961c266fbc
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796670"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods-deprecated"></a><span data-ttu-id="8ff80-103">Список без пароляMicrosoftAuthenticatorAuthenticationMethods (неподготовлен)</span><span class="sxs-lookup"><span data-stu-id="8ff80-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods (deprecated)</span></span>
<span data-ttu-id="8ff80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff80-105">Получить список объектов метода microsoft [Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) user без пароля для телефона и их свойств.</span><span class="sxs-lookup"><span data-stu-id="8ff80-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!CAUTION]
> <span data-ttu-id="8ff80-106">API метода microsoft Authenticator Без пароля для телефона является неподготовленным и перестает возвращать результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8ff80-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="8ff80-107">Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="8ff80-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff80-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff80-108">Permissions</span></span>

<span data-ttu-id="8ff80-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="8ff80-111">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="8ff80-111">Permissions acting on self</span></span>

|<span data-ttu-id="8ff80-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff80-112">Permission type</span></span>      | <span data-ttu-id="8ff80-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ff80-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8ff80-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ff80-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ff80-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ff80-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="8ff80-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ff80-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ff80-117">Not supported.</span></span> |
| <span data-ttu-id="8ff80-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ff80-118">Application</span></span>                            | <span data-ttu-id="8ff80-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ff80-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="8ff80-120">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="8ff80-120">Permissions acting on other users</span></span>

|<span data-ttu-id="8ff80-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff80-121">Permission type</span></span>      | <span data-ttu-id="8ff80-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ff80-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="8ff80-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ff80-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ff80-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff80-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8ff80-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ff80-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff80-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ff80-126">Not supported.</span></span> |
| <span data-ttu-id="8ff80-127">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ff80-127">Application</span></span>                            | <span data-ttu-id="8ff80-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff80-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="8ff80-129">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="8ff80-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="8ff80-130">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8ff80-130">Global admin</span></span>
* <span data-ttu-id="8ff80-131">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="8ff80-131">Global reader</span></span>
* <span data-ttu-id="8ff80-132">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8ff80-132">Privileged authentication admin</span></span>
* <span data-ttu-id="8ff80-133">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="8ff80-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="8ff80-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ff80-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ff80-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8ff80-135">Optional query parameters</span></span>
<span data-ttu-id="8ff80-136">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8ff80-136">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ff80-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ff80-137">Request headers</span></span>
|<span data-ttu-id="8ff80-138">Имя</span><span class="sxs-lookup"><span data-stu-id="8ff80-138">Name</span></span>|<span data-ttu-id="8ff80-139">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff80-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8ff80-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ff80-140">Authorization</span></span>|<span data-ttu-id="8ff80-141">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8ff80-141">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff80-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ff80-142">Request body</span></span>
<span data-ttu-id="8ff80-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ff80-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff80-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff80-144">Response</span></span>

<span data-ttu-id="8ff80-145">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [Без пароляMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ff80-145">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ff80-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ff80-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ff80-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ff80-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8ff80-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff80-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="8ff80-149">C#</span><span class="sxs-lookup"><span data-stu-id="8ff80-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ff80-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ff80-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ff80-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ff80-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ff80-152">Java</span><span class="sxs-lookup"><span data-stu-id="8ff80-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8ff80-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff80-153">Response</span></span>
<span data-ttu-id="8ff80-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8ff80-154">The following is an example of the response.</span></span>

<span data-ttu-id="8ff80-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8ff80-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

