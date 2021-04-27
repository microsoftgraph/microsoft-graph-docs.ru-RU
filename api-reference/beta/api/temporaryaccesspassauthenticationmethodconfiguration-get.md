---
title: Получить temporaryAccessPassAuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b0874968f9cce1b60a3b0f85a68ac4ccbf9a887e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049648"
---
# <a name="get-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="e9e7c-103">Получить temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9e7c-103">Get temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="e9e7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e7c-105">Ознакомьтесь с свойствами и отношениями объекта [temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) [](../resources/authenticationmethodspolicies-overview.md) который представляет политику метода проверки подлинности временных пропусков доступа для клиента Azure Active Directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-105">Read the properties and relationships of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object, which represents the Temporary Access Pass [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9e7c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9e7c-106">Permissions</span></span>
<span data-ttu-id="e9e7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9e7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e7c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9e7c-109">Permission type</span></span>|<span data-ttu-id="e9e7c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9e7c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9e7c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9e7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9e7c-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e9e7c-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e9e7c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9e7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9e7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-114">Not supported.</span></span>|
|<span data-ttu-id="e9e7c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9e7c-115">Application</span></span>|<span data-ttu-id="e9e7c-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e9e7c-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="e9e7c-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="e9e7c-118">Дополнительные сведения см. в[дополнительных сведениях.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e9e7c-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="e9e7c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9e7c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
## <a name="request-headers"></a><span data-ttu-id="e9e7c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9e7c-120">Request headers</span></span>
|<span data-ttu-id="e9e7c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e9e7c-121">Name</span></span>|<span data-ttu-id="e9e7c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e7c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e9e7c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9e7c-123">Authorization</span></span>|<span data-ttu-id="e9e7c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9e7c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9e7c-126">Request body</span></span>
<span data-ttu-id="e9e7c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e9e7c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9e7c-128">Response</span></span>
<span data-ttu-id="e9e7c-129">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-129">The following is an example of the response.</span></span>

<span data-ttu-id="e9e7c-130">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e9e7c-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodConfigurations/$entity",
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
    "id": "TemporaryAccessPass",
    "state": "enabled",
    "defaultLifetimeInMinutes": 60,
    "defaultLength": 12,
    "minimumLifetimeInMinutes": 60,
    "maximumLifetimeInMinutes": 1440,
    "isUsableOnce": false,
    "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('TemporaryAccessPass')/microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration/includeTargets",
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false
        }
    ]
}
```