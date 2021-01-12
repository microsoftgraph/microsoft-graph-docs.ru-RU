---
title: Методы List
description: Получить список объектов метода проверки подлинности.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac205663b183e91b0925a3c246e9dd5a78c9aeba
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796558"
---
# <a name="list-methods"></a><span data-ttu-id="26273-103">Методы List</span><span class="sxs-lookup"><span data-stu-id="26273-103">List methods</span></span>

<span data-ttu-id="26273-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26273-105">Получить список объектов [метода проверки подлинности.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="26273-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span> <span data-ttu-id="26273-106">В [настоящее время возвращаются только объекты](../resources/phoneauthenticationmethod.md) [метода](../resources/passwordauthenticationmethod.md) проверки подлинности по телефону и пароля.</span><span class="sxs-lookup"><span data-stu-id="26273-106">Currently only [phone authentication method](../resources/phoneauthenticationmethod.md) and [password authentication method](../resources/passwordauthenticationmethod.md) objects are returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="26273-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26273-107">Permissions</span></span>

<span data-ttu-id="26273-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26273-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="26273-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="26273-110">Permissions acting on self</span></span>

|<span data-ttu-id="26273-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26273-111">Permission type</span></span>      | <span data-ttu-id="26273-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26273-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="26273-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26273-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="26273-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26273-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="26273-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26273-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26273-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26273-116">Not supported.</span></span> |
| <span data-ttu-id="26273-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26273-117">Application</span></span>                            | <span data-ttu-id="26273-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26273-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="26273-119">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="26273-119">Permissions acting on other users</span></span>

|<span data-ttu-id="26273-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26273-120">Permission type</span></span>      | <span data-ttu-id="26273-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26273-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="26273-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26273-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="26273-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26273-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="26273-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26273-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26273-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26273-125">Not supported.</span></span> |
| <span data-ttu-id="26273-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="26273-126">Application</span></span>                            | <span data-ttu-id="26273-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26273-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="26273-128">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="26273-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="26273-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="26273-129">Global admin</span></span>
* <span data-ttu-id="26273-130">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="26273-130">Global reader</span></span>
* <span data-ttu-id="26273-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="26273-131">Privileged authentication admin</span></span>
* <span data-ttu-id="26273-132">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="26273-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="26273-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26273-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26273-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26273-134">Optional query parameters</span></span>

<span data-ttu-id="26273-135">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="26273-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26273-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26273-136">Request headers</span></span>

| <span data-ttu-id="26273-137">Имя</span><span class="sxs-lookup"><span data-stu-id="26273-137">Name</span></span>      |<span data-ttu-id="26273-138">Описание</span><span class="sxs-lookup"><span data-stu-id="26273-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26273-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26273-139">Authorization</span></span> | <span data-ttu-id="26273-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26273-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26273-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26273-142">Request body</span></span>

<span data-ttu-id="26273-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26273-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26273-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="26273-144">Response</span></span>

<span data-ttu-id="26273-145">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [authenticationMethod](../resources/authenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26273-145">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26273-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="26273-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26273-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="26273-147">Request</span></span>

<span data-ttu-id="26273-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26273-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26273-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="26273-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="26273-150">C#</span><span class="sxs-lookup"><span data-stu-id="26273-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26273-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26273-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26273-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26273-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26273-153">Java</span><span class="sxs-lookup"><span data-stu-id="26273-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-methods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26273-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="26273-154">Response</span></span>

<span data-ttu-id="26273-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26273-155">The following is an example of the response.</span></span>

> <span data-ttu-id="26273-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26273-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
