---
title: Получить emailAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e3e2fd05c8d4f2d3f3036c55a6f9c817e2ba9c91
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436311"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="d2f79-103">Получить emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2f79-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="d2f79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2f79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f79-105">Ознакомьтесь с свойствами и отношениями объекта [электронной почтыAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности [OTP](../resources/authenticationmethodspolicies-overview.md) электронной почты для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d2f79-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f79-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f79-106">Permissions</span></span>

<span data-ttu-id="d2f79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f79-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f79-109">Permission type</span></span>|<span data-ttu-id="d2f79-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f79-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2f79-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f79-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d2f79-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d2f79-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2f79-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f79-114">Not supported.</span></span>|
|<span data-ttu-id="d2f79-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f79-115">Application</span></span>|<span data-ttu-id="d2f79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f79-116">Not supported.</span></span>|

<span data-ttu-id="d2f79-117">Для делегирования сценариев администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="d2f79-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d2f79-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d2f79-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d2f79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f79-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="d2f79-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f79-120">Request headers</span></span>

|<span data-ttu-id="d2f79-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2f79-121">Name</span></span>|<span data-ttu-id="d2f79-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d2f79-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2f79-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f79-123">Authorization</span></span>|<span data-ttu-id="d2f79-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f79-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f79-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2f79-126">Request body</span></span>

<span data-ttu-id="d2f79-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f79-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2f79-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f79-128">Response</span></span>

<span data-ttu-id="d2f79-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2f79-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2f79-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2f79-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2f79-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f79-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="d2f79-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f79-132">Response</span></span>

<span data-ttu-id="d2f79-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2f79-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "allowExternalIdToUseEmailOtp": "True",
    "includeTargets":[
        {
          "targetType":"group",
          "id":"all_users",
          "isRegistrationRequired":false,
        }
    ]
  }
}
```

