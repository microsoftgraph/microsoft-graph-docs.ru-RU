---
title: Создание пользователя
description: Используйте этот API, чтобы создать нового пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2bd39aa9251fabeeb564eb9db1e782804f533543
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334618"
---
# <a name="create-user"></a><span data-ttu-id="6a07c-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="6a07c-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a07c-104">Используйте этот API, чтобы создать нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-104">Use this API to create a new user.</span></span>
<span data-ttu-id="6a07c-105">В теле запроса указан пользователь, которого нужно создать.</span><span class="sxs-lookup"><span data-stu-id="6a07c-105">The request body contains the user to create.</span></span> <span data-ttu-id="6a07c-106">Вам нужно указать как минимум обязательные свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="6a07c-107">При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="6a07c-107">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a07c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a07c-108">Permissions</span></span>
<span data-ttu-id="6a07c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a07c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a07c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a07c-111">Permission type</span></span>      | <span data-ttu-id="6a07c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a07c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a07c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a07c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6a07c-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a07c-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a07c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a07c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a07c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a07c-116">Not supported.</span></span>    |
|<span data-ttu-id="6a07c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a07c-117">Application</span></span> | <span data-ttu-id="6a07c-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a07c-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a07c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a07c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="6a07c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a07c-120">Request headers</span></span>
| <span data-ttu-id="6a07c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a07c-121">Header</span></span>       | <span data-ttu-id="6a07c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6a07c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a07c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a07c-123">Authorization</span></span>  | <span data-ttu-id="6a07c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a07c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6a07c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a07c-126">Content-Type</span></span>  | <span data-ttu-id="6a07c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6a07c-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a07c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a07c-128">Request body</span></span>
<span data-ttu-id="6a07c-129">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a07c-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="6a07c-130">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="6a07c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="6a07c-131">Parameter</span></span> | <span data-ttu-id="6a07c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6a07c-132">Type</span></span> | <span data-ttu-id="6a07c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6a07c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a07c-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="6a07c-134">accountEnabled</span></span> |<span data-ttu-id="6a07c-135">boolean</span><span class="sxs-lookup"><span data-stu-id="6a07c-135">boolean</span></span> |<span data-ttu-id="6a07c-136">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="6a07c-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="6a07c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6a07c-137">displayName</span></span> |<span data-ttu-id="6a07c-138">строка</span><span class="sxs-lookup"><span data-stu-id="6a07c-138">string</span></span> |<span data-ttu-id="6a07c-139">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="6a07c-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="6a07c-140">onPremisesImmutableId</span></span> |<span data-ttu-id="6a07c-141">string</span><span class="sxs-lookup"><span data-stu-id="6a07c-141">string</span></span> |<span data-ttu-id="6a07c-142">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="6a07c-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6a07c-143">mailNickname</span></span> |<span data-ttu-id="6a07c-144">string</span><span class="sxs-lookup"><span data-stu-id="6a07c-144">string</span></span> |<span data-ttu-id="6a07c-145">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="6a07c-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="6a07c-146">passwordProfile</span></span>|[<span data-ttu-id="6a07c-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="6a07c-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="6a07c-148">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a07c-148">The password profile for the user.</span></span>|
|<span data-ttu-id="6a07c-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a07c-149">userPrincipalName</span></span> |<span data-ttu-id="6a07c-150">string</span><span class="sxs-lookup"><span data-stu-id="6a07c-150">string</span></span> |<span data-ttu-id="6a07c-151">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6a07c-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="6a07c-152">Так как **Пользовательский** ресурс поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавить настраиваемые свойства с собственными данными в экземпляр пользователя при его создании.</span><span class="sxs-lookup"><span data-stu-id="6a07c-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="6a07c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a07c-153">Response</span></span>

<span data-ttu-id="6a07c-154">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6a07c-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a07c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="6a07c-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a07c-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a07c-156">Request</span></span>
<span data-ttu-id="6a07c-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a07c-157">Here is an example of the request.</span></span>
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
<span data-ttu-id="6a07c-158">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a07c-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6a07c-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a07c-159">Response</span></span>
<span data-ttu-id="6a07c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6a07c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6a07c-163">См. также</span><span class="sxs-lookup"><span data-stu-id="6a07c-163">See also</span></span>

- [<span data-ttu-id="6a07c-164">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="6a07c-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6a07c-165">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6a07c-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6a07c-166">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6a07c-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
