---
title: Удаление windowsHelloForBusinessAuthenticationMethod
description: Удаляет объект windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: de3e491a5eef3f09b89134fdc45dbb9805b82627
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467948"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="6c242-103">Удаление windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c242-103">Delete windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="6c242-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c242-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c242-105">Удаляет [объект windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="6c242-105">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c242-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c242-106">Permissions</span></span>

<span data-ttu-id="6c242-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="6c242-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="6c242-109">Permissions acting on self</span></span>

|<span data-ttu-id="6c242-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c242-110">Permission type</span></span>      | <span data-ttu-id="6c242-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c242-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="6c242-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c242-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c242-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c242-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="6c242-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c242-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c242-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c242-115">Not supported.</span></span> |
| <span data-ttu-id="6c242-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c242-116">Application</span></span>                            | <span data-ttu-id="6c242-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c242-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="6c242-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="6c242-118">Permissions acting on other users</span></span>

|<span data-ttu-id="6c242-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c242-119">Permission type</span></span>      | <span data-ttu-id="6c242-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c242-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="6c242-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c242-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c242-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c242-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="6c242-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c242-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c242-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c242-124">Not supported.</span></span> |
| <span data-ttu-id="6c242-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c242-125">Application</span></span>                            | <span data-ttu-id="6c242-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c242-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="6c242-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="6c242-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="6c242-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6c242-128">Global admin</span></span>
* <span data-ttu-id="6c242-129">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6c242-129">Privileged authentication admin</span></span>
* <span data-ttu-id="6c242-130">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6c242-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6c242-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c242-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="6c242-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c242-132">Request headers</span></span>
|<span data-ttu-id="6c242-133">Имя</span><span class="sxs-lookup"><span data-stu-id="6c242-133">Name</span></span>|<span data-ttu-id="6c242-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6c242-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c242-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c242-135">Authorization</span></span>|<span data-ttu-id="6c242-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c242-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c242-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c242-138">Request body</span></span>
<span data-ttu-id="6c242-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c242-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c242-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c242-140">Response</span></span>

<span data-ttu-id="6c242-141">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c242-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6c242-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c242-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c242-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c242-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6c242-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c242-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="6c242-145">C#</span><span class="sxs-lookup"><span data-stu-id="6c242-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-windowshelloforbusinessauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c242-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c242-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-windowshelloforbusinessauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c242-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c242-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-windowshelloforbusinessauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c242-148">Java</span><span class="sxs-lookup"><span data-stu-id="6c242-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-windowshelloforbusinessauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6c242-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c242-149">Response</span></span>
<span data-ttu-id="6c242-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6c242-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

