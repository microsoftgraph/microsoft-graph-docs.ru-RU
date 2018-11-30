---
title: Создание пользователя
description: Используйте этот интерфейс API для создания нового пользователя.
ms.openlocfilehash: 17df752fb3767e82b72e46857e9ce6a2a8769db7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075903"
---
# <a name="create-user"></a><span data-ttu-id="7ca19-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="7ca19-103">Create user</span></span>

> <span data-ttu-id="7ca19-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ca19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ca19-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca19-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ca19-106">Используйте этот интерфейс API для создания нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-106">Use this API to create a new user.</span></span>
<span data-ttu-id="7ca19-107">Текст запроса содержит пользователю создать.</span><span class="sxs-lookup"><span data-stu-id="7ca19-107">The request body contains the user to create.</span></span> <span data-ttu-id="7ca19-108">Как минимум необходимо указать необходимые свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-108">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="7ca19-109">При необходимости можно указать любые другие свойства для записи.</span><span class="sxs-lookup"><span data-stu-id="7ca19-109">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ca19-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ca19-110">Permissions</span></span>
<span data-ttu-id="7ca19-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ca19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ca19-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ca19-113">Permission type</span></span>      | <span data-ttu-id="7ca19-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ca19-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ca19-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ca19-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7ca19-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ca19-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ca19-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ca19-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ca19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca19-118">Not supported.</span></span>    |
|<span data-ttu-id="7ca19-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ca19-119">Application</span></span> | <span data-ttu-id="7ca19-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ca19-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ca19-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ca19-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="7ca19-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ca19-122">Request headers</span></span>
| <span data-ttu-id="7ca19-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ca19-123">Header</span></span>       | <span data-ttu-id="7ca19-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7ca19-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ca19-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ca19-125">Authorization</span></span>  | <span data-ttu-id="7ca19-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ca19-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ca19-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ca19-128">Content-Type</span></span>  | <span data-ttu-id="7ca19-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7ca19-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ca19-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ca19-130">Request body</span></span>
<span data-ttu-id="7ca19-131">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ca19-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="7ca19-132">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="7ca19-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ca19-133">Parameter</span></span> | <span data-ttu-id="7ca19-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7ca19-134">Type</span></span> | <span data-ttu-id="7ca19-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7ca19-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ca19-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7ca19-136">accountEnabled</span></span> |<span data-ttu-id="7ca19-137">boolean</span><span class="sxs-lookup"><span data-stu-id="7ca19-137">boolean</span></span> |<span data-ttu-id="7ca19-138">Если учетная запись обеспечена — true, в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="7ca19-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="7ca19-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7ca19-139">displayName</span></span> |<span data-ttu-id="7ca19-140">строка</span><span class="sxs-lookup"><span data-stu-id="7ca19-140">string</span></span> |<span data-ttu-id="7ca19-141">Имя, которое следует отобразить в адресной книге для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="7ca19-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="7ca19-142">onPremisesImmutableId</span></span> |<span data-ttu-id="7ca19-143">string</span><span class="sxs-lookup"><span data-stu-id="7ca19-143">string</span></span> |<span data-ttu-id="7ca19-144">Необходимо указывать только при создании учетной записи пользователя, если вы используете федеративный домен для свойства userPrincipalName (UPN) этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="7ca19-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7ca19-145">mailNickname</span></span> |<span data-ttu-id="7ca19-146">string</span><span class="sxs-lookup"><span data-stu-id="7ca19-146">string</span></span> |<span data-ttu-id="7ca19-147">Почтовый псевдоним для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="7ca19-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="7ca19-148">passwordProfile</span></span>|[<span data-ttu-id="7ca19-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="7ca19-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="7ca19-150">Пароль для профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca19-150">The password profile for the user.</span></span>|
|<span data-ttu-id="7ca19-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ca19-151">userPrincipalName</span></span> |<span data-ttu-id="7ca19-152">string</span><span class="sxs-lookup"><span data-stu-id="7ca19-152">string</span></span> |<span data-ttu-id="7ca19-153">Имя участника-пользователя (polzovatel@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7ca19-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="7ca19-154">Поскольку **пользовательский** ресурс поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в экземпляр пользовательского при его создании.</span><span class="sxs-lookup"><span data-stu-id="7ca19-154">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="7ca19-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ca19-155">Response</span></span>

<span data-ttu-id="7ca19-156">В случае успеха этот метод возвратит код отклика `201 Created` и объект [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ca19-156">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ca19-157">Пример</span><span class="sxs-lookup"><span data-stu-id="7ca19-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ca19-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ca19-158">Request</span></span>
<span data-ttu-id="7ca19-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ca19-159">Here is an example of the request.</span></span>
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
  "userPrincipalName": "upn-value@tenant-value@onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="7ca19-160">В теле запроса предоставьте описание объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ca19-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7ca19-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ca19-161">Response</span></span>
<span data-ttu-id="7ca19-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ca19-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7ca19-165">См. также</span><span class="sxs-lookup"><span data-stu-id="7ca19-165">See also</span></span>

- [<span data-ttu-id="7ca19-166">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7ca19-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7ca19-167">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7ca19-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7ca19-168">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7ca19-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
