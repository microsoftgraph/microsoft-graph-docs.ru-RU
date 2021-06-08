---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: Включить SMS для мобильного телефона.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1452d3e3e1c93def07dce3b6ee78a996c374ae0c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786474"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="34a64-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="34a64-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="34a64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34a64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34a64-105">Включить SMS для существующего номера `mobile` телефона.</span><span class="sxs-lookup"><span data-stu-id="34a64-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="34a64-106">Чтобы успешно включить:</span><span class="sxs-lookup"><span data-stu-id="34a64-106">To be successfully enabled:</span></span>

* <span data-ttu-id="34a64-107">Телефон должен иметь `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="34a64-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="34a64-108">Телефон должен быть уникальным в системе SMS регистрации (никто другой не может также использовать этот номер).</span><span class="sxs-lookup"><span data-stu-id="34a64-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="34a64-109">Пользователь должен быть включен для SMS входа в политику методов [проверки подлинности.](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="34a64-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="34a64-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34a64-110">Permissions</span></span>

<span data-ttu-id="34a64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="34a64-113">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="34a64-113">Permissions acting on self</span></span>

|<span data-ttu-id="34a64-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a64-114">Permission type</span></span>      | <span data-ttu-id="34a64-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a64-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="34a64-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a64-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="34a64-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a64-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="34a64-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a64-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a64-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a64-119">Not supported.</span></span> |
| <span data-ttu-id="34a64-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34a64-120">Application</span></span>                            | <span data-ttu-id="34a64-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a64-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="34a64-122">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="34a64-122">Permissions acting on other users</span></span>

|<span data-ttu-id="34a64-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a64-123">Permission type</span></span>      | <span data-ttu-id="34a64-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a64-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="34a64-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a64-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="34a64-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a64-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="34a64-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a64-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a64-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a64-128">Not supported.</span></span> |
| <span data-ttu-id="34a64-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="34a64-129">Application</span></span>                            | <span data-ttu-id="34a64-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a64-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="34a64-131">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="34a64-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="34a64-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="34a64-132">Global admin</span></span>
* <span data-ttu-id="34a64-133">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="34a64-133">Privileged authentication admin</span></span>
* <span data-ttu-id="34a64-134">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="34a64-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="34a64-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34a64-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```
<span data-ttu-id="34a64-136">Значение для `id` `mobile` phoneType `3179e48a-750b-4051-897c-87b9720928f7` — .</span><span class="sxs-lookup"><span data-stu-id="34a64-136">The value of `id` for the `mobile` phoneType is `3179e48a-750b-4051-897c-87b9720928f7`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34a64-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34a64-137">Request headers</span></span>

| <span data-ttu-id="34a64-138">Имя</span><span class="sxs-lookup"><span data-stu-id="34a64-138">Name</span></span>          | <span data-ttu-id="34a64-139">Описание</span><span class="sxs-lookup"><span data-stu-id="34a64-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="34a64-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34a64-140">Authorization</span></span> | <span data-ttu-id="34a64-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a64-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34a64-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34a64-143">Request body</span></span>

<span data-ttu-id="34a64-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34a64-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34a64-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a64-145">Response</span></span>

<span data-ttu-id="34a64-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="34a64-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34a64-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="34a64-148">Examples</span></span>

<span data-ttu-id="34a64-149">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="34a64-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="34a64-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="34a64-150">Request</span></span>

<span data-ttu-id="34a64-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34a64-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34a64-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="34a64-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="34a64-153">C#</span><span class="sxs-lookup"><span data-stu-id="34a64-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34a64-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34a64-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34a64-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34a64-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34a64-156">Java</span><span class="sxs-lookup"><span data-stu-id="34a64-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34a64-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a64-157">Response</span></span>

<span data-ttu-id="34a64-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="34a64-158">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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
