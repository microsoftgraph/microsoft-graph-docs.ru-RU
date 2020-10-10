---
title: Создание Фонеаусентикатионмесод
description: Добавление нового метода проверки подлинности телефона.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48133bff3dc0532c2669a608697e1fca1a10d9ca
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417781"
---
# <a name="create-phoneauthenticationmethod"></a><span data-ttu-id="ba4c5-103">Создание Фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ba4c5-103">Create phoneAuthenticationMethod</span></span>

<span data-ttu-id="ba4c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba4c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba4c5-105">Добавление нового [метода проверки подлинности телефона](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="ba4c5-105">Add a new [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> <span data-ttu-id="ba4c5-106">У пользователя может быть только один телефон каждого типа, записанный в свойстве **фонетипе** .</span><span class="sxs-lookup"><span data-stu-id="ba4c5-106">A user may only have one phone of each type, captured in the **phoneType** property.</span></span> <span data-ttu-id="ba4c5-107">Это означает, что, например, `mobile` при добавлении телефона в пользователя с уже существующим `mobile` телефоном произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-107">This means, for example, adding a `mobile` phone to a user with a preexisting `mobile` phone will fail.</span></span> <span data-ttu-id="ba4c5-108">Кроме того, перед добавлением телефона у пользователя всегда должен быть `mobile` Телефон `alternateMobile` .</span><span class="sxs-lookup"><span data-stu-id="ba4c5-108">Additionally, a user must always have a `mobile` phone before adding an `alternateMobile` phone.</span></span>

<span data-ttu-id="ba4c5-109">Добавление телефонного номера делает его доступным для использования в Azure Multi-Factor Authentication (MFA) и самостоятельном сбросе пароля (SSPR), если он включен.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-109">Adding a phone number makes it available for use in both Azure multi-factor authentication (MFA) and self-service password reset (SSPR), if enabled.</span></span>

<span data-ttu-id="ba4c5-110">Кроме того, если для пользователя включена политика для входа в SMS и `mobile` добавляется номер, система попытается зарегистрировать номер для использования в этой системе.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-110">Additionally, if a user is enabled by policy to use SMS sign-in and a `mobile` number is added, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba4c5-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba4c5-111">Permissions</span></span>

<span data-ttu-id="ba4c5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba4c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba4c5-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba4c5-114">Permission type</span></span>                        | <span data-ttu-id="ba4c5-115">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="ba4c5-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="ba4c5-116">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="ba4c5-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ba4c5-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba4c5-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba4c5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-118">Not supported.</span></span> | <span data-ttu-id="ba4c5-119">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ba4c5-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ba4c5-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba4c5-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba4c5-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-121">Not supported.</span></span> | <span data-ttu-id="ba4c5-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-122">Not supported.</span></span> |
| <span data-ttu-id="ba4c5-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba4c5-123">Application</span></span>                            | <span data-ttu-id="ba4c5-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-124">Not supported.</span></span> | <span data-ttu-id="ba4c5-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-125">Not supported.</span></span> |

<span data-ttu-id="ba4c5-126">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="ba4c5-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="ba4c5-127">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ba4c5-127">Global admin</span></span>
* <span data-ttu-id="ba4c5-128">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ba4c5-128">Privileged authentication admin</span></span>
* <span data-ttu-id="ba4c5-129">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ba4c5-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ba4c5-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba4c5-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="request-headers"></a><span data-ttu-id="ba4c5-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba4c5-131">Request headers</span></span>

| <span data-ttu-id="ba4c5-132">Имя</span><span class="sxs-lookup"><span data-stu-id="ba4c5-132">Name</span></span>          | <span data-ttu-id="ba4c5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ba4c5-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ba4c5-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba4c5-134">Authorization</span></span> | <span data-ttu-id="ba4c5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba4c5-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba4c5-137">Content-Type</span></span>  | <span data-ttu-id="ba4c5-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba4c5-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba4c5-140">Request body</span></span>

<span data-ttu-id="ba4c5-141">В тексте запроса добавьте представление объекта [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-141">In the request body, supply a JSON representation of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="ba4c5-142">Формат JSON должен включать `phoneNumber` и `phoneType` , но не `smsSignInState` (доступен только для чтения).</span><span class="sxs-lookup"><span data-stu-id="ba4c5-142">The JSON must include `phoneNumber` and `phoneType`, but not `smsSignInState` (which is read-only).</span></span>

| <span data-ttu-id="ba4c5-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba4c5-143">Property</span></span>     | <span data-ttu-id="ba4c5-144">Тип</span><span class="sxs-lookup"><span data-stu-id="ba4c5-144">Type</span></span>        | <span data-ttu-id="ba4c5-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ba4c5-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba4c5-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ba4c5-146">phoneNumber</span></span>|<span data-ttu-id="ba4c5-147">String</span><span class="sxs-lookup"><span data-stu-id="ba4c5-147">String</span></span>|<span data-ttu-id="ba4c5-148">Номер телефона для текста или вызов для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="ba4c5-149">Номера телефонов используют формат "+ \<country code\> \<number\> x \<extension\> " с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="ba4c5-150">Например, допустимые + 1 5555551234 или + 1 5555551234x123.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="ba4c5-151">При создании или обновлении числа отклоняются, если они не совпадают с требуемым форматом.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="ba4c5-152">фонетипе</span><span class="sxs-lookup"><span data-stu-id="ba4c5-152">phoneType</span></span>|<span data-ttu-id="ba4c5-153">String</span><span class="sxs-lookup"><span data-stu-id="ba4c5-153">String</span></span>|<span data-ttu-id="ba4c5-154">Возможные значения: `mobile` , `alternateMobile` и `office` .</span><span class="sxs-lookup"><span data-stu-id="ba4c5-154">Possible values are: `mobile`, `alternateMobile`, and `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="ba4c5-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba4c5-155">Response</span></span>

<span data-ttu-id="ba4c5-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-156">If successful, this method returns a `201 Created` response code and a new [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba4c5-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba4c5-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba4c5-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba4c5-158">Request</span></span>

<span data-ttu-id="ba4c5-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba4c5-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba4c5-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba4c5-161">C#</span><span class="sxs-lookup"><span data-stu-id="ba4c5-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba4c5-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba4c5-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba4c5-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba4c5-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba4c5-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba4c5-164">Response</span></span>

<span data-ttu-id="ba4c5-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-165">The following is an example of the response.</span></span>

> <span data-ttu-id="ba4c5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba4c5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
