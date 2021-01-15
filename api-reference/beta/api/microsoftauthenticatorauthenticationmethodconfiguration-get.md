---
title: Get microsoftAuthenticatorAuthenticationMethodConfiguration
description: Чтение свойств и связей объекта microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8eb1862fc301edb154d334f62cd82958abb39071
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874514"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="72a11-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="72a11-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="72a11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72a11-105">Извлечение свойств и связей объекта [microsoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности Microsoft Authenticator для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="72a11-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="72a11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72a11-106">Permissions</span></span>
<span data-ttu-id="72a11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72a11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72a11-109">Permission type</span></span>|<span data-ttu-id="72a11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72a11-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72a11-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72a11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72a11-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="72a11-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="72a11-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72a11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72a11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a11-114">Not supported.</span></span>|
|<span data-ttu-id="72a11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72a11-115">Application</span></span>|<span data-ttu-id="72a11-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="72a11-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="72a11-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="72a11-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="72a11-118">Дополнительные сведения см. в [сведениях о роли.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="72a11-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="72a11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72a11-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="72a11-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72a11-120">Request headers</span></span>
|<span data-ttu-id="72a11-121">Имя</span><span class="sxs-lookup"><span data-stu-id="72a11-121">Name</span></span>|<span data-ttu-id="72a11-122">Описание</span><span class="sxs-lookup"><span data-stu-id="72a11-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72a11-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72a11-123">Authorization</span></span>|<span data-ttu-id="72a11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72a11-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72a11-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72a11-126">Request body</span></span>
<span data-ttu-id="72a11-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72a11-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72a11-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a11-128">Response</span></span>

<span data-ttu-id="72a11-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72a11-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72a11-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="72a11-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72a11-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72a11-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="72a11-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a11-132">Response</span></span>
<span data-ttu-id="72a11-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72a11-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

