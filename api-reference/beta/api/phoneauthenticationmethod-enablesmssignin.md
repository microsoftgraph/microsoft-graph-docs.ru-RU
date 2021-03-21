---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: Включить вход в SMS для мобильного телефона.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: def7c4409ea38adf1764a7b3f1adf1d9280b992a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957315"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="8b387-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="8b387-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="8b387-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b387-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b387-105">Включить вход в SMS для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="8b387-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="8b387-106">Чтобы успешно включить:</span><span class="sxs-lookup"><span data-stu-id="8b387-106">To be successfully enabled:</span></span>

* <span data-ttu-id="8b387-107">Телефон должен иметь `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="8b387-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="8b387-108">Телефон должен быть уникальным в системе регистрации SMS (никто другой не может использовать этот номер).</span><span class="sxs-lookup"><span data-stu-id="8b387-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="8b387-109">Пользователь должен быть включен для входа в SMS в политике [методов проверки подлинности.](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="8b387-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b387-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b387-110">Permissions</span></span>

<span data-ttu-id="8b387-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b387-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="8b387-113">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="8b387-113">Permissions acting on self</span></span>

|<span data-ttu-id="8b387-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b387-114">Permission type</span></span>      | <span data-ttu-id="8b387-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b387-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8b387-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b387-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b387-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b387-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="8b387-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b387-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b387-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b387-119">Not supported.</span></span> |
| <span data-ttu-id="8b387-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b387-120">Application</span></span>                            | <span data-ttu-id="8b387-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b387-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="8b387-122">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="8b387-122">Permissions acting on other users</span></span>

|<span data-ttu-id="8b387-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b387-123">Permission type</span></span>      | <span data-ttu-id="8b387-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b387-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8b387-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b387-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b387-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b387-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8b387-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b387-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b387-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b387-128">Not supported.</span></span> |
| <span data-ttu-id="8b387-129">Application</span><span class="sxs-lookup"><span data-stu-id="8b387-129">Application</span></span>                            | <span data-ttu-id="8b387-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b387-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="8b387-131">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="8b387-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="8b387-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8b387-132">Global admin</span></span>
* <span data-ttu-id="8b387-133">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8b387-133">Privileged authentication admin</span></span>
* <span data-ttu-id="8b387-134">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8b387-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="8b387-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b387-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```
<span data-ttu-id="8b387-136">Значение для `id` `mobile` phoneType `3179e48a-750b-4051-897c-87b9720928f7` — .</span><span class="sxs-lookup"><span data-stu-id="8b387-136">The value of `id` for the `mobile` phoneType is `3179e48a-750b-4051-897c-87b9720928f7`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b387-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b387-137">Request headers</span></span>

| <span data-ttu-id="8b387-138">Имя</span><span class="sxs-lookup"><span data-stu-id="8b387-138">Name</span></span>          | <span data-ttu-id="8b387-139">Описание</span><span class="sxs-lookup"><span data-stu-id="8b387-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b387-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b387-140">Authorization</span></span> | <span data-ttu-id="8b387-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b387-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b387-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b387-143">Request body</span></span>

<span data-ttu-id="8b387-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b387-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b387-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b387-145">Response</span></span>

<span data-ttu-id="8b387-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b387-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b387-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b387-148">Examples</span></span>

<span data-ttu-id="8b387-149">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8b387-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8b387-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b387-150">Request</span></span>

<span data-ttu-id="8b387-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b387-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b387-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b387-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="8b387-153">C#</span><span class="sxs-lookup"><span data-stu-id="8b387-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b387-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b387-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b387-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b387-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b387-156">Java</span><span class="sxs-lookup"><span data-stu-id="8b387-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b387-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b387-157">Response</span></span>

<span data-ttu-id="8b387-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8b387-158">The following is an example of the response.</span></span>
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
  "description": "phoneAuthenticationMethod: enableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
