---
title: Получить проверку подлинностиMethodsPolicy
description: Ознакомьтесь с свойствами и отношениями объекта authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b54b95f3db35d744d400fb50a221cdfdad12890b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682922"
---
# <a name="get-authenticationmethodspolicy"></a><span data-ttu-id="3ffd9-103">Получить проверку подлинностиMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="3ffd9-103">Get authenticationMethodsPolicy</span></span>
<span data-ttu-id="3ffd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ffd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ffd9-105">Ознакомьтесь с свойствами и отношениями объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3ffd9-105">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ffd9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ffd9-106">Permissions</span></span>
<span data-ttu-id="3ffd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ffd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ffd9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ffd9-109">Permission type</span></span>|<span data-ttu-id="3ffd9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ffd9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ffd9-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ffd9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3ffd9-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ffd9-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="3ffd9-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ffd9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ffd9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ffd9-114">Not supported.</span></span>|
|<span data-ttu-id="3ffd9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ffd9-115">Application</span></span>|<span data-ttu-id="3ffd9-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ffd9-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ffd9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ffd9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ffd9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ffd9-118">Optional query parameters</span></span>
<span data-ttu-id="3ffd9-119">Этот метод не поддерживает параметры необязательных запросов.</span><span class="sxs-lookup"><span data-stu-id="3ffd9-119">This method does not support any optional query parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ffd9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ffd9-120">Request headers</span></span>
|<span data-ttu-id="3ffd9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3ffd9-121">Name</span></span>|<span data-ttu-id="3ffd9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ffd9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3ffd9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ffd9-123">Authorization</span></span>|<span data-ttu-id="3ffd9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ffd9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ffd9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ffd9-126">Request body</span></span>
<span data-ttu-id="3ffd9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ffd9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ffd9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ffd9-128">Response</span></span>

<span data-ttu-id="3ffd9-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3ffd9-129">If successful, this method returns a `200 OK` response code and an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ffd9-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ffd9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ffd9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ffd9-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```


### <a name="response"></a><span data-ttu-id="3ffd9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ffd9-132">Response</span></span>
<span data-ttu-id="3ffd9-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3ffd9-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "lastModifiedDateTime": "2021-05-24T18:02:30.5288302Z",
    "policyVersion": "1.4",
    "registrationEnforcement": {
        "authenticationMethodsRegistrationCampaign": {
            "snoozeDurationInDays": 2,
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
