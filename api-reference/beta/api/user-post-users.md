---
title: Создание пользователя
description: Создание пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62c57763c41c034b6c93a8e0e40780a9f0ccc69b
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914681"
---
# <a name="create-user"></a><span data-ttu-id="223df-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="223df-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="223df-104">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-104">Create a new user.</span></span>
<span data-ttu-id="223df-105">В теле запроса указан пользователь, которого нужно создать.</span><span class="sxs-lookup"><span data-stu-id="223df-105">The request body contains the user to create.</span></span> <span data-ttu-id="223df-106">Вам нужно указать как минимум обязательные свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="223df-107">При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="223df-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="223df-108">Внешние пользователи должны создаваться с помощью приглашения.</span><span class="sxs-lookup"><span data-stu-id="223df-108">External users must be created through an invitation.</span></span> <span data-ttu-id="223df-109">Если необходимо включить создание внешних пользователей, обратитесь к разделу [приглашение](../resources/invitation.md).</span><span class="sxs-lookup"><span data-stu-id="223df-109">If you need to enable the creation of external users, see [invitation](../resources/invitation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="223df-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="223df-110">Permissions</span></span>

<span data-ttu-id="223df-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="223df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="223df-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="223df-113">Permission type</span></span>      | <span data-ttu-id="223df-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="223df-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="223df-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="223df-115">Delegated (work or school account)</span></span> | <span data-ttu-id="223df-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="223df-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="223df-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="223df-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="223df-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="223df-118">Not supported.</span></span>    |
|<span data-ttu-id="223df-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="223df-119">Application</span></span> | <span data-ttu-id="223df-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="223df-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="223df-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="223df-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="223df-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="223df-122">Request headers</span></span>
| <span data-ttu-id="223df-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="223df-123">Header</span></span>       | <span data-ttu-id="223df-124">Значение</span><span class="sxs-lookup"><span data-stu-id="223df-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="223df-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="223df-125">Authorization</span></span>  | <span data-ttu-id="223df-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="223df-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="223df-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="223df-128">Content-Type</span></span>  | <span data-ttu-id="223df-129">application/json</span><span class="sxs-lookup"><span data-stu-id="223df-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="223df-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="223df-130">Request body</span></span>

<span data-ttu-id="223df-131">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="223df-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="223df-132">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="223df-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="223df-133">Parameter</span></span> | <span data-ttu-id="223df-134">Тип</span><span class="sxs-lookup"><span data-stu-id="223df-134">Type</span></span> | <span data-ttu-id="223df-135">Описание</span><span class="sxs-lookup"><span data-stu-id="223df-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="223df-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="223df-136">accountEnabled</span></span> |<span data-ttu-id="223df-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="223df-137">Boolean</span></span> |<span data-ttu-id="223df-138">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="223df-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="223df-139">displayName</span><span class="sxs-lookup"><span data-stu-id="223df-139">displayName</span></span> |<span data-ttu-id="223df-140">строка</span><span class="sxs-lookup"><span data-stu-id="223df-140">string</span></span> |<span data-ttu-id="223df-141">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="223df-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="223df-142">onPremisesImmutableId</span></span> |<span data-ttu-id="223df-143">string</span><span class="sxs-lookup"><span data-stu-id="223df-143">string</span></span> |<span data-ttu-id="223df-144">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="223df-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="223df-145">mailNickname</span></span> |<span data-ttu-id="223df-146">string</span><span class="sxs-lookup"><span data-stu-id="223df-146">string</span></span> |<span data-ttu-id="223df-147">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="223df-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="223df-148">passwordProfile</span></span>|[<span data-ttu-id="223df-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="223df-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="223df-150">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="223df-150">The password profile for the user.</span></span>|
|<span data-ttu-id="223df-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="223df-151">userPrincipalName</span></span> |<span data-ttu-id="223df-152">string</span><span class="sxs-lookup"><span data-stu-id="223df-152">string</span></span> |<span data-ttu-id="223df-153">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="223df-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="223df-154">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в экземпляр пользователя при его создании.</span><span class="sxs-lookup"><span data-stu-id="223df-154">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="223df-155">Федеративные пользователи, созданные с помощью этого API, будут вынуждены подписываться каждые 12 часов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="223df-155">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="223df-156">Дополнительные сведения об изменении этого способа приведены в статье [исключения для времени существования маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="223df-156">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="223df-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="223df-157">Response</span></span>

<span data-ttu-id="223df-158">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="223df-158">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="223df-159">Пример</span><span class="sxs-lookup"><span data-stu-id="223df-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="223df-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="223df-160">Request</span></span>
<span data-ttu-id="223df-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="223df-161">Here is an example of the request.</span></span>
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
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
<span data-ttu-id="223df-162">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="223df-162">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="223df-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="223df-163">Response</span></span>
<span data-ttu-id="223df-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="223df-164">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="223df-165">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="223df-165">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="223df-166">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="223df-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="223df-167">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="223df-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="223df-168">C#</span><span class="sxs-lookup"><span data-stu-id="223df-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="223df-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="223df-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="223df-170">См. также</span><span class="sxs-lookup"><span data-stu-id="223df-170">See also</span></span>

- [<span data-ttu-id="223df-171">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="223df-171">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="223df-172">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="223df-172">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="223df-173">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="223df-173">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
