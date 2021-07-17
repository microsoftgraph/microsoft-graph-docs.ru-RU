---
title: Получить emailAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 15aa3de4b66b566c1943709330478d035ead0977
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442950"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="46d0b-103">Получить emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="46d0b-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="46d0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46d0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46d0b-105">Ознакомьтесь с свойствами и отношениями объекта [электронной почтыAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности [OTP](../resources/authenticationmethodspolicies-overview.md) электронной почты для клиента Azure Active Directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="46d0b-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="46d0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46d0b-106">Permissions</span></span>

<span data-ttu-id="46d0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46d0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46d0b-109">Permission type</span></span>|<span data-ttu-id="46d0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46d0b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46d0b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46d0b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46d0b-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="46d0b-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="46d0b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46d0b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46d0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46d0b-114">Not supported.</span></span>|
|<span data-ttu-id="46d0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46d0b-115">Application</span></span>|<span data-ttu-id="46d0b-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="46d0b-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="46d0b-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="46d0b-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="46d0b-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="46d0b-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="46d0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46d0b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="46d0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46d0b-120">Request headers</span></span>

|<span data-ttu-id="46d0b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="46d0b-121">Name</span></span>|<span data-ttu-id="46d0b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="46d0b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46d0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46d0b-123">Authorization</span></span>|<span data-ttu-id="46d0b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46d0b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d0b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46d0b-126">Request body</span></span>

<span data-ttu-id="46d0b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46d0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46d0b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="46d0b-128">Response</span></span>

<span data-ttu-id="46d0b-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="46d0b-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46d0b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="46d0b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46d0b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="46d0b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46d0b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="46d0b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```msgraph-interactive
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```
# <a name="c"></a>[<span data-ttu-id="46d0b-133">C#</span><span class="sxs-lookup"><span data-stu-id="46d0b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46d0b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46d0b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46d0b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46d0b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46d0b-136">Java</span><span class="sxs-lookup"><span data-stu-id="46d0b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46d0b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="46d0b-137">Response</span></span>

<span data-ttu-id="46d0b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="46d0b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "id": "Email",
    "state": "enabled",
    "allowExternalIdToUseEmailOtp": "enabled"
  }
}
```
