---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: Включить вход с помощью SMS для мобильного телефона.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e2c8087005f65ac74a202ea43d90767172267a46
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796607"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="0d456-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="0d456-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="0d456-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d456-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d456-105">Включить вход с помощью SMS для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="0d456-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="0d456-106">Чтобы успешно включить:</span><span class="sxs-lookup"><span data-stu-id="0d456-106">To be successfully enabled:</span></span>

* <span data-ttu-id="0d456-107">Телефон должен иметь `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="0d456-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="0d456-108">Телефон должен быть уникальным в системе sms-входов (никто больше не может использовать этот номер).</span><span class="sxs-lookup"><span data-stu-id="0d456-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="0d456-109">Пользователю необходимо включить вход с помощью SMS в политике [методов проверки подлинности.](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="0d456-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d456-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d456-110">Permissions</span></span>

<span data-ttu-id="0d456-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d456-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="0d456-113">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="0d456-113">Permissions acting on self</span></span>

|<span data-ttu-id="0d456-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d456-114">Permission type</span></span>      | <span data-ttu-id="0d456-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d456-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0d456-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d456-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d456-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d456-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="0d456-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d456-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d456-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d456-119">Not supported.</span></span> |
| <span data-ttu-id="0d456-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d456-120">Application</span></span>                            | <span data-ttu-id="0d456-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d456-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="0d456-122">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="0d456-122">Permissions acting on other users</span></span>

|<span data-ttu-id="0d456-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d456-123">Permission type</span></span>      | <span data-ttu-id="0d456-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d456-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="0d456-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d456-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d456-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d456-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0d456-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d456-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d456-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d456-128">Not supported.</span></span> |
| <span data-ttu-id="0d456-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d456-129">Application</span></span>                            | <span data-ttu-id="0d456-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d456-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="0d456-131">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="0d456-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="0d456-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0d456-132">Global admin</span></span>
* <span data-ttu-id="0d456-133">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0d456-133">Privileged authentication admin</span></span>
* <span data-ttu-id="0d456-134">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0d456-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0d456-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d456-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="0d456-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d456-136">Request headers</span></span>

| <span data-ttu-id="0d456-137">Имя</span><span class="sxs-lookup"><span data-stu-id="0d456-137">Name</span></span>          | <span data-ttu-id="0d456-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0d456-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0d456-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d456-139">Authorization</span></span> | <span data-ttu-id="0d456-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d456-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d456-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d456-142">Request body</span></span>

<span data-ttu-id="0d456-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d456-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d456-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d456-144">Response</span></span>

<span data-ttu-id="0d456-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d456-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d456-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="0d456-147">Examples</span></span>

<span data-ttu-id="0d456-148">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0d456-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0d456-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d456-149">Request</span></span>

<span data-ttu-id="0d456-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d456-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d456-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d456-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="0d456-152">C#</span><span class="sxs-lookup"><span data-stu-id="0d456-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d456-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d456-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d456-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d456-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d456-155">Java</span><span class="sxs-lookup"><span data-stu-id="0d456-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d456-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d456-156">Response</span></span>

<span data-ttu-id="0d456-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0d456-157">The following is an example of the response.</span></span>
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
