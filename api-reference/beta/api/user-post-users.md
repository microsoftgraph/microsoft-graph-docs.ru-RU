---
title: Создание пользователя
description: Создание пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6eb65544ed26e0b08802fbc84ce8dbcabf0a8ed1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362061"
---
# <a name="create-user"></a><span data-ttu-id="b8b26-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="b8b26-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8b26-104">Создайте нового [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b8b26-104">Create a new [user](../resources/user.md).</span></span>
<span data-ttu-id="b8b26-105">В теле запроса указан пользователь, которого нужно создать.</span><span class="sxs-lookup"><span data-stu-id="b8b26-105">The request body contains the user to create.</span></span> <span data-ttu-id="b8b26-106">Вам нужно указать как минимум обязательные свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8b26-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="b8b26-107">При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="b8b26-107">You can optionally specify any other writable properties.</span></span>

>[!NOTE]
><span data-ttu-id="b8b26-108">Для создания внешних пользователей используйте [API приглашения](invitation-post.md).</span><span class="sxs-lookup"><span data-stu-id="b8b26-108">To create external users, use the [invitation API](invitation-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8b26-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8b26-109">Permissions</span></span>

<span data-ttu-id="b8b26-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b26-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8b26-112">Permission type</span></span>      | <span data-ttu-id="b8b26-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8b26-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8b26-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8b26-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b8b26-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8b26-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8b26-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8b26-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8b26-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8b26-117">Not supported.</span></span>    |
|<span data-ttu-id="b8b26-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8b26-118">Application</span></span> | <span data-ttu-id="b8b26-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8b26-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8b26-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8b26-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="b8b26-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8b26-121">Request headers</span></span>
| <span data-ttu-id="b8b26-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8b26-122">Header</span></span>       | <span data-ttu-id="b8b26-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b8b26-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8b26-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8b26-124">Authorization</span></span>  | <span data-ttu-id="b8b26-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8b26-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8b26-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8b26-127">Content-Type</span></span>  | <span data-ttu-id="b8b26-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b8b26-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8b26-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8b26-129">Request body</span></span>

<span data-ttu-id="b8b26-130">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8b26-130">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="b8b26-131">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8b26-131">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="b8b26-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="b8b26-132">Parameter</span></span> | <span data-ttu-id="b8b26-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b8b26-133">Type</span></span> | <span data-ttu-id="b8b26-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b8b26-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8b26-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b8b26-135">accountEnabled</span></span> |<span data-ttu-id="b8b26-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b26-136">Boolean</span></span> |<span data-ttu-id="b8b26-137">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="b8b26-137">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="b8b26-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b8b26-138">displayName</span></span> |<span data-ttu-id="b8b26-139">строка</span><span class="sxs-lookup"><span data-stu-id="b8b26-139">string</span></span> |<span data-ttu-id="b8b26-140">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8b26-140">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="b8b26-141">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="b8b26-141">onPremisesImmutableId</span></span> |<span data-ttu-id="b8b26-142">string</span><span class="sxs-lookup"><span data-stu-id="b8b26-142">string</span></span> |<span data-ttu-id="b8b26-143">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8b26-143">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="b8b26-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b8b26-144">mailNickname</span></span> |<span data-ttu-id="b8b26-145">string</span><span class="sxs-lookup"><span data-stu-id="b8b26-145">string</span></span> |<span data-ttu-id="b8b26-146">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8b26-146">The mail alias for the user.</span></span>|
|<span data-ttu-id="b8b26-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="b8b26-147">passwordProfile</span></span>|[<span data-ttu-id="b8b26-148">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="b8b26-148">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="b8b26-149">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8b26-149">The password profile for the user.</span></span>|
|<span data-ttu-id="b8b26-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8b26-150">userPrincipalName</span></span> |<span data-ttu-id="b8b26-151">string</span><span class="sxs-lookup"><span data-stu-id="b8b26-151">string</span></span> |<span data-ttu-id="b8b26-152">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b8b26-152">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="b8b26-153">Так как ресурс **User** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в экземпляр пользователя при его создании.</span><span class="sxs-lookup"><span data-stu-id="b8b26-153">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

>[!NOTE]
><span data-ttu-id="b8b26-154">Федеративные пользователи, созданные с помощью этого API, будут вынуждены подписываться каждые 12 часов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b8b26-154">Federated users created using this API will be forced to sign in every 12 hours by default.</span></span> <span data-ttu-id="b8b26-155">Дополнительные сведения об изменении этого способа приведены в статье [исключения для времени существования маркеров](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span><span class="sxs-lookup"><span data-stu-id="b8b26-155">For more information about how to change this, see [Exceptions for token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions).</span></span>

## <a name="response"></a><span data-ttu-id="b8b26-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8b26-156">Response</span></span>

<span data-ttu-id="b8b26-157">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b8b26-157">If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b26-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b8b26-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8b26-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8b26-159">Request</span></span>
<span data-ttu-id="b8b26-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8b26-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8b26-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8b26-161">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8b26-162">C#</span><span class="sxs-lookup"><span data-stu-id="b8b26-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8b26-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8b26-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8b26-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b8b26-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8b26-165">Java</span><span class="sxs-lookup"><span data-stu-id="b8b26-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b8b26-166">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8b26-166">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b8b26-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8b26-167">Response</span></span>
<span data-ttu-id="b8b26-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8b26-168">Here is an example of the response.</span></span> 

[!NOTE]
<span data-ttu-id="b8b26-169">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8b26-169">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8b26-170">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8b26-170">All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b8b26-171">См. также</span><span class="sxs-lookup"><span data-stu-id="b8b26-171">See also</span></span>

- [<span data-ttu-id="b8b26-172">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b8b26-172">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b8b26-173">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="b8b26-173">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b8b26-174">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="b8b26-174">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
  ]
}
-->
