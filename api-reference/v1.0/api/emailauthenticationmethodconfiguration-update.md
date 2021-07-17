---
title: Обновление emailAuthenticationMethodConfiguration
description: Обновление свойств объекта emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9ceff3ec236e607e531a0a95f6763bcab10b3609
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442903"
---
# <a name="update-emailauthenticationmethodconfiguration"></a><span data-ttu-id="86589-103">Обновление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="86589-103">Update emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="86589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86589-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86589-105">Обновим свойства объекта [emailAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности [OTP](../resources/authenticationmethodspolicies-overview.md) электронной почты для клиента Azure Active Directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="86589-105">Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="86589-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86589-106">Permissions</span></span>
<span data-ttu-id="86589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86589-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86589-109">Permission type</span></span>|<span data-ttu-id="86589-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86589-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86589-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86589-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86589-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86589-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="86589-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86589-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86589-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86589-114">Not supported.</span></span>|
|<span data-ttu-id="86589-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86589-115">Application</span></span>|<span data-ttu-id="86589-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86589-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="86589-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="86589-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="86589-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="86589-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="86589-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86589-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="86589-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86589-120">Request headers</span></span>

|<span data-ttu-id="86589-121">Имя</span><span class="sxs-lookup"><span data-stu-id="86589-121">Name</span></span>|<span data-ttu-id="86589-122">Описание</span><span class="sxs-lookup"><span data-stu-id="86589-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86589-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86589-123">Authorization</span></span>|<span data-ttu-id="86589-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86589-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86589-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86589-126">Content-Type</span></span>|<span data-ttu-id="86589-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86589-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86589-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86589-129">Request body</span></span>

<span data-ttu-id="86589-130">В теле запроса поставляем представление JSON объекта [emailAuthenticationMethodConfiguration.](../resources/emailauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86589-130">In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.</span></span> <span data-ttu-id="86589-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="86589-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="86589-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="86589-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="86589-133">Список свойств, которые можно обновить, см. в электронной [почтеAuthenticationMethodConfiguration.](../resources/emailauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86589-133">For the list of properties that can be updated, see [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="86589-134">**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.emailAuthenticationMethodConfiguration` должно быть включено в тело.</span><span class="sxs-lookup"><span data-stu-id="86589-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.emailAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="86589-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="86589-135">Response</span></span>

<span data-ttu-id="86589-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86589-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86589-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="86589-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86589-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="86589-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="86589-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="86589-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "enabled",
}
```
# <a name="c"></a>[<span data-ttu-id="86589-141">C#</span><span class="sxs-lookup"><span data-stu-id="86589-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86589-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86589-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86589-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86589-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86589-144">Java</span><span class="sxs-lookup"><span data-stu-id="86589-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86589-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="86589-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 NO CONTENT
```

