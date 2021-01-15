---
title: Get fido2AuthenticationMethodConfiguration
description: Чтение свойств и связей объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 19e751bab6f076f7269ca895abc35f40a1160423
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872998"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="1ca9e-103">Get fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ca9e-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="1ca9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ca9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca9e-105">Извлечение свойств и связей объекта [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) который представляет [](../resources/authenticationmethodspolicies-overview.md) политику метода проверки подлинности клавиш безопасности FIDO2 для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1ca9e-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ca9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca9e-106">Permissions</span></span>
<span data-ttu-id="1ca9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ca9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca9e-109">Permission type</span></span>|<span data-ttu-id="1ca9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ca9e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ca9e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ca9e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ca9e-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1ca9e-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1ca9e-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ca9e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ca9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-114">Not supported.</span></span>|
|<span data-ttu-id="1ca9e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ca9e-115">Application</span></span>|<span data-ttu-id="1ca9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-116">Not supported.</span></span>|

<span data-ttu-id="1ca9e-117">Для делегирования сценариев администратору требуется следующая [роль:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1ca9e-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1ca9e-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1ca9e-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="1ca9e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ca9e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="1ca9e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ca9e-120">Request headers</span></span>
|<span data-ttu-id="1ca9e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1ca9e-121">Name</span></span>|<span data-ttu-id="1ca9e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca9e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1ca9e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ca9e-123">Authorization</span></span>|<span data-ttu-id="1ca9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ca9e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ca9e-126">Request body</span></span>
<span data-ttu-id="1ca9e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ca9e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca9e-128">Response</span></span>

<span data-ttu-id="1ca9e-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-129">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ca9e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ca9e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ca9e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ca9e-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="1ca9e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca9e-132">Response</span></span>
<span data-ttu-id="1ca9e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-133">The following is an example of the response.</span></span>

<span data-ttu-id="1ca9e-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ca9e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

