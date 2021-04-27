---
title: Создание phoneAuthenticationMethod
description: Добавьте новый метод проверки подлинности телефона.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6b2490cb0d2c7e625c83b1e3d5075e8f6a815e69
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047996"
---
# <a name="create-phoneauthenticationmethod"></a><span data-ttu-id="69fad-103">Создание phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="69fad-103">Create phoneAuthenticationMethod</span></span>

<span data-ttu-id="69fad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69fad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69fad-105">Добавьте новый [метод проверки подлинности телефона.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="69fad-105">Add a new [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> <span data-ttu-id="69fad-106">У пользователя может быть только один телефон каждого типа, захваченный в **свойстве phoneType.**</span><span class="sxs-lookup"><span data-stu-id="69fad-106">A user may only have one phone of each type, captured in the **phoneType** property.</span></span> <span data-ttu-id="69fad-107">Это означает, например, что добавление телефона пользователю с `mobile` предустанавливным телефоном не `mobile` удастся.</span><span class="sxs-lookup"><span data-stu-id="69fad-107">This means, for example, adding a `mobile` phone to a user with a preexisting `mobile` phone will fail.</span></span> <span data-ttu-id="69fad-108">Кроме того, перед добавлением телефона у пользователя всегда должен быть `mobile` `alternateMobile` телефон.</span><span class="sxs-lookup"><span data-stu-id="69fad-108">Additionally, a user must always have a `mobile` phone before adding an `alternateMobile` phone.</span></span>

<span data-ttu-id="69fad-109">Добавление номера телефона делает его доступным для использования в многофакторной проверке подлинности Azure (MFA) и сбросе пароля самообслуживления (SSPR), если включена.</span><span class="sxs-lookup"><span data-stu-id="69fad-109">Adding a phone number makes it available for use in both Azure multi-factor authentication (MFA) and self-service password reset (SSPR), if enabled.</span></span>

<span data-ttu-id="69fad-110">Кроме того, если политика позволяет пользователю использовать SMS входа и добавляется номер, система попытается зарегистрировать номер для использования в `mobile` этой системе.</span><span class="sxs-lookup"><span data-stu-id="69fad-110">Additionally, if a user is enabled by policy to use SMS sign-in and a `mobile` number is added, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="69fad-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69fad-111">Permissions</span></span>

<span data-ttu-id="69fad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69fad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69fad-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69fad-114">Permission type</span></span>                        | <span data-ttu-id="69fad-115">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="69fad-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="69fad-116">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="69fad-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="69fad-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69fad-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="69fad-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69fad-118">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="69fad-119">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69fad-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="69fad-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69fad-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69fad-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69fad-121">Not supported.</span></span> | <span data-ttu-id="69fad-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69fad-122">Not supported.</span></span> |
| <span data-ttu-id="69fad-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="69fad-123">Application</span></span>                            | <span data-ttu-id="69fad-124">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="69fad-124">Not applicable.</span></span> | <span data-ttu-id="69fad-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69fad-125">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="69fad-126">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="69fad-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="69fad-127">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="69fad-127">Global admin</span></span>
* <span data-ttu-id="69fad-128">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="69fad-128">Privileged authentication admin</span></span>
* <span data-ttu-id="69fad-129">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="69fad-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="69fad-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69fad-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="request-headers"></a><span data-ttu-id="69fad-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69fad-131">Request headers</span></span>

| <span data-ttu-id="69fad-132">Имя</span><span class="sxs-lookup"><span data-stu-id="69fad-132">Name</span></span>          | <span data-ttu-id="69fad-133">Описание</span><span class="sxs-lookup"><span data-stu-id="69fad-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="69fad-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69fad-134">Authorization</span></span> | <span data-ttu-id="69fad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69fad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69fad-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69fad-137">Content-Type</span></span>  | <span data-ttu-id="69fad-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69fad-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69fad-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69fad-140">Request body</span></span>

<span data-ttu-id="69fad-141">В теле запроса поставляем JSON-представление объекта [phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="69fad-141">In the request body, supply a JSON representation of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="69fad-142">JSON должен включать и не включать `phoneNumber` `phoneType` `smsSignInState` (только для чтения).</span><span class="sxs-lookup"><span data-stu-id="69fad-142">The JSON must include `phoneNumber` and `phoneType`, but not `smsSignInState` (which is read-only).</span></span>

| <span data-ttu-id="69fad-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="69fad-143">Property</span></span>     | <span data-ttu-id="69fad-144">Тип</span><span class="sxs-lookup"><span data-stu-id="69fad-144">Type</span></span>        | <span data-ttu-id="69fad-145">Описание</span><span class="sxs-lookup"><span data-stu-id="69fad-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69fad-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="69fad-146">phoneNumber</span></span>|<span data-ttu-id="69fad-147">String</span><span class="sxs-lookup"><span data-stu-id="69fad-147">String</span></span>|<span data-ttu-id="69fad-148">Номер телефона для текста или вызова для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="69fad-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="69fad-149">Телефон номера используют формат "+ \<country code\> \<number\> \<extension\> x", с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="69fad-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="69fad-150">Например, допустимы +1 5555551234 или +1 5555551234x1233.</span><span class="sxs-lookup"><span data-stu-id="69fad-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="69fad-151">При создании и обновлении номера отклоняется, если они не соответствуют требуемой форме.</span><span class="sxs-lookup"><span data-stu-id="69fad-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="69fad-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="69fad-152">phoneType</span></span>|<span data-ttu-id="69fad-153">String</span><span class="sxs-lookup"><span data-stu-id="69fad-153">String</span></span>|<span data-ttu-id="69fad-154">Возможные значения: `mobile` , `alternateMobile` и `office` .</span><span class="sxs-lookup"><span data-stu-id="69fad-154">Possible values are: `mobile`, `alternateMobile`, and `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="69fad-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="69fad-155">Response</span></span>

<span data-ttu-id="69fad-156">В случае успешной работы этот метод возвращает код ответа и новый `201 Created` [объект phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="69fad-156">If successful, this method returns a `201 Created` response code and a new [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69fad-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="69fad-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69fad-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="69fad-158">Request</span></span>

<span data-ttu-id="69fad-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69fad-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69fad-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="69fad-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile"
}
```
# <a name="c"></a>[<span data-ttu-id="69fad-161">C#</span><span class="sxs-lookup"><span data-stu-id="69fad-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69fad-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69fad-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69fad-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69fad-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69fad-164">Java</span><span class="sxs-lookup"><span data-stu-id="69fad-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-phoneauthenticationmethod-from-authentication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69fad-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="69fad-165">Response</span></span>

<span data-ttu-id="69fad-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69fad-166">The following is an example of the response.</span></span>

> <span data-ttu-id="69fad-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="69fad-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "phoneType-value",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
