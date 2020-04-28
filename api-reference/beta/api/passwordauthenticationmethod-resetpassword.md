---
title: 'Пассвордаусентикатионмесод: Ресетпассворд'
description: Сброс пароля пользователя
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9dabb63709b42f7eaa9c3791e9e91300f5063469
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806005"
---
# <a name="passwordauthenticationmethod-resetpassword"></a><span data-ttu-id="059fd-103">Пассвордаусентикатионмесод: Ресетпассворд</span><span class="sxs-lookup"><span data-stu-id="059fd-103">passwordAuthenticationMethod: resetPassword</span></span>

<span data-ttu-id="059fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="059fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="059fd-105">Инициация сброса пароля, связанного с объектом [метода проверки подлинности](../resources/passwordauthenticationmethod.md) с помощью пароля.</span><span class="sxs-lookup"><span data-stu-id="059fd-105">Initiate a reset for the password associated with a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> <span data-ttu-id="059fd-106">Это может сделать только администратор с соответствующими разрешениями и не может быть выполнен для собственной учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="059fd-106">This can only be done by an administrator with appropriate permissions and cannot be performed on a user's own account.</span></span>

<span data-ttu-id="059fd-107">Этот процесс записывает новый пароль в Azure Active Directory и передает его в локальную службу Active Directory, если она настроена с помощью обратной записи пароля.</span><span class="sxs-lookup"><span data-stu-id="059fd-107">This flow writes the new password to Azure Active Directory and pushes it to on-premises Active Directory if configured using password writeback.</span></span> <span data-ttu-id="059fd-108">Администратор может предоставить новый пароль или создать его в системе.</span><span class="sxs-lookup"><span data-stu-id="059fd-108">The admin can either provide a new password or have the system generate one.</span></span> <span data-ttu-id="059fd-109">Пользователю предлагается сменить пароль при следующем входе в систему.</span><span class="sxs-lookup"><span data-stu-id="059fd-109">The user is prompted to change their password on their next sign in.</span></span>

<span data-ttu-id="059fd-110">Этот сброс является длительной операцией и возвращает ссылку в `Location` заголовке, с которой вызывающий может периодически проверять состояние сброса.</span><span class="sxs-lookup"><span data-stu-id="059fd-110">This reset is a long-running operation and will return a link in the `Location` header where the caller can periodically check for the status of the reset.</span></span>

## <a name="permissions"></a><span data-ttu-id="059fd-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="059fd-111">Permissions</span></span>

<span data-ttu-id="059fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="059fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="059fd-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="059fd-114">Permission type</span></span>                        | <span data-ttu-id="059fd-115">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="059fd-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="059fd-116">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="059fd-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="059fd-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="059fd-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="059fd-118">Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="059fd-118">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="059fd-119">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="059fd-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="059fd-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="059fd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="059fd-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059fd-121">Not supported.</span></span> | <span data-ttu-id="059fd-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059fd-122">Not supported.</span></span> |
| <span data-ttu-id="059fd-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="059fd-123">Application</span></span>                            | <span data-ttu-id="059fd-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059fd-124">Not supported.</span></span> | <span data-ttu-id="059fd-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059fd-125">Not supported.</span></span> |

<span data-ttu-id="059fd-126">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="059fd-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="059fd-127">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="059fd-127">Global admin</span></span>
* <span data-ttu-id="059fd-128">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="059fd-128">Privileged authentication admin</span></span>
* <span data-ttu-id="059fd-129">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="059fd-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="059fd-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="059fd-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a><span data-ttu-id="059fd-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="059fd-131">Request headers</span></span>

| <span data-ttu-id="059fd-132">Имя</span><span class="sxs-lookup"><span data-stu-id="059fd-132">Name</span></span>          | <span data-ttu-id="059fd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="059fd-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="059fd-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="059fd-134">Authorization</span></span> | <span data-ttu-id="059fd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="059fd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="059fd-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="059fd-137">Content-type</span></span>  | <span data-ttu-id="059fd-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="059fd-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="059fd-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="059fd-140">Request body</span></span>

<span data-ttu-id="059fd-141">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="059fd-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="059fd-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="059fd-142">Parameter</span></span>    | <span data-ttu-id="059fd-143">Тип</span><span class="sxs-lookup"><span data-stu-id="059fd-143">Type</span></span>        | <span data-ttu-id="059fd-144">Описание</span><span class="sxs-lookup"><span data-stu-id="059fd-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="059fd-145">newPassword</span><span class="sxs-lookup"><span data-stu-id="059fd-145">newPassword</span></span>|<span data-ttu-id="059fd-146">String</span><span class="sxs-lookup"><span data-stu-id="059fd-146">String</span></span>|<span data-ttu-id="059fd-147">Новый пароль, введенный администратором. Необходим для клиентов со сценариями гибридного пароля.</span><span class="sxs-lookup"><span data-stu-id="059fd-147">The new password entered by the admin. Required for tenants with hybrid password scenarios.</span></span> <span data-ttu-id="059fd-148">Если параметр не задан для пароля в облаке, система возвращает пароль, созданный системой.</span><span class="sxs-lookup"><span data-stu-id="059fd-148">If omitted for a cloud-only password, the system returns a system-generated password.</span></span> <span data-ttu-id="059fd-149">Это строка Юникода без другой кодировки.</span><span class="sxs-lookup"><span data-stu-id="059fd-149">This is a unicode string with no other encoding.</span></span> <span data-ttu-id="059fd-150">Она проверяется относительно системы запрещенных паролей клиента перед принятием, а также должна соответствовать облачным и/или локальным требованиям к паролю клиента.</span><span class="sxs-lookup"><span data-stu-id="059fd-150">It is validated against the tenant's banned password system before acceptance, and must adhere to the tenant's cloud and/or on-premises password requirements.</span></span>|

## <a name="response"></a><span data-ttu-id="059fd-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="059fd-151">Response</span></span>

<span data-ttu-id="059fd-152">В случае успешного выполнения этот метод возвращает `202 ACCEPTED` код отклика и URL- `Location` адрес в заголовке.</span><span class="sxs-lookup"><span data-stu-id="059fd-152">If successful, this method returns a `202 ACCEPTED` response code and a URL in the `Location` header.</span></span>

<span data-ttu-id="059fd-153">Если вызывающий абонент не отправил пароль, то пароль, созданный корпорацией Майкрософт, предоставляется в объекте JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="059fd-153">If the caller did not submit a password, a Microsoft-generated password is provided in a JSON object in the response body.</span></span>

### <a name="response-headers"></a><span data-ttu-id="059fd-154">Заголовки откликов</span><span class="sxs-lookup"><span data-stu-id="059fd-154">Response headers</span></span>

| <span data-ttu-id="059fd-155">Имя</span><span class="sxs-lookup"><span data-stu-id="059fd-155">Name</span></span>        | <span data-ttu-id="059fd-156">Описание</span><span class="sxs-lookup"><span data-stu-id="059fd-156">Description</span></span>     |
|:------------|:----------------|
|<span data-ttu-id="059fd-157">Расположение</span><span class="sxs-lookup"><span data-stu-id="059fd-157">Location</span></span>     | <span data-ttu-id="059fd-158">URL-адрес, который необходимо вызвать для проверки состояния операции.</span><span class="sxs-lookup"><span data-stu-id="059fd-158">URL to call to check the status of the operation.</span></span>|
|<span data-ttu-id="059fd-159">Retry — после</span><span class="sxs-lookup"><span data-stu-id="059fd-159">Retry-after</span></span>  | <span data-ttu-id="059fd-160">Продолжительность в секундах.</span><span class="sxs-lookup"><span data-stu-id="059fd-160">Duration in seconds.</span></span>|

## <a name="examples"></a><span data-ttu-id="059fd-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="059fd-161">Examples</span></span>

### <a name="example-1-user-submitted-password"></a><span data-ttu-id="059fd-162">Пример 1: пароль, отправленный пользователем</span><span class="sxs-lookup"><span data-stu-id="059fd-162">Example 1: User-submitted password</span></span>

<span data-ttu-id="059fd-163">В приведенном ниже примере показано, как вызвать этот API, когда вызывающая сторона отправит пароль.</span><span class="sxs-lookup"><span data-stu-id="059fd-163">The following example shows how to call this API when the caller submits a password.</span></span>

#### <a name="request"></a><span data-ttu-id="059fd-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="059fd-164">Request</span></span>

<span data-ttu-id="059fd-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="059fd-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="059fd-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="059fd-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/authentication/passwordMethods/{id}/resetPassword
Content-type: application/json

{
  "newPassword": "newPassword-value",
}
```
# <a name="c"></a>[<span data-ttu-id="059fd-167">C#</span><span class="sxs-lookup"><span data-stu-id="059fd-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="059fd-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="059fd-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="059fd-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="059fd-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="059fd-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="059fd-170">Response</span></span>

<span data-ttu-id="059fd-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="059fd-171">The following is an example of the response.</span></span>

> <span data-ttu-id="059fd-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="059fd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 ACCEPTED
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/{id}/authentication/operations/{id}
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

### <a name="example-2-system-generated-password"></a><span data-ttu-id="059fd-174">Пример 2: пароль, созданный системой</span><span class="sxs-lookup"><span data-stu-id="059fd-174">Example 2: System-generated password</span></span>

<span data-ttu-id="059fd-175">В приведенном ниже примере показано, как вызывать этот API, когда вызывающий абонент не отправляет пароль.</span><span class="sxs-lookup"><span data-stu-id="059fd-175">The following example shows how to call this API when the caller does not submit a password.</span></span>

#### <a name="request"></a><span data-ttu-id="059fd-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="059fd-176">Request</span></span>

<span data-ttu-id="059fd-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="059fd-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="059fd-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="059fd-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/authentication/passwordMethods/{id}/resetPassword
```
# <a name="c"></a>[<span data-ttu-id="059fd-179">C#</span><span class="sxs-lookup"><span data-stu-id="059fd-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="059fd-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="059fd-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="059fd-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="059fd-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="059fd-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="059fd-182">Response</span></span>

<span data-ttu-id="059fd-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="059fd-183">The following is an example of the response.</span></span>

> <span data-ttu-id="059fd-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="059fd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/{id}/authentication/operations/{id}
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
