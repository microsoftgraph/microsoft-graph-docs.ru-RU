---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: Отключение sms-входов для мобильного телефона
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5e4440c5fac4a774b264b068a6e1e17d3d7c7d83
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796635"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="91b07-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="91b07-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="91b07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b07-105">Отключать вход с помощью SMS для существующего `mobile` номера телефона.</span><span class="sxs-lookup"><span data-stu-id="91b07-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="91b07-106">**Примечание.** Номер больше не будет доступен для sms-входов, что может препятствовать входу пользователя.</span><span class="sxs-lookup"><span data-stu-id="91b07-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="91b07-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91b07-107">Permissions</span></span>

<span data-ttu-id="91b07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="91b07-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="91b07-110">Permissions acting on self</span></span>

|<span data-ttu-id="91b07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91b07-111">Permission type</span></span>      | <span data-ttu-id="91b07-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91b07-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="91b07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91b07-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="91b07-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91b07-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="91b07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91b07-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91b07-116">Not supported.</span></span> |
| <span data-ttu-id="91b07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91b07-117">Application</span></span>                            | <span data-ttu-id="91b07-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91b07-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="91b07-119">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="91b07-119">Permissions acting on other users</span></span>

|<span data-ttu-id="91b07-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91b07-120">Permission type</span></span>      | <span data-ttu-id="91b07-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91b07-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="91b07-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91b07-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="91b07-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b07-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="91b07-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91b07-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b07-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91b07-125">Not supported.</span></span> |
| <span data-ttu-id="91b07-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="91b07-126">Application</span></span>                            | <span data-ttu-id="91b07-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b07-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="91b07-128">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="91b07-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="91b07-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="91b07-129">Global admin</span></span>
* <span data-ttu-id="91b07-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="91b07-130">Privileged authentication admin</span></span>
* <span data-ttu-id="91b07-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="91b07-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="91b07-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91b07-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="91b07-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91b07-133">Request headers</span></span>

| <span data-ttu-id="91b07-134">Имя</span><span class="sxs-lookup"><span data-stu-id="91b07-134">Name</span></span>          | <span data-ttu-id="91b07-135">Описание</span><span class="sxs-lookup"><span data-stu-id="91b07-135">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="91b07-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91b07-136">Authorization</span></span> | <span data-ttu-id="91b07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91b07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b07-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91b07-139">Request body</span></span>

<span data-ttu-id="91b07-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91b07-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91b07-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="91b07-141">Response</span></span>

<span data-ttu-id="91b07-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91b07-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91b07-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="91b07-144">Examples</span></span>

<span data-ttu-id="91b07-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="91b07-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="91b07-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="91b07-146">Request</span></span>

<span data-ttu-id="91b07-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91b07-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91b07-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b07-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="91b07-149">C#</span><span class="sxs-lookup"><span data-stu-id="91b07-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b07-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b07-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b07-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b07-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91b07-152">Java</span><span class="sxs-lookup"><span data-stu-id="91b07-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91b07-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="91b07-153">Response</span></span>

<span data-ttu-id="91b07-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91b07-154">The following is an example of the response.</span></span>
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
