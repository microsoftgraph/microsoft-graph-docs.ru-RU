---
title: Обновление проверки подлинностиMethodsPolicy
description: Обновление свойств объекта authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 22630c6651e94faa243e98f275c6d299edd88173
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682925"
---
# <a name="update-authenticationmethodspolicy"></a><span data-ttu-id="0b19d-103">Обновление проверки подлинностиMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="0b19d-103">Update authenticationMethodsPolicy</span></span>
<span data-ttu-id="0b19d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b19d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b19d-105">Обновление свойств объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b19d-105">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b19d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b19d-106">Permissions</span></span>
<span data-ttu-id="0b19d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b19d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b19d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b19d-109">Permission type</span></span>|<span data-ttu-id="0b19d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b19d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b19d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b19d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b19d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b19d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="0b19d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b19d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b19d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b19d-114">Not supported.</span></span>|
|<span data-ttu-id="0b19d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b19d-115">Application</span></span>|<span data-ttu-id="0b19d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b19d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b19d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b19d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="0b19d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b19d-118">Request headers</span></span>
|<span data-ttu-id="0b19d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b19d-119">Name</span></span>|<span data-ttu-id="0b19d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0b19d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b19d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b19d-121">Authorization</span></span>|<span data-ttu-id="0b19d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b19d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0b19d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b19d-124">Content-Type</span></span>|<span data-ttu-id="0b19d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b19d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b19d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b19d-127">Request body</span></span>
<span data-ttu-id="0b19d-128">В органе запроса необходимо предоставить представление JSON объекта [registrationEnforcement,](../resources/registrationenforcement.md) чтобы побудить пользователей настроить целевые методы проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0b19d-128">In the request body, supply a JSON representation of the [registrationEnforcement](../resources/registrationenforcement.md) object to prompt users to set up targeted authentication methods.</span></span> 

|<span data-ttu-id="0b19d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b19d-129">Property</span></span>|<span data-ttu-id="0b19d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0b19d-130">Type</span></span>|<span data-ttu-id="0b19d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0b19d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b19d-132">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="0b19d-132">registrationEnforcement</span></span>|[<span data-ttu-id="0b19d-133">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="0b19d-133">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="0b19d-134">Принудительное выполнение регистрации во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="0b19d-134">Enforce registration at sign-in time.</span></span> <span data-ttu-id="0b19d-135">Это свойство можно использовать для того, чтобы побудить пользователей настроить целевые методы проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0b19d-135">This property can be used to prompt users to set up targeted authentication methods.</span></span>|

## <a name="response"></a><span data-ttu-id="0b19d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b19d-136">Response</span></span>
<span data-ttu-id="0b19d-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="0b19d-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0b19d-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b19d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b19d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b19d-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodspolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
Content-Type: application/json
Content-length: 293

{
  "registrationEnforcement": {
    "authenticationMethodsRegistrationCampaign": {
        "snoozeDurationInDays": 1,
        "state": "enabled",
        "excludeTargets": [],
        "includeTargets": [
            {
                "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                "targetType": "group",
                "targetedAuthenticationMethod": "microsoftAuthenticator"
            }
        ]
    }
  }
}
```


### <a name="response"></a><span data-ttu-id="0b19d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b19d-140">Response</span></span>
<span data-ttu-id="0b19d-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b19d-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodsPolicy",
  "id": "authenticationMethodsPolicy",
  "displayName": "Authentication Methods Policy",
  "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
  "lastModifiedDateTime": "2021-05-25T01:08:08.6712279Z",
  "policyVersion": "1.4",
  "registrationEnforcement": {
    "authenticationMethodsRegistrationCampaign": {
        "snoozeDurationInDays": 1,
        "state": "enabled",
        "excludeTargets": [],
        "includeTargets": [
            {
                "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                "targetType": "group",
                "targetedAuthenticationMethod": "microsoftAuthenticator"
            }
        ]
    }
  }
}
```
