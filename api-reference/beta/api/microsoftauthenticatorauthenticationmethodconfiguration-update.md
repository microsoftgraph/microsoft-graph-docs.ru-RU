---
title: Обновление microsoftAuthenticatorAuthenticationMethodConfiguration
description: Обновление свойств объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bce76566495d0312679030b6e8b2fb16ea632fe9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473055"
---
# <a name="update-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="faf94-103">Обновление microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="faf94-103">Update microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="faf94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faf94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faf94-105">Обновим свойства объекта [MicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="faf94-105">Update the properties of a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>


## <a name="permissions"></a><span data-ttu-id="faf94-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="faf94-106">Permissions</span></span>
<span data-ttu-id="faf94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faf94-109">Permission type</span></span>|<span data-ttu-id="faf94-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="faf94-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faf94-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faf94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="faf94-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="faf94-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="faf94-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faf94-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faf94-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faf94-114">Not supported.</span></span>|
|<span data-ttu-id="faf94-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faf94-115">Application</span></span>|<span data-ttu-id="faf94-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="faf94-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="faf94-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="faf94-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="faf94-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="faf94-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="faf94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faf94-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="faf94-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faf94-120">Request headers</span></span>
|<span data-ttu-id="faf94-121">Имя</span><span class="sxs-lookup"><span data-stu-id="faf94-121">Name</span></span>|<span data-ttu-id="faf94-122">Описание</span><span class="sxs-lookup"><span data-stu-id="faf94-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="faf94-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faf94-123">Authorization</span></span>|<span data-ttu-id="faf94-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faf94-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="faf94-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="faf94-126">Content-Type</span></span>|<span data-ttu-id="faf94-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faf94-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf94-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="faf94-129">Request body</span></span>
<span data-ttu-id="faf94-130">В корпусе запроса необходимо предоставить представление JSON объекта [MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) со значениями полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="faf94-130">In the request body, supply a JSON representation of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="faf94-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="faf94-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="faf94-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="faf94-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="faf94-133">Список свойств см. в [списке microsoftAuthenticatorAuthenticationMethodConfiguration.](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf94-133">For the list of properties, see [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="faf94-134">**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` должно быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="faf94-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="faf94-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf94-135">Response</span></span>

<span data-ttu-id="faf94-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="faf94-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="faf94-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="faf94-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="faf94-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="faf94-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="faf94-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="faf94-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "state": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="faf94-141">C#</span><span class="sxs-lookup"><span data-stu-id="faf94-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-microsoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="faf94-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="faf94-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-microsoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="faf94-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="faf94-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-microsoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="faf94-144">Java</span><span class="sxs-lookup"><span data-stu-id="faf94-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-microsoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="faf94-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf94-145">Response</span></span>
<span data-ttu-id="faf94-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="faf94-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "129ae788-e788-129a-88e7-9a1288e79a12",
  "state": "String"
}
```

