---
title: Создание пользователя
description: С помощью этого API можно создать объект User.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 54c4ce8f21a2e62311d3931915f682f8f2366bfc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372561"
---
# <a name="create-user"></a><span data-ttu-id="035f5-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="035f5-103">Create User</span></span>

<span data-ttu-id="035f5-p101">Создание [пользователя](../resources/user.md). В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="035f5-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="035f5-108">Чтобы создать внешних пользователей, используйте [API приглашений](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="035f5-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="035f5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="035f5-109">Permissions</span></span>

<span data-ttu-id="035f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="035f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="035f5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="035f5-112">Permission type</span></span>      | <span data-ttu-id="035f5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="035f5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="035f5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="035f5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="035f5-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="035f5-115">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="035f5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="035f5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="035f5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="035f5-117">Not supported.</span></span>    |
|<span data-ttu-id="035f5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="035f5-118">Application</span></span> | <span data-ttu-id="035f5-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="035f5-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="035f5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="035f5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="035f5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="035f5-121">Request headers</span></span>

| <span data-ttu-id="035f5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="035f5-122">Header</span></span>       | <span data-ttu-id="035f5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="035f5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="035f5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="035f5-124">Authorization</span></span>  | <span data-ttu-id="035f5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="035f5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="035f5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="035f5-127">Content-Type</span></span>  | <span data-ttu-id="035f5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="035f5-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="035f5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="035f5-129">Request body</span></span>

<span data-ttu-id="035f5-130">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="035f5-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="035f5-131">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="035f5-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="035f5-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="035f5-132">Parameter</span></span> | <span data-ttu-id="035f5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="035f5-133">Type</span></span> | <span data-ttu-id="035f5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="035f5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="035f5-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="035f5-135">accountEnabled</span></span> |<span data-ttu-id="035f5-136">boolean</span><span class="sxs-lookup"><span data-stu-id="035f5-136">boolean</span></span> |<span data-ttu-id="035f5-137">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="035f5-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="035f5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="035f5-138">displayName</span></span> |<span data-ttu-id="035f5-139">string</span><span class="sxs-lookup"><span data-stu-id="035f5-139">string</span></span> |<span data-ttu-id="035f5-140">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="035f5-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="035f5-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="035f5-141">onPremisesImmutableId</span></span> |<span data-ttu-id="035f5-142">string</span><span class="sxs-lookup"><span data-stu-id="035f5-142">string</span></span> |<span data-ttu-id="035f5-143">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="035f5-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="035f5-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="035f5-144">mailNickname</span></span> |<span data-ttu-id="035f5-145">string</span><span class="sxs-lookup"><span data-stu-id="035f5-145">string</span></span> |<span data-ttu-id="035f5-146">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="035f5-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="035f5-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="035f5-147">passwordProfile</span></span>|[<span data-ttu-id="035f5-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="035f5-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="035f5-149">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="035f5-149">The password profile for the user.</span></span>|
|<span data-ttu-id="035f5-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="035f5-150">userPrincipalName</span></span> |<span data-ttu-id="035f5-151">string</span><span class="sxs-lookup"><span data-stu-id="035f5-151">string</span></span> |<span data-ttu-id="035f5-152">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="035f5-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="035f5-153">Так как ресурс **user** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в экземпляр user при его создании.</span><span class="sxs-lookup"><span data-stu-id="035f5-153">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="035f5-154">Федеративные пользователи, созданные с помощью этого API, по умолчанию должны выполнять вход каждые 12 часов.</span><span class="sxs-lookup"><span data-stu-id="035f5-154">Federated users created using this API will be forced to sign-in every 12 hours by default.</span></span>  <span data-ttu-id="035f5-155">Дополнительные сведения об изменении этого параметра см. в разделе [Исключения для сроков действия маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="035f5-155">For more information on how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="035f5-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="035f5-156">Response</span></span>

<span data-ttu-id="035f5-157">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="035f5-157">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="035f5-158">Пример</span><span class="sxs-lookup"><span data-stu-id="035f5-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="035f5-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="035f5-159">Request</span></span>

<span data-ttu-id="035f5-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="035f5-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="035f5-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="035f5-161">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="035f5-162">C#</span><span class="sxs-lookup"><span data-stu-id="035f5-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="035f5-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="035f5-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="035f5-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="035f5-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="035f5-165">Java</span><span class="sxs-lookup"><span data-stu-id="035f5-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="035f5-166">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="035f5-166">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="035f5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="035f5-167">Response</span></span>

<span data-ttu-id="035f5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="035f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
