---
title: Get passwordAuthenticationMethod
description: Извлечение свойств и связей объекта passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2112788ce5127326e0e82ef91c1068b5b56ec14a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515597"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="ef2b7-103">Get passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef2b7-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="ef2b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef2b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef2b7-105">Извлечение свойств и связей объекта [метода проверки подлинности паролей.](../resources/passwordauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ef2b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2b7-106">Permissions</span></span>

<span data-ttu-id="ef2b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef2b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ef2b7-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="ef2b7-109">Permissions acting on self</span></span>

|<span data-ttu-id="ef2b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2b7-110">Permission type</span></span>      | <span data-ttu-id="ef2b7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ef2b7-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef2b7-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef2b7-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ef2b7-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef2b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-115">Not supported.</span></span> |
| <span data-ttu-id="ef2b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef2b7-116">Application</span></span>                            | <span data-ttu-id="ef2b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ef2b7-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="ef2b7-118">Permissions acting on other users</span></span>

|<span data-ttu-id="ef2b7-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2b7-119">Permission type</span></span>      | <span data-ttu-id="ef2b7-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ef2b7-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef2b7-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2b7-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ef2b7-123">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef2b7-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-124">Not supported.</span></span> |
| <span data-ttu-id="ef2b7-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef2b7-125">Application</span></span>                            | <span data-ttu-id="ef2b7-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2b7-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ef2b7-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ef2b7-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ef2b7-128">Global admin</span></span>
* <span data-ttu-id="ef2b7-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ef2b7-129">Global reader</span></span>
* <span data-ttu-id="ef2b7-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ef2b7-130">Privileged authentication admin</span></span>
* <span data-ttu-id="ef2b7-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ef2b7-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef2b7-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef2b7-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef2b7-133">Optional query parameters</span></span>

<span data-ttu-id="ef2b7-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef2b7-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef2b7-135">Request headers</span></span>

| <span data-ttu-id="ef2b7-136">Имя</span><span class="sxs-lookup"><span data-stu-id="ef2b7-136">Name</span></span>      |<span data-ttu-id="ef2b7-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ef2b7-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef2b7-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef2b7-138">Authorization</span></span> | <span data-ttu-id="ef2b7-139">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ef2b7-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef2b7-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef2b7-140">Request body</span></span>

<span data-ttu-id="ef2b7-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef2b7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef2b7-142">Response</span></span>

<span data-ttu-id="ef2b7-143">В случае успешной работы этот метод возвращает код отклика и запрашиваемого `200 OK` [пароляAuthenticationMethod](../resources/passwordauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef2b7-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef2b7-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef2b7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef2b7-145">Request</span></span>

<span data-ttu-id="ef2b7-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef2b7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef2b7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="ef2b7-148">C#</span><span class="sxs-lookup"><span data-stu-id="ef2b7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef2b7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef2b7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef2b7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef2b7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef2b7-151">Java</span><span class="sxs-lookup"><span data-stu-id="ef2b7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ef2b7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef2b7-152">Response</span></span>

<span data-ttu-id="ef2b7-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-153">The following is an example of the response.</span></span>

> <span data-ttu-id="ef2b7-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
