---
title: Get phoneAuthenticationMethod
description: Извлечение одного объекта phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4aea872d99deedb3fbf952954e2d6ff691994220
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957301"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="475fd-103">Get phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="475fd-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="475fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="475fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="475fd-105">Извлечение одного [объекта phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="475fd-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="475fd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="475fd-106">Permissions</span></span>

<span data-ttu-id="475fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="475fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="475fd-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="475fd-109">Permissions acting on self</span></span>

|<span data-ttu-id="475fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="475fd-110">Permission type</span></span>      | <span data-ttu-id="475fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="475fd-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="475fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="475fd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="475fd-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="475fd-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="475fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="475fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="475fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475fd-115">Not supported.</span></span> |
| <span data-ttu-id="475fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="475fd-116">Application</span></span>                            | <span data-ttu-id="475fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475fd-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="475fd-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="475fd-118">Permissions acting on other users</span></span>

|<span data-ttu-id="475fd-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="475fd-119">Permission type</span></span>      | <span data-ttu-id="475fd-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="475fd-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="475fd-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="475fd-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="475fd-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475fd-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="475fd-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="475fd-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="475fd-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475fd-124">Not supported.</span></span> |
| <span data-ttu-id="475fd-125">Application</span><span class="sxs-lookup"><span data-stu-id="475fd-125">Application</span></span>                            | <span data-ttu-id="475fd-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475fd-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="475fd-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="475fd-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="475fd-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="475fd-128">Global admin</span></span>
* <span data-ttu-id="475fd-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="475fd-129">Global reader</span></span>
* <span data-ttu-id="475fd-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="475fd-130">Privileged authentication admin</span></span>
* <span data-ttu-id="475fd-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="475fd-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="475fd-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="475fd-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="475fd-133">Значение, `id` соответствующее извлечению phoneType, является одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="475fd-133">The value of `id` corresponding to the phoneType to retrieve is one of the following:</span></span>
+ <span data-ttu-id="475fd-134">`b6332ec1-7057-4abe-9331-3d72feddfe41` для получения `alternateMobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="475fd-134">`b6332ec1-7057-4abe-9331-3d72feddfe41` to retrieve the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="475fd-135">`e37fc753-ff3b-4958-9484-eaa9425c82bc` для получения `office` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="475fd-135">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to retrieve the `office` **phoneType**.</span></span>
+ <span data-ttu-id="475fd-136">`3179e48a-750b-4051-897c-87b9720928f7` для получения `mobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="475fd-136">`3179e48a-750b-4051-897c-87b9720928f7` to retrieve the `mobile` **phoneType**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="475fd-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="475fd-137">Optional query parameters</span></span>

<span data-ttu-id="475fd-138">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="475fd-138">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="475fd-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="475fd-139">Request headers</span></span>

| <span data-ttu-id="475fd-140">Имя</span><span class="sxs-lookup"><span data-stu-id="475fd-140">Name</span></span>      |<span data-ttu-id="475fd-141">Описание</span><span class="sxs-lookup"><span data-stu-id="475fd-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="475fd-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="475fd-142">Authorization</span></span> | <span data-ttu-id="475fd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="475fd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="475fd-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="475fd-145">Request body</span></span>

<span data-ttu-id="475fd-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="475fd-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="475fd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="475fd-147">Response</span></span>

<span data-ttu-id="475fd-148">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="475fd-148">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="475fd-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="475fd-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="475fd-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="475fd-150">Request</span></span>

<span data-ttu-id="475fd-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="475fd-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="475fd-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="475fd-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="475fd-153">C#</span><span class="sxs-lookup"><span data-stu-id="475fd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="475fd-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="475fd-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="475fd-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="475fd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="475fd-156">Java</span><span class="sxs-lookup"><span data-stu-id="475fd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="475fd-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="475fd-157">Response</span></span>

<span data-ttu-id="475fd-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="475fd-158">The following is an example of the response.</span></span>

> <span data-ttu-id="475fd-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="475fd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
