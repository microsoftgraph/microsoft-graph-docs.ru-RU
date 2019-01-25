---
title: Создание пользователя
description: Используйте этот интерфейс API для создания нового пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9d1e98ffa4be67141d1e5ae679f9f51a71ef92fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529336"
---
# <a name="create-user"></a><span data-ttu-id="2c0cc-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="2c0cc-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c0cc-p101">С помощью этого API можно создать пользователя. В теле запроса указан пользователь, которого нужно создать. Вам нужно указать как минимум обязательные свойства для пользователя. При необходимости вы можете указать другие записываемые свойства.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-p101">Use this API to create a new user. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c0cc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c0cc-108">Permissions</span></span>
<span data-ttu-id="2c0cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c0cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c0cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c0cc-111">Permission type</span></span>      | <span data-ttu-id="2c0cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c0cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c0cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c0cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c0cc-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c0cc-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c0cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c0cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c0cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-116">Not supported.</span></span>    |
|<span data-ttu-id="2c0cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c0cc-117">Application</span></span> | <span data-ttu-id="2c0cc-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0cc-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c0cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c0cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="2c0cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c0cc-120">Request headers</span></span>
| <span data-ttu-id="2c0cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c0cc-121">Header</span></span>       | <span data-ttu-id="2c0cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2c0cc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c0cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c0cc-123">Authorization</span></span>  | <span data-ttu-id="2c0cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c0cc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c0cc-126">Content-Type</span></span>  | <span data-ttu-id="2c0cc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2c0cc-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c0cc-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c0cc-128">Request body</span></span>
<span data-ttu-id="2c0cc-129">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="2c0cc-130">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="2c0cc-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c0cc-131">Parameter</span></span> | <span data-ttu-id="2c0cc-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2c0cc-132">Type</span></span> | <span data-ttu-id="2c0cc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2c0cc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c0cc-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="2c0cc-134">accountEnabled</span></span> |<span data-ttu-id="2c0cc-135">boolean</span><span class="sxs-lookup"><span data-stu-id="2c0cc-135">boolean</span></span> |<span data-ttu-id="2c0cc-136">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="2c0cc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2c0cc-137">displayName</span></span> |<span data-ttu-id="2c0cc-138">строка</span><span class="sxs-lookup"><span data-stu-id="2c0cc-138">string</span></span> |<span data-ttu-id="2c0cc-139">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="2c0cc-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="2c0cc-140">onPremisesImmutableId</span></span> |<span data-ttu-id="2c0cc-141">string</span><span class="sxs-lookup"><span data-stu-id="2c0cc-141">string</span></span> |<span data-ttu-id="2c0cc-142">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="2c0cc-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2c0cc-143">mailNickname</span></span> |<span data-ttu-id="2c0cc-144">string</span><span class="sxs-lookup"><span data-stu-id="2c0cc-144">string</span></span> |<span data-ttu-id="2c0cc-145">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="2c0cc-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="2c0cc-146">passwordProfile</span></span>|[<span data-ttu-id="2c0cc-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="2c0cc-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="2c0cc-148">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-148">The password profile for the user.</span></span>|
|<span data-ttu-id="2c0cc-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2c0cc-149">userPrincipalName</span></span> |<span data-ttu-id="2c0cc-150">string</span><span class="sxs-lookup"><span data-stu-id="2c0cc-150">string</span></span> |<span data-ttu-id="2c0cc-151">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2c0cc-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="2c0cc-152">Поскольку **пользовательский** ресурс поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в экземпляр пользовательского при его создании.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="2c0cc-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c0cc-153">Response</span></span>

<span data-ttu-id="2c0cc-154">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c0cc-155">Пример</span><span class="sxs-lookup"><span data-stu-id="2c0cc-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c0cc-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c0cc-156">Request</span></span>
<span data-ttu-id="2c0cc-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-157">Here is an example of the request.</span></span>
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
<span data-ttu-id="2c0cc-158">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2c0cc-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c0cc-159">Response</span></span>
<span data-ttu-id="2c0cc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2c0cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
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

## <a name="see-also"></a><span data-ttu-id="2c0cc-163">См. также</span><span class="sxs-lookup"><span data-stu-id="2c0cc-163">See also</span></span>

- [<span data-ttu-id="2c0cc-164">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="2c0cc-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2c0cc-165">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2c0cc-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2c0cc-166">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2c0cc-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
