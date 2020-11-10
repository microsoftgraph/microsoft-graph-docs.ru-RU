---
title: Получение объекта signIn
doc_type: apiPageType
description: Получение объекта SignIn, содержащего все входные сведения о клиенте Azure Active Directory.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 15debdb65b2cb5f76c5ca77958b641d3daeb73f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969125"
---
# <a name="get-signin"></a><span data-ttu-id="92b65-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="92b65-103">Get signIn</span></span>

<span data-ttu-id="92b65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92b65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92b65-105">Получение объекта [SignIn](../resources/signin.md) , содержащего конкретное пользовательское событие входа для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="92b65-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="92b65-106">Сюда входят входы, в которых пользователю предлагается ввести имя пользователя или пароль, а также маркеры сеансов.</span><span class="sxs-lookup"><span data-stu-id="92b65-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="92b65-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92b65-107">Permissions</span></span>

<span data-ttu-id="92b65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b65-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92b65-110">Permission type</span></span>      | <span data-ttu-id="92b65-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92b65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="92b65-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92b65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92b65-113">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="92b65-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="92b65-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92b65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92b65-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="92b65-115">Not supported</span></span> |
| <span data-ttu-id="92b65-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="92b65-116">Application</span></span> | <span data-ttu-id="92b65-117">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="92b65-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="92b65-118">Кроме того, приложения должны быть [правильно зарегистрированы](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="92b65-118">In addition, apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="92b65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92b65-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92b65-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92b65-120">Optional query parameters</span></span>

<span data-ttu-id="92b65-121">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="92b65-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="92b65-122">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="92b65-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="92b65-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92b65-123">Request headers</span></span>

| <span data-ttu-id="92b65-124">Имя</span><span class="sxs-lookup"><span data-stu-id="92b65-124">Name</span></span>      |<span data-ttu-id="92b65-125">Описание</span><span class="sxs-lookup"><span data-stu-id="92b65-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92b65-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92b65-126">Authorization</span></span> | <span data-ttu-id="92b65-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="92b65-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="92b65-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92b65-128">Request body</span></span>

<span data-ttu-id="92b65-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92b65-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b65-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b65-130">Response</span></span>

<span data-ttu-id="92b65-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [SignIn](../resources/signin.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92b65-131">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92b65-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="92b65-132">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="92b65-133">Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа.</span><span class="sxs-lookup"><span data-stu-id="92b65-133">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="92b65-134">Основной способ проверки подлинности — Фидо.</span><span class="sxs-lookup"><span data-stu-id="92b65-134">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="92b65-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b65-135">Request</span></span>

<span data-ttu-id="92b65-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b65-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="92b65-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="92b65-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="92b65-138">C#</span><span class="sxs-lookup"><span data-stu-id="92b65-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92b65-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92b65-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92b65-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92b65-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92b65-141">Java</span><span class="sxs-lookup"><span data-stu-id="92b65-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="92b65-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b65-142">Response</span></span>

<span data-ttu-id="92b65-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92b65-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [
        {
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "MultifactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2@contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
            "authenticationDetails": [
                    {
              "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
              "authenticationMethod":"FIDO2",
              "authenticationMethodDetail":"1G54395783",
              "succeeded":true,
              "authenticationStepResultDetail":"methodSucceeded",
              "authenticationStepRequirement":"Primary authentication"
            },
            {
              "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
              "authenticationMethod":"Claim in access token",
              "authenticationMethodDetail":null,
              "succeeded":true,
              "authenticationStepResultDetail":"methodSucceeded",
              "authenticationStepRequirement":"MFA"
            }
            ],
            "authenticationRequirementPolicies": []
        }
    ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="92b65-144">Пример 2: пользователь входит только с основной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="92b65-144">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="92b65-145">Первичная проверка подлинности осуществляется с помощью облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="92b65-145">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="92b65-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b65-146">Request</span></span>

<span data-ttu-id="92b65-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b65-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="92b65-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="92b65-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="92b65-149">C#</span><span class="sxs-lookup"><span data-stu-id="92b65-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92b65-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92b65-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92b65-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92b65-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92b65-152">Java</span><span class="sxs-lookup"><span data-stu-id="92b65-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92b65-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b65-153">Response</span></span>

<span data-ttu-id="92b65-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92b65-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
