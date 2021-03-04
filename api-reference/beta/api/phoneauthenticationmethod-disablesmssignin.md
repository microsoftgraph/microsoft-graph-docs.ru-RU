---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: Отключение sms-регистрации для мобильного телефона
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 235257c4df9c24dec33aad15e11b2318e0fb8e30
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447729"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="53688-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="53688-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="53688-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53688-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53688-105">Отключение sms-регистрации для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="53688-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="53688-106">**Примечание:** Номер больше не будет доступен для регистрации SMS, что может помешать входу пользователя.</span><span class="sxs-lookup"><span data-stu-id="53688-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="53688-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53688-107">Permissions</span></span>

<span data-ttu-id="53688-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="53688-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="53688-110">Permissions acting on self</span></span>

|<span data-ttu-id="53688-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53688-111">Permission type</span></span>      | <span data-ttu-id="53688-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53688-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="53688-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53688-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="53688-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53688-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="53688-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53688-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53688-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53688-116">Not supported.</span></span> |
| <span data-ttu-id="53688-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53688-117">Application</span></span>                            | <span data-ttu-id="53688-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53688-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="53688-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="53688-119">Permissions acting on other users</span></span>

|<span data-ttu-id="53688-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53688-120">Permission type</span></span>      | <span data-ttu-id="53688-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53688-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="53688-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53688-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="53688-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53688-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="53688-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53688-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53688-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53688-125">Not supported.</span></span> |
| <span data-ttu-id="53688-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="53688-126">Application</span></span>                            | <span data-ttu-id="53688-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53688-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="53688-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="53688-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="53688-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="53688-129">Global admin</span></span>
* <span data-ttu-id="53688-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="53688-130">Privileged authentication admin</span></span>
* <span data-ttu-id="53688-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="53688-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="53688-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53688-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="53688-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53688-133">Request headers</span></span>

| <span data-ttu-id="53688-134">Имя</span><span class="sxs-lookup"><span data-stu-id="53688-134">Name</span></span>          | <span data-ttu-id="53688-135">Описание</span><span class="sxs-lookup"><span data-stu-id="53688-135">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53688-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53688-136">Authorization</span></span> | <span data-ttu-id="53688-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53688-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53688-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53688-139">Request body</span></span>

<span data-ttu-id="53688-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53688-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53688-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="53688-141">Response</span></span>

<span data-ttu-id="53688-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53688-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53688-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="53688-144">Examples</span></span>

<span data-ttu-id="53688-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="53688-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="53688-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="53688-146">Request</span></span>

<span data-ttu-id="53688-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53688-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53688-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="53688-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="53688-149">C#</span><span class="sxs-lookup"><span data-stu-id="53688-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53688-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53688-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53688-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53688-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53688-152">Java</span><span class="sxs-lookup"><span data-stu-id="53688-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53688-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="53688-153">Response</span></span>

<span data-ttu-id="53688-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53688-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: disableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
