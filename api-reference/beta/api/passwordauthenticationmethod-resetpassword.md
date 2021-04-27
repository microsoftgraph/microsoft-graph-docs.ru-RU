---
title: 'passwordAuthenticationMethod: resetPassword'
description: Сброс пароля пользователя
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 392629ed4cc686855b1ec31aba09f1b70a62c5a9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049172"
---
# <a name="passwordauthenticationmethod-resetpassword"></a><span data-ttu-id="33858-103">passwordAuthenticationMethod: resetPassword</span><span class="sxs-lookup"><span data-stu-id="33858-103">passwordAuthenticationMethod: resetPassword</span></span>

<span data-ttu-id="33858-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33858-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33858-105">Инициировать сброс пароля, связанного с объектом метода проверки [подлинности](../resources/passwordauthenticationmethod.md) паролей.</span><span class="sxs-lookup"><span data-stu-id="33858-105">Initiate a reset for the password associated with a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> <span data-ttu-id="33858-106">Это может быть сделано только администратором с соответствующими разрешениями и не может выполняться на собственной учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="33858-106">This can only be done by an administrator with appropriate permissions and cannot be performed on a user's own account.</span></span>

<span data-ttu-id="33858-107">Этот поток записывает новый пароль Azure Active Directory и толкает его на локальное Active Directory, если настроен с помощью записи пароля.</span><span class="sxs-lookup"><span data-stu-id="33858-107">This flow writes the new password to Azure Active Directory and pushes it to on-premises Active Directory if configured using password writeback.</span></span> <span data-ttu-id="33858-108">Администратор может либо предоставить новый пароль, либо создать его в системе.</span><span class="sxs-lookup"><span data-stu-id="33858-108">The admin can either provide a new password or have the system generate one.</span></span> <span data-ttu-id="33858-109">Пользователю предложено изменить пароль при следующем входе.</span><span class="sxs-lookup"><span data-stu-id="33858-109">The user is prompted to change their password on their next sign in.</span></span>

<span data-ttu-id="33858-110">Этот сброс является длительной операцией и возвращает ссылку в загонке, где вызываемая может периодически проверять состояние `Location` сброса.</span><span class="sxs-lookup"><span data-stu-id="33858-110">This reset is a long-running operation and will return a link in the `Location` header where the caller can periodically check for the status of the reset.</span></span>

## <a name="permissions"></a><span data-ttu-id="33858-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33858-111">Permissions</span></span>

<span data-ttu-id="33858-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33858-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33858-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33858-114">Permission type</span></span>                        | <span data-ttu-id="33858-115">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="33858-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="33858-116">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="33858-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="33858-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33858-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="33858-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33858-118">Not supported.</span></span> | <span data-ttu-id="33858-119">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33858-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="33858-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33858-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33858-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33858-121">Not supported.</span></span> | <span data-ttu-id="33858-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33858-122">Not supported.</span></span> |
| <span data-ttu-id="33858-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33858-123">Application</span></span>                            | <span data-ttu-id="33858-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33858-124">Not supported.</span></span> | <span data-ttu-id="33858-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33858-125">Not supported.</span></span> |

<span data-ttu-id="33858-126">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="33858-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="33858-127">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="33858-127">Global admin</span></span>
* <span data-ttu-id="33858-128">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="33858-128">Privileged authentication admin</span></span>
* <span data-ttu-id="33858-129">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="33858-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="33858-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33858-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a><span data-ttu-id="33858-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33858-131">Request headers</span></span>

| <span data-ttu-id="33858-132">Имя</span><span class="sxs-lookup"><span data-stu-id="33858-132">Name</span></span>          | <span data-ttu-id="33858-133">Описание</span><span class="sxs-lookup"><span data-stu-id="33858-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="33858-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33858-134">Authorization</span></span> | <span data-ttu-id="33858-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33858-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33858-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33858-137">Content-type</span></span>  | <span data-ttu-id="33858-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33858-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33858-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33858-140">Request body</span></span>

<span data-ttu-id="33858-141">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="33858-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33858-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="33858-142">Parameter</span></span>    | <span data-ttu-id="33858-143">Тип</span><span class="sxs-lookup"><span data-stu-id="33858-143">Type</span></span>        | <span data-ttu-id="33858-144">Описание</span><span class="sxs-lookup"><span data-stu-id="33858-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33858-145">newPassword</span><span class="sxs-lookup"><span data-stu-id="33858-145">newPassword</span></span>|<span data-ttu-id="33858-146">String</span><span class="sxs-lookup"><span data-stu-id="33858-146">String</span></span>|<span data-ttu-id="33858-147">Новый пароль, вписаный администратором. Требуется для клиентов с гибридными сценариями паролей.</span><span class="sxs-lookup"><span data-stu-id="33858-147">The new password entered by the admin. Required for tenants with hybrid password scenarios.</span></span> <span data-ttu-id="33858-148">Если не будет пропущен пароль только для облака, система возвращает созданный системой пароль.</span><span class="sxs-lookup"><span data-stu-id="33858-148">If omitted for a cloud-only password, the system returns a system-generated password.</span></span> <span data-ttu-id="33858-149">Это строка единого кода без другого кодирования.</span><span class="sxs-lookup"><span data-stu-id="33858-149">This is a unicode string with no other encoding.</span></span> <span data-ttu-id="33858-150">Он проверяется в отношении запрещенной системы паролей клиента перед принятием и должен соответствовать требованиям облачного и/или локального пароля клиента.</span><span class="sxs-lookup"><span data-stu-id="33858-150">It is validated against the tenant's banned password system before acceptance, and must adhere to the tenant's cloud and/or on-premises password requirements.</span></span>|

## <a name="response"></a><span data-ttu-id="33858-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="33858-151">Response</span></span>

<span data-ttu-id="33858-152">В случае успешной работы этот метод возвращает код `202 ACCEPTED` ответа и URL-адрес в `Location` загонах.</span><span class="sxs-lookup"><span data-stu-id="33858-152">If successful, this method returns a `202 ACCEPTED` response code and a URL in the `Location` header.</span></span>

<span data-ttu-id="33858-153">Если вызываемый не представил пароль, созданный Корпорацией Майкрософт пароль предоставляется в объекте JSON в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="33858-153">If the caller did not submit a password, a Microsoft-generated password is provided in a JSON object in the response body.</span></span>

### <a name="response-headers"></a><span data-ttu-id="33858-154">Заголовки откликов</span><span class="sxs-lookup"><span data-stu-id="33858-154">Response headers</span></span>

| <span data-ttu-id="33858-155">Имя</span><span class="sxs-lookup"><span data-stu-id="33858-155">Name</span></span>        | <span data-ttu-id="33858-156">Описание</span><span class="sxs-lookup"><span data-stu-id="33858-156">Description</span></span>     |
|:------------|:----------------|
|<span data-ttu-id="33858-157">Расположение</span><span class="sxs-lookup"><span data-stu-id="33858-157">Location</span></span>     | <span data-ttu-id="33858-158">URL-адрес для вызова, чтобы проверить состояние операции.</span><span class="sxs-lookup"><span data-stu-id="33858-158">URL to call to check the status of the operation.</span></span>|
|<span data-ttu-id="33858-159">Retry-after</span><span class="sxs-lookup"><span data-stu-id="33858-159">Retry-after</span></span>  | <span data-ttu-id="33858-160">Длительность в секундах.</span><span class="sxs-lookup"><span data-stu-id="33858-160">Duration in seconds.</span></span>|

## <a name="examples"></a><span data-ttu-id="33858-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="33858-161">Examples</span></span>

### <a name="example-1-user-submitted-password"></a><span data-ttu-id="33858-162">Пример 1. Пароль, отправленный пользователем</span><span class="sxs-lookup"><span data-stu-id="33858-162">Example 1: User-submitted password</span></span>

<span data-ttu-id="33858-163">В следующем примере показано, как вызвать этот API при отправке пароля вызываемой.</span><span class="sxs-lookup"><span data-stu-id="33858-163">The following example shows how to call this API when the caller submits a password.</span></span>

#### <a name="request"></a><span data-ttu-id="33858-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="33858-164">Request</span></span>

<span data-ttu-id="33858-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33858-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33858-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="33858-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
Content-type: application/json

{
  "newPassword": "newPassword-value",
}
```
# <a name="c"></a>[<span data-ttu-id="33858-167">C#</span><span class="sxs-lookup"><span data-stu-id="33858-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33858-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33858-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33858-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33858-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33858-170">Java</span><span class="sxs-lookup"><span data-stu-id="33858-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-adminprovided-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33858-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="33858-171">Response</span></span>

<span data-ttu-id="33858-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="33858-172">The following is an example of the response.</span></span>

> <span data-ttu-id="33858-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33858-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 ACCEPTED
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/operations/{id}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-system-generated-password"></a><span data-ttu-id="33858-174">Пример 2. Созданный системой пароль</span><span class="sxs-lookup"><span data-stu-id="33858-174">Example 2: System-generated password</span></span>

<span data-ttu-id="33858-175">В следующем примере показано, как вызывать этот API, если вызываемая не представляет пароль.</span><span class="sxs-lookup"><span data-stu-id="33858-175">The following example shows how to call this API when the caller does not submit a password.</span></span>

#### <a name="request"></a><span data-ttu-id="33858-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="33858-176">Request</span></span>

<span data-ttu-id="33858-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33858-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33858-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="33858-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```
# <a name="c"></a>[<span data-ttu-id="33858-179">C#</span><span class="sxs-lookup"><span data-stu-id="33858-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33858-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33858-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33858-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33858-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33858-182">Java</span><span class="sxs-lookup"><span data-stu-id="33858-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-systemgenerated-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33858-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="33858-183">Response</span></span>

<span data-ttu-id="33858-184">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="33858-184">The following is an example of the response.</span></span>

> <span data-ttu-id="33858-185">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33858-185">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/{id | userPrincipalName}/authentication/operations/{id}
Content-type: application/json

{
  "password": "new system generated password"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
