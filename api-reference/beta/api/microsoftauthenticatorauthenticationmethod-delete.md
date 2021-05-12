---
title: Удаление MicrosoftAuthenticatorAuthenticationMethod
description: Удаляет объект MicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6d81e3a2ebf0cdbcea426d51cfcd1f3c9686cb1d
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335683"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="e3f5a-103">Удаление MicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e3f5a-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="e3f5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f5a-105">Удаляет объект [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3f5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3f5a-106">Permissions</span></span>

<span data-ttu-id="e3f5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="e3f5a-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="e3f5a-109">Permissions acting on self</span></span>

|<span data-ttu-id="e3f5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3f5a-110">Permission type</span></span>      | <span data-ttu-id="e3f5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e3f5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3f5a-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3f5a-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="e3f5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3f5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-115">Not supported.</span></span> |
| <span data-ttu-id="e3f5a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3f5a-116">Application</span></span>                            | <span data-ttu-id="e3f5a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="e3f5a-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="e3f5a-118">Permissions acting on other users</span></span>

|<span data-ttu-id="e3f5a-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3f5a-119">Permission type</span></span>      | <span data-ttu-id="e3f5a-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e3f5a-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3f5a-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f5a-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e3f5a-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3f5a-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-124">Not supported.</span></span> |
| <span data-ttu-id="e3f5a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3f5a-125">Application</span></span>                            | <span data-ttu-id="e3f5a-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f5a-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e3f5a-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e3f5a-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="e3f5a-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e3f5a-128">Global admin</span></span>
* <span data-ttu-id="e3f5a-129">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e3f5a-129">Privileged authentication admin</span></span>
* <span data-ttu-id="e3f5a-130">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e3f5a-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e3f5a-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3f5a-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="e3f5a-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3f5a-132">Request headers</span></span>
|<span data-ttu-id="e3f5a-133">Имя</span><span class="sxs-lookup"><span data-stu-id="e3f5a-133">Name</span></span>|<span data-ttu-id="e3f5a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e3f5a-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3f5a-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3f5a-135">Authorization</span></span>|<span data-ttu-id="e3f5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3f5a-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3f5a-138">Request body</span></span>
<span data-ttu-id="e3f5a-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3f5a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3f5a-140">Response</span></span>

<span data-ttu-id="e3f5a-141">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e3f5a-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3f5a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3f5a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3f5a-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e3f5a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3f5a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="e3f5a-145">C#</span><span class="sxs-lookup"><span data-stu-id="e3f5a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3f5a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3f5a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3f5a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3f5a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3f5a-148">Java</span><span class="sxs-lookup"><span data-stu-id="e3f5a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e3f5a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3f5a-149">Response</span></span>
<span data-ttu-id="e3f5a-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3f5a-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

