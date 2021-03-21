---
title: Получить emailAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce3336973819f1b3062912b361c1d513e0d9098c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964851"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="f26f7-103">Получить emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="f26f7-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="f26f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f26f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f26f7-105">Ознакомьтесь с свойствами и отношениями объекта [электронной почтыAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности [OTP](../resources/authenticationmethodspolicies-overview.md) электронной почты для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f26f7-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f26f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f26f7-106">Permissions</span></span>

<span data-ttu-id="f26f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f26f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f26f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f26f7-109">Permission type</span></span>|<span data-ttu-id="f26f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f26f7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f26f7-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f26f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f26f7-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f26f7-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="f26f7-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f26f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f26f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f26f7-114">Not supported.</span></span>|
|<span data-ttu-id="f26f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f26f7-115">Application</span></span>|<span data-ttu-id="f26f7-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f26f7-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="f26f7-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="f26f7-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="f26f7-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="f26f7-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="f26f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f26f7-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="f26f7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f26f7-120">Request headers</span></span>

|<span data-ttu-id="f26f7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f26f7-121">Name</span></span>|<span data-ttu-id="f26f7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f26f7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f26f7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f26f7-123">Authorization</span></span>|<span data-ttu-id="f26f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f26f7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f26f7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f26f7-126">Request body</span></span>

<span data-ttu-id="f26f7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f26f7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f26f7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f26f7-128">Response</span></span>

<span data-ttu-id="f26f7-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f26f7-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f26f7-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f26f7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f26f7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f26f7-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="f26f7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f26f7-132">Response</span></span>

<span data-ttu-id="f26f7-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f26f7-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "allowExternalIdToUseEmailOtp": "True"
  }
}
```
