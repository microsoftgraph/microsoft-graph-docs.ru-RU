---
title: Удаление temporaryAccessPassAuthenticationMethod
description: Удаляет объект temporaryAccessPassAuthenticationMethod.
author: inbarckMS
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5c9046137e5c8de5420a14f5c313c30e5f47fac1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049683"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="21994-103">Удаление temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="21994-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="21994-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21994-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21994-105">Удаление [объекта temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="21994-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="21994-106">Несмотря на то, что текущий временный пропуск доступа для пользователя действителен, его необходимо удалить, прежде чем будет создан новый временный пропуск доступа для пользователя.</span><span class="sxs-lookup"><span data-stu-id="21994-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="21994-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21994-107">Permissions</span></span>
<span data-ttu-id="21994-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="21994-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="21994-110">Permissions acting on self</span></span>

|<span data-ttu-id="21994-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21994-111">Permission type</span></span>      | <span data-ttu-id="21994-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21994-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="21994-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21994-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="21994-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21994-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="21994-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21994-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21994-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21994-116">Not supported.</span></span> |
| <span data-ttu-id="21994-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21994-117">Application</span></span>                            | <span data-ttu-id="21994-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21994-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="21994-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="21994-119">Permissions acting on other users</span></span>

|<span data-ttu-id="21994-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21994-120">Permission type</span></span>      | <span data-ttu-id="21994-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21994-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="21994-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21994-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="21994-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21994-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="21994-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21994-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21994-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21994-125">Not supported.</span></span> |
| <span data-ttu-id="21994-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="21994-126">Application</span></span>                            | <span data-ttu-id="21994-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21994-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="21994-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="21994-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="21994-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="21994-129">Global admin</span></span>
* <span data-ttu-id="21994-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="21994-130">Privileged authentication admin</span></span>
* <span data-ttu-id="21994-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="21994-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="21994-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21994-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21994-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21994-133">Request headers</span></span>
|<span data-ttu-id="21994-134">Имя</span><span class="sxs-lookup"><span data-stu-id="21994-134">Name</span></span>|<span data-ttu-id="21994-135">Описание</span><span class="sxs-lookup"><span data-stu-id="21994-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="21994-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21994-136">Authorization</span></span>|<span data-ttu-id="21994-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21994-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21994-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21994-139">Request body</span></span>
<span data-ttu-id="21994-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21994-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21994-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="21994-141">Response</span></span>

<span data-ttu-id="21994-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21994-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21994-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="21994-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21994-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="21994-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="21994-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="21994-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="21994-147">C#</span><span class="sxs-lookup"><span data-stu-id="21994-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21994-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21994-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21994-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21994-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21994-150">Java</span><span class="sxs-lookup"><span data-stu-id="21994-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="21994-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="21994-151">Response</span></span>
<span data-ttu-id="21994-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21994-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
