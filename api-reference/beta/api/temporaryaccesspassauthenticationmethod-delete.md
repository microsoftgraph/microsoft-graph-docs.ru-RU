---
title: Удаление temporaryAccessPassAuthenticationMethod
description: Удаляет объект temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 590a0d3d7581b0d8f1b109351c9c563812a973e6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761509"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="bbe5a-103">Удаление temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bbe5a-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="bbe5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbe5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe5a-105">Удаление [объекта temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="bbe5a-106">Несмотря на то, что текущий временный пропуск доступа для пользователя действителен, его необходимо удалить, прежде чем будет создан новый временный пропуск доступа для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbe5a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbe5a-107">Permissions</span></span>
<span data-ttu-id="bbe5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbe5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="bbe5a-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="bbe5a-110">Permissions acting on self</span></span>

|<span data-ttu-id="bbe5a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbe5a-111">Permission type</span></span>      | <span data-ttu-id="bbe5a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="bbe5a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbe5a-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbe5a-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="bbe5a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbe5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-116">Not supported.</span></span> |
| <span data-ttu-id="bbe5a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbe5a-117">Application</span></span>                            | <span data-ttu-id="bbe5a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="bbe5a-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="bbe5a-119">Permissions acting on other users</span></span>

|<span data-ttu-id="bbe5a-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbe5a-120">Permission type</span></span>      | <span data-ttu-id="bbe5a-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="bbe5a-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbe5a-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe5a-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="bbe5a-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbe5a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-125">Not supported.</span></span> |
| <span data-ttu-id="bbe5a-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbe5a-126">Application</span></span>                            | <span data-ttu-id="bbe5a-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe5a-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="bbe5a-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="bbe5a-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="bbe5a-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="bbe5a-129">Global admin</span></span>
* <span data-ttu-id="bbe5a-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="bbe5a-130">Privileged authentication admin</span></span>
* <span data-ttu-id="bbe5a-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="bbe5a-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="bbe5a-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbe5a-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bbe5a-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbe5a-133">Request headers</span></span>
|<span data-ttu-id="bbe5a-134">Имя</span><span class="sxs-lookup"><span data-stu-id="bbe5a-134">Name</span></span>|<span data-ttu-id="bbe5a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="bbe5a-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bbe5a-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbe5a-136">Authorization</span></span>|<span data-ttu-id="bbe5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbe5a-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbe5a-139">Request body</span></span>
<span data-ttu-id="bbe5a-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbe5a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbe5a-141">Response</span></span>

<span data-ttu-id="bbe5a-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbe5a-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="bbe5a-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bbe5a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbe5a-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bbe5a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbe5a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="bbe5a-147">C#</span><span class="sxs-lookup"><span data-stu-id="bbe5a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbe5a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbe5a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbe5a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe5a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbe5a-150">Java</span><span class="sxs-lookup"><span data-stu-id="bbe5a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bbe5a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbe5a-151">Response</span></span>
<span data-ttu-id="bbe5a-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bbe5a-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
