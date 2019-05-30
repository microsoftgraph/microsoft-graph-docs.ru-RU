---
title: Создание пользователя
description: Создание пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 19388f645eeea78a4237a8085abdd17b3c819f08
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536983"
---
# <a name="create-user"></a><span data-ttu-id="eb484-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="eb484-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb484-104">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-104">Create a new user.</span></span>
<span data-ttu-id="eb484-105">В теле запроса указан пользователь, которого нужно создать.</span><span class="sxs-lookup"><span data-stu-id="eb484-105">The request body contains the user to create.</span></span> <span data-ttu-id="eb484-106">Вам нужно указать как минимум обязательные свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="eb484-107">При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="eb484-107">You can optionally specify any other writable properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb484-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb484-108">Permissions</span></span>

<span data-ttu-id="eb484-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb484-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb484-111">Permission type</span></span>      | <span data-ttu-id="eb484-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb484-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb484-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb484-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eb484-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb484-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb484-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb484-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb484-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb484-116">Not supported.</span></span>    |
|<span data-ttu-id="eb484-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb484-117">Application</span></span> | <span data-ttu-id="eb484-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb484-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb484-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb484-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="eb484-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb484-120">Request headers</span></span>
| <span data-ttu-id="eb484-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb484-121">Header</span></span>       | <span data-ttu-id="eb484-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eb484-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb484-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb484-123">Authorization</span></span>  | <span data-ttu-id="eb484-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb484-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb484-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb484-126">Content-Type</span></span>  | <span data-ttu-id="eb484-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb484-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb484-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb484-128">Request body</span></span>

<span data-ttu-id="eb484-129">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb484-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="eb484-130">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="eb484-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="eb484-131">Parameter</span></span> | <span data-ttu-id="eb484-132">Тип</span><span class="sxs-lookup"><span data-stu-id="eb484-132">Type</span></span> | <span data-ttu-id="eb484-133">Описание</span><span class="sxs-lookup"><span data-stu-id="eb484-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb484-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="eb484-134">accountEnabled</span></span> |<span data-ttu-id="eb484-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb484-135">Boolean</span></span> |<span data-ttu-id="eb484-136">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="eb484-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="eb484-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eb484-137">displayName</span></span> |<span data-ttu-id="eb484-138">string</span><span class="sxs-lookup"><span data-stu-id="eb484-138">string</span></span> |<span data-ttu-id="eb484-139">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="eb484-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="eb484-140">onPremisesImmutableId</span></span> |<span data-ttu-id="eb484-141">string</span><span class="sxs-lookup"><span data-stu-id="eb484-141">string</span></span> |<span data-ttu-id="eb484-142">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="eb484-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="eb484-143">mailNickname</span></span> |<span data-ttu-id="eb484-144">string</span><span class="sxs-lookup"><span data-stu-id="eb484-144">string</span></span> |<span data-ttu-id="eb484-145">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="eb484-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="eb484-146">passwordProfile</span></span>|[<span data-ttu-id="eb484-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="eb484-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="eb484-148">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb484-148">The password profile for the user.</span></span>|
|<span data-ttu-id="eb484-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eb484-149">userPrincipalName</span></span> |<span data-ttu-id="eb484-150">string</span><span class="sxs-lookup"><span data-stu-id="eb484-150">string</span></span> |<span data-ttu-id="eb484-151">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="eb484-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="eb484-152">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в экземпляр пользователя при его создании.</span><span class="sxs-lookup"><span data-stu-id="eb484-152">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="eb484-153">Федеративные пользователи, созданные с помощью этого API, будут вынуждены подписываться каждые 12 часов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eb484-153">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="eb484-154">Дополнительные сведения об изменении этого способа приведены в статье [исключения для времени существования маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="eb484-154">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="eb484-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb484-155">Response</span></span>

<span data-ttu-id="eb484-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb484-156">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb484-157">Пример</span><span class="sxs-lookup"><span data-stu-id="eb484-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb484-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb484-158">Request</span></span>
<span data-ttu-id="eb484-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb484-159">Here is an example of the request.</span></span>
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
<span data-ttu-id="eb484-160">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb484-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eb484-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb484-161">Response</span></span>
<span data-ttu-id="eb484-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb484-162">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="eb484-163">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eb484-163">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb484-164">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb484-164">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb484-165">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="eb484-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb484-166">C#</span><span class="sxs-lookup"><span data-stu-id="eb484-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb484-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb484-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="eb484-168">См. также</span><span class="sxs-lookup"><span data-stu-id="eb484-168">See also</span></span>

- [<span data-ttu-id="eb484-169">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="eb484-169">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eb484-170">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="eb484-170">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="eb484-171">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="eb484-171">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
