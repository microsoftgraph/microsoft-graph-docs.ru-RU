---
title: Методы List
description: Извлечение списка объектов метода проверки подлинности.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 05606726178d2c1d2a2bb308f941810363e357c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048003"
---
# <a name="list-methods"></a><span data-ttu-id="0a013-103">Методы List</span><span class="sxs-lookup"><span data-stu-id="0a013-103">List methods</span></span>

<span data-ttu-id="0a013-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a013-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a013-105">Извлечение списка объектов метода [проверки подлинности.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="0a013-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a013-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a013-106">Permissions</span></span>

<span data-ttu-id="0a013-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="0a013-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="0a013-109">Permissions acting on self</span></span>

|<span data-ttu-id="0a013-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a013-110">Permission type</span></span>      | <span data-ttu-id="0a013-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a013-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0a013-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a013-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a013-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a013-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="0a013-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a013-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a013-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a013-115">Not supported.</span></span> |
| <span data-ttu-id="0a013-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a013-116">Application</span></span>                            | <span data-ttu-id="0a013-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a013-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="0a013-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="0a013-118">Permissions acting on other users</span></span>

|<span data-ttu-id="0a013-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a013-119">Permission type</span></span>      | <span data-ttu-id="0a013-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a013-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0a013-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a013-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a013-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a013-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0a013-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a013-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a013-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a013-124">Not supported.</span></span> |
| <span data-ttu-id="0a013-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a013-125">Application</span></span>                            | <span data-ttu-id="0a013-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a013-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="0a013-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="0a013-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="0a013-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0a013-128">Global admin</span></span>
* <span data-ttu-id="0a013-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="0a013-129">Global reader</span></span>
* <span data-ttu-id="0a013-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0a013-130">Privileged authentication admin</span></span>
* <span data-ttu-id="0a013-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="0a013-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="0a013-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a013-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a013-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a013-133">Optional query parameters</span></span>

<span data-ttu-id="0a013-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0a013-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a013-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a013-135">Request headers</span></span>

| <span data-ttu-id="0a013-136">Имя</span><span class="sxs-lookup"><span data-stu-id="0a013-136">Name</span></span>      |<span data-ttu-id="0a013-137">Описание</span><span class="sxs-lookup"><span data-stu-id="0a013-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a013-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a013-138">Authorization</span></span> | <span data-ttu-id="0a013-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a013-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a013-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a013-141">Request body</span></span>

<span data-ttu-id="0a013-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a013-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a013-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a013-143">Response</span></span>

<span data-ttu-id="0a013-144">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [authenticationMethod](../resources/authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a013-144">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a013-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a013-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a013-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a013-146">Request</span></span>

<span data-ttu-id="0a013-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a013-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a013-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a013-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="0a013-149">C#</span><span class="sxs-lookup"><span data-stu-id="0a013-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a013-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a013-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a013-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a013-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a013-152">Java</span><span class="sxs-lookup"><span data-stu-id="0a013-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-methods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a013-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a013-153">Response</span></span>

<span data-ttu-id="0a013-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0a013-154">The following is an example of the response.</span></span>

> <span data-ttu-id="0a013-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a013-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "odata.type": "#microsoft.graph.passwordAuthenticationMethod",
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "3179e48a-750b-4051-897c-87b9720928f7",
      "phoneNumber": "+1 2065555555",
      "authenticationPhoneType": "mobile",
      "smsSignInState": "ready"
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41",
      "phoneNumber": "+1 2065555556",
      "authenticationPhoneType": "alternateMobile",
      "smsSignInState": "notSupported"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
