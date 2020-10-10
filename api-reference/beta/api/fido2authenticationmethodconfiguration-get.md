---
title: Получение fido2AuthenticationMethodConfiguration
description: Чтение свойств и связей объекта fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5411f9c76b6870eccdb43863b5a62380d7caafa3
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418427"
---
# <a name="get-fido2authenticationmethodconfiguration"></a><span data-ttu-id="0ab6e-103">Получение fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ab6e-103">Get fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="0ab6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ab6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ab6e-105">Получение свойств и связей объекта [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) , который представляет [политику метода проверки подлинности](../resources/authenticationmethodspolicies-overview.md) FIDO2 с ключами безопасности для клиента Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0ab6e-105">Retrieve the properties and relationships of the [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ab6e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ab6e-106">Permissions</span></span>
<span data-ttu-id="0ab6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ab6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab6e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ab6e-109">Permission type</span></span>|<span data-ttu-id="0ab6e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ab6e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ab6e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ab6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ab6e-112">Policy. ReadWrite. AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ab6e-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="0ab6e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ab6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ab6e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-114">Not supported.</span></span>|
|<span data-ttu-id="0ab6e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ab6e-115">Application</span></span>|<span data-ttu-id="0ab6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-116">Not supported.</span></span>|

<span data-ttu-id="0ab6e-117">Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="0ab6e-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0ab6e-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0ab6e-118">Global admin</span></span>
* <span data-ttu-id="0ab6e-119">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="0ab6e-119">Global reader</span></span>
* <span data-ttu-id="0ab6e-120">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0ab6e-120">Privileged authentication admin</span></span>
* <span data-ttu-id="0ab6e-121">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0ab6e-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0ab6e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ab6e-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="0ab6e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ab6e-123">Request headers</span></span>
|<span data-ttu-id="0ab6e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0ab6e-124">Name</span></span>|<span data-ttu-id="0ab6e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0ab6e-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ab6e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ab6e-126">Authorization</span></span>|<span data-ttu-id="0ab6e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ab6e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ab6e-129">Request body</span></span>
<span data-ttu-id="0ab6e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ab6e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ab6e-131">Response</span></span>

<span data-ttu-id="0ab6e-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-132">If successful, this method returns a `200 OK` response code and a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ab6e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ab6e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ab6e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ab6e-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="0ab6e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ab6e-135">Response</span></span>
<span data-ttu-id="0ab6e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-136">The following is an example of the response.</span></span>

<span data-ttu-id="0ab6e-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ab6e-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "id": "Fido2",
    "state": "enabled",
    "isSelfServiceRegistrationAllowed": true,
    "isAttestationEnforced": true,
    "keyRestrictions": {
        "isEnforced": false,
        "enforcementType": "block",
        "aaGuids": []
    },
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
  }
}
```

