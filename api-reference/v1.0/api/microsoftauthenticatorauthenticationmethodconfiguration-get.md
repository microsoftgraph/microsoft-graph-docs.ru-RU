---
title: Получите microsoftAuthenticatorAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f94c20bcfb29de6af6ec77371594b367ed93e88b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949031"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="a659d-103">Получите microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="a659d-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="a659d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a659d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a659d-105">Извлечение свойств и связей объекта [MicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a659d-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a659d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a659d-106">Permissions</span></span>
<span data-ttu-id="a659d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a659d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a659d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a659d-109">Permission type</span></span>|<span data-ttu-id="a659d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a659d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a659d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a659d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a659d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a659d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="a659d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a659d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a659d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a659d-114">Not supported.</span></span>|
|<span data-ttu-id="a659d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a659d-115">Application</span></span>|<span data-ttu-id="a659d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a659d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="a659d-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="a659d-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="a659d-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="a659d-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="a659d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a659d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="a659d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a659d-120">Request headers</span></span>
|<span data-ttu-id="a659d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a659d-121">Name</span></span>|<span data-ttu-id="a659d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a659d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a659d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a659d-123">Authorization</span></span>|<span data-ttu-id="a659d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a659d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a659d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a659d-126">Request body</span></span>
<span data-ttu-id="a659d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a659d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a659d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a659d-128">Response</span></span>

<span data-ttu-id="a659d-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a659d-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a659d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a659d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a659d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a659d-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="a659d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a659d-132">Response</span></span>
<span data-ttu-id="a659d-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a659d-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "129ae788-e788-129a-88e7-9a1288e79a12",
    "state": "String"
  }
}
```

