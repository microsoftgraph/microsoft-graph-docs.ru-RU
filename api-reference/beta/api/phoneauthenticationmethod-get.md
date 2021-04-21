---
title: Get phoneAuthenticationMethod
description: Извлечение одного объекта phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f968838fb5e492c548f154afd311c212a05334fc
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921653"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="b4be5-103">Get phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b4be5-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="b4be5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4be5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4be5-105">Извлечение одного [объекта phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b4be5-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="b4be5-106">Этот метод доступен только для стандартных пользователей Azure AD и B2B, но не для пользователей B2C.</span><span class="sxs-lookup"><span data-stu-id="b4be5-106">This method is available only for standard Azure AD and B2B users, but not B2C users.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4be5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4be5-107">Permissions</span></span>

<span data-ttu-id="b4be5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4be5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b4be5-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="b4be5-110">Permissions acting on self</span></span>

|<span data-ttu-id="b4be5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4be5-111">Permission type</span></span>      | <span data-ttu-id="b4be5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4be5-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b4be5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4be5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4be5-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4be5-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b4be5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4be5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4be5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4be5-116">Not supported.</span></span> |
| <span data-ttu-id="b4be5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4be5-117">Application</span></span>                            | <span data-ttu-id="b4be5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4be5-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b4be5-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="b4be5-119">Permissions acting on other users</span></span>

|<span data-ttu-id="b4be5-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4be5-120">Permission type</span></span>      | <span data-ttu-id="b4be5-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4be5-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b4be5-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4be5-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4be5-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4be5-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b4be5-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4be5-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4be5-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4be5-125">Not supported.</span></span> |
| <span data-ttu-id="b4be5-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4be5-126">Application</span></span>                            | <span data-ttu-id="b4be5-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4be5-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b4be5-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b4be5-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b4be5-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b4be5-129">Global admin</span></span>
* <span data-ttu-id="b4be5-130">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="b4be5-130">Global reader</span></span>
* <span data-ttu-id="b4be5-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b4be5-131">Privileged authentication admin</span></span>
* <span data-ttu-id="b4be5-132">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="b4be5-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="b4be5-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4be5-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="b4be5-134">Значение, `id` соответствующее извлечению phoneType, является одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="b4be5-134">The value of `id` corresponding to the phoneType to retrieve is one of the following:</span></span>
+ <span data-ttu-id="b4be5-135">`b6332ec1-7057-4abe-9331-3d72feddfe41` для получения `alternateMobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="b4be5-135">`b6332ec1-7057-4abe-9331-3d72feddfe41` to retrieve the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="b4be5-136">`e37fc753-ff3b-4958-9484-eaa9425c82bc` для получения `office` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="b4be5-136">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to retrieve the `office` **phoneType**.</span></span>
+ <span data-ttu-id="b4be5-137">`3179e48a-750b-4051-897c-87b9720928f7` для получения `mobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="b4be5-137">`3179e48a-750b-4051-897c-87b9720928f7` to retrieve the `mobile` **phoneType**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b4be5-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4be5-138">Optional query parameters</span></span>

<span data-ttu-id="b4be5-139">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4be5-139">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4be5-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4be5-140">Request headers</span></span>

| <span data-ttu-id="b4be5-141">Имя</span><span class="sxs-lookup"><span data-stu-id="b4be5-141">Name</span></span>      |<span data-ttu-id="b4be5-142">Описание</span><span class="sxs-lookup"><span data-stu-id="b4be5-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4be5-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4be5-143">Authorization</span></span> | <span data-ttu-id="b4be5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4be5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4be5-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4be5-146">Request body</span></span>

<span data-ttu-id="b4be5-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4be5-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4be5-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4be5-148">Response</span></span>

<span data-ttu-id="b4be5-149">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b4be5-149">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4be5-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4be5-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4be5-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4be5-151">Request</span></span>

<span data-ttu-id="b4be5-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4be5-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4be5-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4be5-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="b4be5-154">C#</span><span class="sxs-lookup"><span data-stu-id="b4be5-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4be5-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4be5-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4be5-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4be5-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4be5-157">Java</span><span class="sxs-lookup"><span data-stu-id="b4be5-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4be5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4be5-158">Response</span></span>

<span data-ttu-id="b4be5-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4be5-159">The following is an example of the response.</span></span>

> <span data-ttu-id="b4be5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4be5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
