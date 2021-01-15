---
title: Get emailAuthenticationMethodConfiguration
description: Чтение свойств и связей объекта emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82f1653e5fdf091bd92638b4596bacd4b8194817
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873327"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="5b971-103">Get emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b971-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="5b971-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b971-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b971-105">Прочитайте свойства и связи объекта [emailAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности [OTP](../resources/authenticationmethodspolicies-overview.md) электронной почты для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5b971-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b971-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b971-106">Permissions</span></span>

<span data-ttu-id="5b971-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b971-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b971-109">Permission type</span></span>|<span data-ttu-id="5b971-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b971-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b971-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b971-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b971-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5b971-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5b971-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b971-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b971-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b971-114">Not supported.</span></span>|
|<span data-ttu-id="5b971-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b971-115">Application</span></span>|<span data-ttu-id="5b971-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b971-116">Not supported.</span></span>|

<span data-ttu-id="5b971-117">Для делегирования сценариев администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="5b971-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5b971-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5b971-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5b971-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b971-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="5b971-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b971-120">Request headers</span></span>

|<span data-ttu-id="5b971-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5b971-121">Name</span></span>|<span data-ttu-id="5b971-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b971-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5b971-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b971-123">Authorization</span></span>|<span data-ttu-id="5b971-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b971-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b971-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b971-126">Request body</span></span>

<span data-ttu-id="5b971-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b971-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b971-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b971-128">Response</span></span>

<span data-ttu-id="5b971-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b971-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b971-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b971-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b971-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b971-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="5b971-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b971-132">Response</span></span>

<span data-ttu-id="5b971-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b971-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

