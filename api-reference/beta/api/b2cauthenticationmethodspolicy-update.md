---
title: Обновление b2cAuthenticationMethodsPolicy
description: Обновление свойств объекта b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc40a64c1af6282b0a618062cb9a0bb4cc62cc5e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458049"
---
# <a name="update-b2cauthenticationmethodspolicy"></a><span data-ttu-id="16bc1-103">Обновление b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="16bc1-103">Update b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="16bc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16bc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16bc1-105">Обновление свойств объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="16bc1-105">Update the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16bc1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16bc1-106">Permissions</span></span>

<span data-ttu-id="16bc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16bc1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16bc1-109">Permission type</span></span>                        | <span data-ttu-id="16bc1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16bc1-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="16bc1-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16bc1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16bc1-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="16bc1-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="16bc1-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16bc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16bc1-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="16bc1-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
| <span data-ttu-id="16bc1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16bc1-115">Application</span></span>                            | <span data-ttu-id="16bc1-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="16bc1-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="16bc1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16bc1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="16bc1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16bc1-118">Request headers</span></span>

|<span data-ttu-id="16bc1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="16bc1-119">Name</span></span>|<span data-ttu-id="16bc1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16bc1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16bc1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16bc1-121">Authorization</span></span>|<span data-ttu-id="16bc1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16bc1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="16bc1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16bc1-124">Content-Type</span></span>|<span data-ttu-id="16bc1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16bc1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16bc1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16bc1-127">Request body</span></span>

<span data-ttu-id="16bc1-128">В тексте запроса предоставьте описание объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16bc1-128">In the request body, supply a JSON representation of the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

<span data-ttu-id="16bc1-129">В таблице ниже показаны свойства, требуемые при обновлении [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="16bc1-129">The following table shows the properties that are required when you update the [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span></span>

| <span data-ttu-id="16bc1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16bc1-130">Property</span></span>     | <span data-ttu-id="16bc1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16bc1-131">Type</span></span>        | <span data-ttu-id="16bc1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16bc1-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16bc1-133">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="16bc1-133">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="16bc1-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="16bc1-134">Boolean</span></span>|<span data-ttu-id="16bc1-135">Администратор клиента может настраивать локальные учетные записи, используя электронную почту, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="16bc1-135">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="16bc1-136">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="16bc1-136">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="16bc1-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="16bc1-137">Boolean</span></span>|<span data-ttu-id="16bc1-138">Администратор клиента может настраивать локальные учетные записи, используя имя пользователя, если включен метод проверки подлинности электронной почты и пароля.</span><span class="sxs-lookup"><span data-stu-id="16bc1-138">The tenant admin can configure local accounts using username if the user name and password authentication method is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="16bc1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="16bc1-139">Response</span></span>

<span data-ttu-id="16bc1-140">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="16bc1-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16bc1-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="16bc1-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16bc1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="16bc1-142">Request</span></span>

<span data-ttu-id="16bc1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16bc1-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16bc1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="16bc1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="16bc1-145">C#</span><span class="sxs-lookup"><span data-stu-id="16bc1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16bc1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16bc1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16bc1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16bc1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16bc1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="16bc1-148">Response</span></span>

<span data-ttu-id="16bc1-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="16bc1-149">The following is an example of the response.</span></span>

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
