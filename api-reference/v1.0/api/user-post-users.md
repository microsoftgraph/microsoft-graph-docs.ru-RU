---
title: Создание пользователя
description: Используйте этот интерфейс API для создания нового пользователя.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 218752a382da4ccb2bdbe240c8c57d03007b0169
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851655"
---
# <a name="create-user"></a><span data-ttu-id="f457f-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="f457f-103">Create User</span></span>

<span data-ttu-id="f457f-p101">С помощью этого API можно создать пользователя. В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="f457f-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="f457f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f457f-108">Permissions</span></span>
<span data-ttu-id="f457f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f457f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f457f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f457f-111">Permission type</span></span>      | <span data-ttu-id="f457f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f457f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f457f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f457f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f457f-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f457f-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f457f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f457f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f457f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f457f-116">Not supported.</span></span>    |
|<span data-ttu-id="f457f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f457f-117">Application</span></span> | <span data-ttu-id="f457f-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f457f-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f457f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f457f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="f457f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f457f-120">Request headers</span></span>
| <span data-ttu-id="f457f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f457f-121">Header</span></span>       | <span data-ttu-id="f457f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f457f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f457f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f457f-123">Authorization</span></span>  | <span data-ttu-id="f457f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f457f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f457f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f457f-126">Content-Type</span></span>  | <span data-ttu-id="f457f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f457f-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f457f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f457f-128">Request body</span></span>
<span data-ttu-id="f457f-129">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f457f-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="f457f-130">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="f457f-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="f457f-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f457f-131">Parameter</span></span> | <span data-ttu-id="f457f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f457f-132">Type</span></span> | <span data-ttu-id="f457f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f457f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f457f-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="f457f-134">accountEnabled</span></span> |<span data-ttu-id="f457f-135">boolean</span><span class="sxs-lookup"><span data-stu-id="f457f-135">boolean</span></span> |<span data-ttu-id="f457f-136">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="f457f-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="f457f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f457f-137">displayName</span></span> |<span data-ttu-id="f457f-138">строка</span><span class="sxs-lookup"><span data-stu-id="f457f-138">string</span></span> |<span data-ttu-id="f457f-139">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f457f-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="f457f-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="f457f-140">onPremisesImmutableId</span></span> |<span data-ttu-id="f457f-141">string</span><span class="sxs-lookup"><span data-stu-id="f457f-141">string</span></span> |<span data-ttu-id="f457f-142">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f457f-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="f457f-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f457f-143">mailNickname</span></span> |<span data-ttu-id="f457f-144">string</span><span class="sxs-lookup"><span data-stu-id="f457f-144">string</span></span> |<span data-ttu-id="f457f-145">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f457f-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="f457f-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="f457f-146">passwordProfile</span></span>|[<span data-ttu-id="f457f-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="f457f-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="f457f-148">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="f457f-148">The password profile for the user.</span></span>|
|<span data-ttu-id="f457f-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f457f-149">userPrincipalName</span></span> |<span data-ttu-id="f457f-150">string</span><span class="sxs-lookup"><span data-stu-id="f457f-150">string</span></span> |<span data-ttu-id="f457f-151">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f457f-151">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="f457f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f457f-152">Response</span></span>

<span data-ttu-id="f457f-153">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f457f-153">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f457f-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f457f-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f457f-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f457f-155">Request</span></span>
<span data-ttu-id="f457f-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f457f-156">Here is an example of the request.</span></span>
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
<span data-ttu-id="f457f-157">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f457f-157">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f457f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="f457f-158">Response</span></span>
<span data-ttu-id="f457f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f457f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
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
  "tocPath": ""
}-->
