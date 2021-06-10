---
title: Обновление проверки подлинностиMethodsPolicy
description: Обновление свойств объекта authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc9c67d5f01d45b1231d1d92922c45c02b3515f4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869102"
---
# <a name="update-authenticationmethodspolicy"></a><span data-ttu-id="2ff1a-103">Обновление проверки подлинностиMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="2ff1a-103">Update authenticationMethodsPolicy</span></span>
<span data-ttu-id="2ff1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ff1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff1a-105">Обновление свойств объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-105">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ff1a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff1a-106">Permissions</span></span>
<span data-ttu-id="2ff1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ff1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ff1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff1a-109">Permission type</span></span>|<span data-ttu-id="2ff1a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ff1a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ff1a-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ff1a-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="2ff1a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ff1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-114">Not supported.</span></span>|
|<span data-ttu-id="2ff1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ff1a-115">Application</span></span>|<span data-ttu-id="2ff1a-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ff1a-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ff1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ff1a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="2ff1a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ff1a-118">Request headers</span></span>
|<span data-ttu-id="2ff1a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ff1a-119">Name</span></span>|<span data-ttu-id="2ff1a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff1a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ff1a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ff1a-121">Authorization</span></span>|<span data-ttu-id="2ff1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2ff1a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ff1a-124">Content-Type</span></span>|<span data-ttu-id="2ff1a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ff1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ff1a-127">Request body</span></span>
<span data-ttu-id="2ff1a-128">В органе запроса необходимо предоставить представление JSON объекта [registrationEnforcement,](../resources/registrationenforcement.md) чтобы побудить пользователей настроить целевые методы проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-128">In the request body, supply a JSON representation of the [registrationEnforcement](../resources/registrationenforcement.md) object to prompt users to set up targeted authentication methods.</span></span> 

|<span data-ttu-id="2ff1a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ff1a-129">Property</span></span>|<span data-ttu-id="2ff1a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2ff1a-130">Type</span></span>|<span data-ttu-id="2ff1a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff1a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff1a-132">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="2ff1a-132">registrationEnforcement</span></span>|[<span data-ttu-id="2ff1a-133">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="2ff1a-133">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="2ff1a-134">Принудительное выполнение регистрации во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-134">Enforce registration at sign-in time.</span></span> <span data-ttu-id="2ff1a-135">Это свойство можно использовать для того, чтобы побудить пользователей настроить целевые методы проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-135">This property can be used to prompt users to set up targeted authentication methods.</span></span>|

## <a name="response"></a><span data-ttu-id="2ff1a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ff1a-136">Response</span></span>
<span data-ttu-id="2ff1a-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2ff1a-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ff1a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ff1a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ff1a-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ff1a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ff1a-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2ff1a-141">C#</span><span class="sxs-lookup"><span data-stu-id="2ff1a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ff1a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ff1a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ff1a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ff1a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ff1a-144">Java</span><span class="sxs-lookup"><span data-stu-id="2ff1a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2ff1a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ff1a-145">Response</span></span>
<span data-ttu-id="2ff1a-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
