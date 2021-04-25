---
title: Обновление b2cAuthenticationMethodsPolicy
description: Обновление свойств объекта b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f2da149c32e10c0871decf1f8be96144b66b173a
ms.sourcegitcommit: 92f545d2d9af13ac7aff9932eb265f136d089f79
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2021
ms.locfileid: "51996126"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="cb2c8-103">Обновление b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="cb2c8-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="cb2c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb2c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb2c8-105">Обновление свойств объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cb2c8-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb2c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb2c8-106">Permissions</span></span>

<span data-ttu-id="cb2c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb2c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb2c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb2c8-109">Permission type</span></span>                        | <span data-ttu-id="cb2c8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb2c8-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="cb2c8-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb2c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb2c8-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb2c8-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="cb2c8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb2c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb2c8-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb2c8-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="cb2c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb2c8-115">Application</span></span>                            | <span data-ttu-id="cb2c8-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb2c8-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb2c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb2c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="cb2c8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb2c8-118">Request headers</span></span>

|<span data-ttu-id="cb2c8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cb2c8-119">Name</span></span>|<span data-ttu-id="cb2c8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb2c8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb2c8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb2c8-121">Authorization</span></span>|<span data-ttu-id="cb2c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cb2c8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb2c8-124">Content-Type</span></span>|<span data-ttu-id="cb2c8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb2c8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb2c8-127">Request body</span></span>

<span data-ttu-id="cb2c8-128">В тексте запроса предоставьте описание объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="cb2c8-129">В таблице ниже показаны свойства, требуемые при обновлении [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cb2c8-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="cb2c8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb2c8-130">Property</span></span>     | <span data-ttu-id="cb2c8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb2c8-131">Type</span></span>        | <span data-ttu-id="cb2c8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb2c8-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb2c8-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="cb2c8-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="cb2c8-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="cb2c8-134">Boolean</span></span>|<span data-ttu-id="cb2c8-135">Администратор клиента может настраивать локальные учетные записи, используя электронную почту, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="cb2c8-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="cb2c8-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="cb2c8-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="cb2c8-137">Boolean</span></span>|<span data-ttu-id="cb2c8-138">Администратор клиента может настраивать локальные учетные записи, используя имя пользователя, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-138">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|
|<span data-ttu-id="cb2c8-139">isPhoneOneTimePasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="cb2c8-139">isPhoneOneTimePasswordAuthenticationEnabled</span></span>|<span data-ttu-id="cb2c8-140">Логический</span><span class="sxs-lookup"><span data-stu-id="cb2c8-140">Boolean</span></span>|<span data-ttu-id="cb2c8-141">Администратор клиента может настраивать локальные учетные записи, используя номер телефона, если включен метод проверки подлинности по номеру телефона и одноразовому паролю.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-141">The tenant admin can configure local accounts using phone number if the phone number and one-time password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="cb2c8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb2c8-142">Response</span></span>

<span data-ttu-id="cb2c8-143">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-143">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb2c8-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb2c8-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb2c8-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb2c8-145">Request</span></span>

<span data-ttu-id="cb2c8-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cb2c8-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb2c8-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true,
    "isPhoneOneTimePasswordAuthenticationEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="cb2c8-148">C#</span><span class="sxs-lookup"><span data-stu-id="cb2c8-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb2c8-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb2c8-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb2c8-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb2c8-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb2c8-151">Java</span><span class="sxs-lookup"><span data-stu-id="cb2c8-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb2c8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb2c8-152">Response</span></span>

<span data-ttu-id="cb2c8-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cb2c8-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cauthenticationmethodspolicy"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update b2cauthenticationmethodspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
