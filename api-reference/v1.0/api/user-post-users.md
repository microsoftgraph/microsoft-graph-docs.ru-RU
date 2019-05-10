---
title: Создание пользователя
description: С помощью этого API можно создать объект User.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d9c247c3d9befef7fb6f342ce063620e11a4d3a6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600829"
---
# <a name="create-user"></a><span data-ttu-id="7134e-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="7134e-103">Create User</span></span>

<span data-ttu-id="7134e-p101">С помощью этого API можно создать пользователя. В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="7134e-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="7134e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7134e-108">Permissions</span></span>
<span data-ttu-id="7134e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7134e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7134e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7134e-111">Permission type</span></span>      | <span data-ttu-id="7134e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7134e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7134e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7134e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7134e-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7134e-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7134e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7134e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7134e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7134e-116">Not supported.</span></span>    |
|<span data-ttu-id="7134e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7134e-117">Application</span></span> | <span data-ttu-id="7134e-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7134e-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7134e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7134e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="7134e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7134e-120">Request headers</span></span>
| <span data-ttu-id="7134e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7134e-121">Header</span></span>       | <span data-ttu-id="7134e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7134e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7134e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7134e-123">Authorization</span></span>  | <span data-ttu-id="7134e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7134e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7134e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7134e-126">Content-Type</span></span>  | <span data-ttu-id="7134e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7134e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7134e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7134e-128">Request body</span></span>
<span data-ttu-id="7134e-129">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7134e-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="7134e-130">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="7134e-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="7134e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="7134e-131">Parameter</span></span> | <span data-ttu-id="7134e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7134e-132">Type</span></span> | <span data-ttu-id="7134e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7134e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7134e-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7134e-134">accountEnabled</span></span> |<span data-ttu-id="7134e-135">boolean</span><span class="sxs-lookup"><span data-stu-id="7134e-135">boolean</span></span> |<span data-ttu-id="7134e-136">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="7134e-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="7134e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7134e-137">displayName</span></span> |<span data-ttu-id="7134e-138">string</span><span class="sxs-lookup"><span data-stu-id="7134e-138">string</span></span> |<span data-ttu-id="7134e-139">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7134e-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="7134e-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="7134e-140">onPremisesImmutableId</span></span> |<span data-ttu-id="7134e-141">string</span><span class="sxs-lookup"><span data-stu-id="7134e-141">string</span></span> |<span data-ttu-id="7134e-142">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7134e-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="7134e-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7134e-143">mailNickname</span></span> |<span data-ttu-id="7134e-144">string</span><span class="sxs-lookup"><span data-stu-id="7134e-144">string</span></span> |<span data-ttu-id="7134e-145">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7134e-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="7134e-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="7134e-146">passwordProfile</span></span>|[<span data-ttu-id="7134e-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="7134e-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="7134e-148">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="7134e-148">The password profile for the user.</span></span>|
|<span data-ttu-id="7134e-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7134e-149">userPrincipalName</span></span> |<span data-ttu-id="7134e-150">string</span><span class="sxs-lookup"><span data-stu-id="7134e-150">string</span></span> |<span data-ttu-id="7134e-151">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7134e-151">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="7134e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7134e-152">Response</span></span>

<span data-ttu-id="7134e-153">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7134e-153">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7134e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="7134e-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7134e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="7134e-155">Request</span></span>
<span data-ttu-id="7134e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7134e-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="7134e-157">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7134e-157">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7134e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7134e-158">Response</span></span>
<span data-ttu-id="7134e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7134e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7134e-162">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7134e-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7134e-163">C#</span><span class="sxs-lookup"><span data-stu-id="7134e-163">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7134e-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7134e-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
