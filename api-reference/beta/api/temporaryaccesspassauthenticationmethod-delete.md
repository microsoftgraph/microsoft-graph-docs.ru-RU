---
title: Удаление temporaryAccessPassAuthenticationMethod
description: Удаляет объект temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 31879dfc0d572f1914b15582ec515b0f8a44c85a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475134"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="468c1-103">Удаление temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="468c1-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="468c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="468c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="468c1-105">Удаление [объекта temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="468c1-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="468c1-106">Несмотря на то, что текущий временный пропуск доступа для пользователя действителен, его необходимо удалить, прежде чем будет создан новый временный пропуск доступа для пользователя.</span><span class="sxs-lookup"><span data-stu-id="468c1-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="468c1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="468c1-107">Permissions</span></span>
<span data-ttu-id="468c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="468c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="468c1-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="468c1-110">Permissions acting on self</span></span>

|<span data-ttu-id="468c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="468c1-111">Permission type</span></span>      | <span data-ttu-id="468c1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="468c1-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="468c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="468c1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="468c1-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="468c1-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="468c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="468c1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="468c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468c1-116">Not supported.</span></span> |
| <span data-ttu-id="468c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="468c1-117">Application</span></span>                            | <span data-ttu-id="468c1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468c1-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="468c1-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="468c1-119">Permissions acting on other users</span></span>

|<span data-ttu-id="468c1-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="468c1-120">Permission type</span></span>      | <span data-ttu-id="468c1-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="468c1-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="468c1-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="468c1-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="468c1-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468c1-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="468c1-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="468c1-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="468c1-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468c1-125">Not supported.</span></span> |
| <span data-ttu-id="468c1-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="468c1-126">Application</span></span>                            | <span data-ttu-id="468c1-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468c1-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="468c1-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="468c1-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="468c1-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="468c1-129">Global admin</span></span>
* <span data-ttu-id="468c1-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="468c1-130">Privileged authentication admin</span></span>
* <span data-ttu-id="468c1-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="468c1-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="468c1-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="468c1-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="468c1-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="468c1-133">Request headers</span></span>
|<span data-ttu-id="468c1-134">Имя</span><span class="sxs-lookup"><span data-stu-id="468c1-134">Name</span></span>|<span data-ttu-id="468c1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="468c1-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="468c1-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="468c1-136">Authorization</span></span>|<span data-ttu-id="468c1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="468c1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="468c1-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="468c1-139">Request body</span></span>
<span data-ttu-id="468c1-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="468c1-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="468c1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="468c1-141">Response</span></span>

<span data-ttu-id="468c1-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="468c1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="468c1-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="468c1-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="468c1-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="468c1-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="468c1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="468c1-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="468c1-147">C#</span><span class="sxs-lookup"><span data-stu-id="468c1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="468c1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="468c1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="468c1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="468c1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="468c1-150">Java</span><span class="sxs-lookup"><span data-stu-id="468c1-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="468c1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="468c1-151">Response</span></span>
<span data-ttu-id="468c1-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="468c1-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
