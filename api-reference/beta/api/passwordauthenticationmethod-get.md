---
title: Get passwordAuthenticationMethod
description: Извлечение свойств и связей объекта passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a34939a59ca265fb7c50b82cf662095052763950
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761439"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="6d2c5-103">Get passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6d2c5-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="6d2c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d2c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d2c5-105">Извлечение свойств и связей объекта [метода проверки подлинности паролей.](../resources/passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6d2c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d2c5-106">Permissions</span></span>

<span data-ttu-id="6d2c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d2c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="6d2c5-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="6d2c5-109">Permissions acting on self</span></span>

|<span data-ttu-id="6d2c5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d2c5-110">Permission type</span></span>      | <span data-ttu-id="6d2c5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="6d2c5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d2c5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d2c5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="6d2c5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d2c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-115">Not supported.</span></span> |
| <span data-ttu-id="6d2c5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d2c5-116">Application</span></span>                            | <span data-ttu-id="6d2c5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="6d2c5-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="6d2c5-118">Permissions acting on other users</span></span>

|<span data-ttu-id="6d2c5-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d2c5-119">Permission type</span></span>      | <span data-ttu-id="6d2c5-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="6d2c5-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d2c5-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2c5-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="6d2c5-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d2c5-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-124">Not supported.</span></span> |
| <span data-ttu-id="6d2c5-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d2c5-125">Application</span></span>                            | <span data-ttu-id="6d2c5-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2c5-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="6d2c5-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="6d2c5-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6d2c5-128">Global admin</span></span>
* <span data-ttu-id="6d2c5-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="6d2c5-129">Global reader</span></span>
* <span data-ttu-id="6d2c5-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6d2c5-130">Privileged authentication admin</span></span>
* <span data-ttu-id="6d2c5-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="6d2c5-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="6d2c5-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d2c5-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d2c5-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d2c5-133">Optional query parameters</span></span>

<span data-ttu-id="6d2c5-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d2c5-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d2c5-135">Request headers</span></span>

| <span data-ttu-id="6d2c5-136">Имя</span><span class="sxs-lookup"><span data-stu-id="6d2c5-136">Name</span></span>      |<span data-ttu-id="6d2c5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="6d2c5-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d2c5-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d2c5-138">Authorization</span></span> | <span data-ttu-id="6d2c5-139">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6d2c5-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d2c5-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d2c5-140">Request body</span></span>

<span data-ttu-id="6d2c5-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d2c5-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d2c5-142">Response</span></span>

<span data-ttu-id="6d2c5-143">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [пароляAuthenticationMethod](../resources/passwordauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d2c5-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d2c5-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d2c5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d2c5-145">Request</span></span>

<span data-ttu-id="6d2c5-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d2c5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d2c5-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="6d2c5-148">C#</span><span class="sxs-lookup"><span data-stu-id="6d2c5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d2c5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d2c5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d2c5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d2c5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d2c5-151">Java</span><span class="sxs-lookup"><span data-stu-id="6d2c5-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d2c5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d2c5-152">Response</span></span>

<span data-ttu-id="6d2c5-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-153">The following is an example of the response.</span></span>

> <span data-ttu-id="6d2c5-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d2c5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
