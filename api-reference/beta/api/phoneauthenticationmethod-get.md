---
title: Get phoneAuthenticationMethod
description: Извлечение одного объекта phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2a4936fcbcd39751e9ba8ed9c7b3df8579fc1f9c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447724"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="58563-103">Get phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="58563-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="58563-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58563-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58563-105">Извлечение одного [объекта phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="58563-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58563-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58563-106">Permissions</span></span>

<span data-ttu-id="58563-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="58563-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="58563-109">Permissions acting on self</span></span>

|<span data-ttu-id="58563-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58563-110">Permission type</span></span>      | <span data-ttu-id="58563-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58563-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="58563-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58563-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="58563-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58563-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="58563-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58563-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58563-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58563-115">Not supported.</span></span> |
| <span data-ttu-id="58563-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58563-116">Application</span></span>                            | <span data-ttu-id="58563-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58563-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="58563-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="58563-118">Permissions acting on other users</span></span>

|<span data-ttu-id="58563-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58563-119">Permission type</span></span>      | <span data-ttu-id="58563-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58563-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="58563-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58563-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="58563-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58563-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="58563-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58563-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58563-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58563-124">Not supported.</span></span> |
| <span data-ttu-id="58563-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="58563-125">Application</span></span>                            | <span data-ttu-id="58563-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58563-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="58563-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="58563-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="58563-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="58563-128">Global admin</span></span>
* <span data-ttu-id="58563-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="58563-129">Global reader</span></span>
* <span data-ttu-id="58563-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="58563-130">Privileged authentication admin</span></span>
* <span data-ttu-id="58563-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="58563-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="58563-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58563-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58563-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58563-133">Optional query parameters</span></span>

<span data-ttu-id="58563-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58563-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58563-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58563-135">Request headers</span></span>

| <span data-ttu-id="58563-136">Имя</span><span class="sxs-lookup"><span data-stu-id="58563-136">Name</span></span>      |<span data-ttu-id="58563-137">Описание</span><span class="sxs-lookup"><span data-stu-id="58563-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58563-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58563-138">Authorization</span></span> | <span data-ttu-id="58563-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58563-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58563-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58563-141">Request body</span></span>

<span data-ttu-id="58563-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58563-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58563-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="58563-143">Response</span></span>

<span data-ttu-id="58563-144">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="58563-144">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58563-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="58563-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58563-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="58563-146">Request</span></span>

<span data-ttu-id="58563-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58563-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58563-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="58563-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="58563-149">C#</span><span class="sxs-lookup"><span data-stu-id="58563-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58563-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58563-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58563-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58563-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58563-152">Java</span><span class="sxs-lookup"><span data-stu-id="58563-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58563-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="58563-153">Response</span></span>

<span data-ttu-id="58563-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58563-154">The following is an example of the response.</span></span>

> <span data-ttu-id="58563-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58563-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
