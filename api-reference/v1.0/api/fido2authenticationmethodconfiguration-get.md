---
title: Get fido2AuthenticationMethodConfiguration
description: Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b517d9e8577c52b94f9f5bec301dc92495d00031
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964868"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="410d0-103">Get fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="410d0-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="410d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="410d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="410d0-105">Извлечение свойств и связей объекта [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) который представляет [](../resources/authenticationmethodspolicies-overview.md) политику метода проверки подлинности ключей безопасности FIDO2 для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="410d0-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="410d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="410d0-106">Permissions</span></span>
<span data-ttu-id="410d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="410d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="410d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="410d0-109">Permission type</span></span>|<span data-ttu-id="410d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="410d0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="410d0-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="410d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="410d0-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="410d0-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="410d0-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="410d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="410d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="410d0-114">Not supported.</span></span>|
|<span data-ttu-id="410d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="410d0-115">Application</span></span>|<span data-ttu-id="410d0-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="410d0-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="410d0-117">Для делегирования сценариев администратору требуется роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="410d0-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="410d0-118">Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="410d0-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="410d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="410d0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="410d0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="410d0-120">Request headers</span></span>
|<span data-ttu-id="410d0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="410d0-121">Name</span></span>|<span data-ttu-id="410d0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="410d0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="410d0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="410d0-123">Authorization</span></span>|<span data-ttu-id="410d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="410d0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="410d0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="410d0-126">Request body</span></span>
<span data-ttu-id="410d0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="410d0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="410d0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="410d0-128">Response</span></span>

<span data-ttu-id="410d0-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="410d0-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="410d0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="410d0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="410d0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="410d0-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="410d0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="410d0-132">Response</span></span>
<span data-ttu-id="410d0-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="410d0-133">The following is an example of the response.</span></span>

<span data-ttu-id="410d0-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="410d0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "value":{
      "@odata.type":"#microsoft.graph.fido2AuthenticationMethodConfiguration",
      "id":"Fido2",
      "state":"enabled",
      "isSelfServiceRegistrationAllowed":true,
      "isAttestationEnforced":true,
      "keyRestrictions":{
         "isEnforced":false,
         "enforcementType":"block",
         "aaGuids":[
            
         ]
      },
      "includeTargets":[
         {
            "targetType":"group",
            "id":"all_users",
            "isRegistrationRequired":false,
            "useForSignIn":true
         }
      ]
   }
}
```

