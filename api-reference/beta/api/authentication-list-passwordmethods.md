---
title: Список passwordMethods
description: Извлечение списка объектов passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b0e03080bed41bc313e9cbe47f2e76b88999b66c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515480"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="64c13-103">Список passwordMethods</span><span class="sxs-lookup"><span data-stu-id="64c13-103">List passwordMethods</span></span>

<span data-ttu-id="64c13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64c13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64c13-105">Извлечение списка [объектов метода проверки подлинности паролей.](../resources/passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="64c13-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="64c13-106">Это возвращает ровно один объект, так как у пользователя может быть точно один пароль.</span><span class="sxs-lookup"><span data-stu-id="64c13-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c13-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64c13-107">Permissions</span></span>

<span data-ttu-id="64c13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="64c13-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="64c13-110">Permissions acting on self</span></span>

|<span data-ttu-id="64c13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c13-111">Permission type</span></span>      | <span data-ttu-id="64c13-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c13-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="64c13-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c13-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="64c13-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64c13-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="64c13-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c13-116">Not supported.</span></span> |
| <span data-ttu-id="64c13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64c13-117">Application</span></span>                            | <span data-ttu-id="64c13-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c13-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="64c13-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="64c13-119">Permissions acting on other users</span></span>

|<span data-ttu-id="64c13-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c13-120">Permission type</span></span>      | <span data-ttu-id="64c13-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c13-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="64c13-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c13-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="64c13-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c13-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="64c13-124">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c13-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c13-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c13-125">Not supported.</span></span> |
| <span data-ttu-id="64c13-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="64c13-126">Application</span></span>                            | <span data-ttu-id="64c13-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c13-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="64c13-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="64c13-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="64c13-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="64c13-129">Global admin</span></span>
* <span data-ttu-id="64c13-130">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="64c13-130">Global reader</span></span>
* <span data-ttu-id="64c13-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="64c13-131">Privileged authentication admin</span></span>
* <span data-ttu-id="64c13-132">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="64c13-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="64c13-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c13-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id | userPrincipalName}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64c13-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64c13-134">Optional query parameters</span></span>

<span data-ttu-id="64c13-135">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64c13-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64c13-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64c13-136">Request headers</span></span>

| <span data-ttu-id="64c13-137">Имя</span><span class="sxs-lookup"><span data-stu-id="64c13-137">Name</span></span>      |<span data-ttu-id="64c13-138">Описание</span><span class="sxs-lookup"><span data-stu-id="64c13-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64c13-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="64c13-139">Authorization</span></span> | <span data-ttu-id="64c13-140">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="64c13-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="64c13-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64c13-141">Request body</span></span>

<span data-ttu-id="64c13-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64c13-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64c13-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c13-143">Response</span></span>

<span data-ttu-id="64c13-144">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="64c13-144">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64c13-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="64c13-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64c13-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c13-146">Request</span></span>

<span data-ttu-id="64c13-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64c13-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64c13-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="64c13-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="64c13-149">C#</span><span class="sxs-lookup"><span data-stu-id="64c13-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64c13-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64c13-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64c13-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64c13-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64c13-152">Java</span><span class="sxs-lookup"><span data-stu-id="64c13-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordmethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64c13-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c13-153">Response</span></span>

<span data-ttu-id="64c13-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64c13-154">The following is an example of the response.</span></span>

> <span data-ttu-id="64c13-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64c13-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List passwordMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
