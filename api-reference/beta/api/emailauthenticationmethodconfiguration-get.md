---
title: Получение Емаилаусентикатионмесодконфигуратион
description: Чтение свойств и связей объекта Емаилаусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5fb2396563ed91f2844867e7ba3780f40644902a
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617146"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="9e9b3-103">Получение Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9e9b3-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="9e9b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e9b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e9b3-105">Прочитайте свойства и связи объекта [емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md) , представляющего [политику метода проверки подлинности методом проверки подлинности методом проверки подлинности](../resources/authenticationmethodspolicies-overview.md) методом OTP для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="9e9b3-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e9b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9b3-106">Permissions</span></span>

<span data-ttu-id="9e9b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e9b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e9b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9b3-109">Permission type</span></span>|<span data-ttu-id="9e9b3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e9b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e9b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e9b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e9b3-112">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9e9b3-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="9e9b3-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e9b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e9b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9b3-114">Not supported.</span></span>|
|<span data-ttu-id="9e9b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e9b3-115">Application</span></span>|<span data-ttu-id="9e9b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9b3-116">Not supported.</span></span>|

<span data-ttu-id="9e9b3-117">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="9e9b3-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9e9b3-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9e9b3-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9e9b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e9b3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="9e9b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e9b3-120">Request headers</span></span>

|<span data-ttu-id="9e9b3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9e9b3-121">Name</span></span>|<span data-ttu-id="9e9b3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9b3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9e9b3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e9b3-123">Authorization</span></span>|<span data-ttu-id="9e9b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e9b3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e9b3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e9b3-126">Request body</span></span>

<span data-ttu-id="9e9b3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e9b3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e9b3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9b3-128">Response</span></span>

<span data-ttu-id="9e9b3-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e9b3-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e9b3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e9b3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e9b3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e9b3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="9e9b3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9b3-132">Response</span></span>

<span data-ttu-id="9e9b3-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9e9b3-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

