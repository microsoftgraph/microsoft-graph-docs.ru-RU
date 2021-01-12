---
title: Список passwordMethods
description: Получить список объектов passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9db73d5f5f01a315a5347fbe0627df991937513f
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796544"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="f467b-103">Список passwordMethods</span><span class="sxs-lookup"><span data-stu-id="f467b-103">List passwordMethods</span></span>

<span data-ttu-id="f467b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f467b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f467b-105">Получить список объектов метода [проверки подлинности](../resources/passwordauthenticationmethod.md) паролем.</span><span class="sxs-lookup"><span data-stu-id="f467b-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="f467b-106">При этом возвращается ровно один объект, так как пользователь может иметь только один пароль.</span><span class="sxs-lookup"><span data-stu-id="f467b-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="f467b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f467b-107">Permissions</span></span>

<span data-ttu-id="f467b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f467b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="f467b-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="f467b-110">Permissions acting on self</span></span>

|<span data-ttu-id="f467b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f467b-111">Permission type</span></span>      | <span data-ttu-id="f467b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f467b-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f467b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f467b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f467b-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f467b-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="f467b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f467b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f467b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f467b-116">Not supported.</span></span> |
| <span data-ttu-id="f467b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f467b-117">Application</span></span>                            | <span data-ttu-id="f467b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f467b-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="f467b-119">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="f467b-119">Permissions acting on other users</span></span>

|<span data-ttu-id="f467b-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f467b-120">Permission type</span></span>      | <span data-ttu-id="f467b-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f467b-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="f467b-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f467b-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="f467b-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f467b-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f467b-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f467b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f467b-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f467b-125">Not supported.</span></span> |
| <span data-ttu-id="f467b-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="f467b-126">Application</span></span>                            | <span data-ttu-id="f467b-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f467b-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f467b-128">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f467b-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="f467b-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f467b-129">Global admin</span></span>
* <span data-ttu-id="f467b-130">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="f467b-130">Global reader</span></span>
* <span data-ttu-id="f467b-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f467b-131">Privileged authentication admin</span></span>
* <span data-ttu-id="f467b-132">Администратор проверки подлинности (видит только маскирование номеров телефонов)</span><span class="sxs-lookup"><span data-stu-id="f467b-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="f467b-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f467b-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id | userPrincipalName}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f467b-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f467b-134">Optional query parameters</span></span>

<span data-ttu-id="f467b-135">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f467b-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f467b-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f467b-136">Request headers</span></span>

| <span data-ttu-id="f467b-137">Имя</span><span class="sxs-lookup"><span data-stu-id="f467b-137">Name</span></span>      |<span data-ttu-id="f467b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f467b-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f467b-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f467b-139">Authorization</span></span> | <span data-ttu-id="f467b-140">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f467b-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f467b-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f467b-141">Request body</span></span>

<span data-ttu-id="f467b-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f467b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f467b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f467b-143">Response</span></span>

<span data-ttu-id="f467b-144">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f467b-144">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f467b-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="f467b-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f467b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f467b-146">Request</span></span>

<span data-ttu-id="f467b-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f467b-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f467b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f467b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="f467b-149">C#</span><span class="sxs-lookup"><span data-stu-id="f467b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f467b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f467b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f467b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f467b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f467b-152">Java</span><span class="sxs-lookup"><span data-stu-id="f467b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordmethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f467b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f467b-153">Response</span></span>

<span data-ttu-id="f467b-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f467b-154">The following is an example of the response.</span></span>

> <span data-ttu-id="f467b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f467b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
