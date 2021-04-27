---
title: Get passwordAuthenticationMethod
description: Извлечение свойств и связей объекта passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 32aad6e260b0eeb4df87cd9daa51f59d0fa82416
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049179"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="354ef-103">Get passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="354ef-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="354ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="354ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="354ef-105">Извлечение свойств и связей объекта [метода проверки подлинности паролей.](../resources/passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="354ef-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="354ef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="354ef-106">Permissions</span></span>

<span data-ttu-id="354ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="354ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="354ef-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="354ef-109">Permissions acting on self</span></span>

|<span data-ttu-id="354ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="354ef-110">Permission type</span></span>      | <span data-ttu-id="354ef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="354ef-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="354ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="354ef-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="354ef-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="354ef-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="354ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="354ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="354ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="354ef-115">Not supported.</span></span> |
| <span data-ttu-id="354ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="354ef-116">Application</span></span>                            | <span data-ttu-id="354ef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="354ef-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="354ef-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="354ef-118">Permissions acting on other users</span></span>

|<span data-ttu-id="354ef-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="354ef-119">Permission type</span></span>      | <span data-ttu-id="354ef-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="354ef-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="354ef-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="354ef-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="354ef-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="354ef-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="354ef-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="354ef-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="354ef-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="354ef-124">Not supported.</span></span> |
| <span data-ttu-id="354ef-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="354ef-125">Application</span></span>                            | <span data-ttu-id="354ef-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="354ef-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="354ef-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="354ef-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="354ef-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="354ef-128">Global admin</span></span>
* <span data-ttu-id="354ef-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="354ef-129">Global reader</span></span>
* <span data-ttu-id="354ef-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="354ef-130">Privileged authentication admin</span></span>
* <span data-ttu-id="354ef-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="354ef-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="354ef-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="354ef-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="354ef-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="354ef-133">Optional query parameters</span></span>

<span data-ttu-id="354ef-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="354ef-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="354ef-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="354ef-135">Request headers</span></span>

| <span data-ttu-id="354ef-136">Имя</span><span class="sxs-lookup"><span data-stu-id="354ef-136">Name</span></span>      |<span data-ttu-id="354ef-137">Описание</span><span class="sxs-lookup"><span data-stu-id="354ef-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="354ef-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="354ef-138">Authorization</span></span> | <span data-ttu-id="354ef-139">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="354ef-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="354ef-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="354ef-140">Request body</span></span>

<span data-ttu-id="354ef-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="354ef-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="354ef-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="354ef-142">Response</span></span>

<span data-ttu-id="354ef-143">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [пароляAuthenticationMethod](../resources/passwordauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="354ef-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="354ef-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="354ef-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="354ef-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="354ef-145">Request</span></span>

<span data-ttu-id="354ef-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="354ef-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="354ef-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="354ef-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="354ef-148">C#</span><span class="sxs-lookup"><span data-stu-id="354ef-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="354ef-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="354ef-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="354ef-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="354ef-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="354ef-151">Java</span><span class="sxs-lookup"><span data-stu-id="354ef-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="354ef-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="354ef-152">Response</span></span>

<span data-ttu-id="354ef-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="354ef-153">The following is an example of the response.</span></span>

> <span data-ttu-id="354ef-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="354ef-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "28c10230-6103-485e-b985-444c60001490",
  "password": null,
  "creationDateTime": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get passwordAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
