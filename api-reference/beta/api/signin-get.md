---
title: Получение объекта signIn
doc_type: apiPageType
description: Получение объекта SignIn, содержащего все входные сведения о клиенте Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed96154c2104dc0b06ee24f01080203a8bb61b15
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938374"
---
# <a name="get-signin"></a><span data-ttu-id="6ff3c-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="6ff3c-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ff3c-104">Получение объекта [SignIn](../resources/signin.md) , содержащего конкретное пользовательское событие входа для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-104">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="6ff3c-105">Сюда входят входы, в которых пользователю предлагается ввести имя пользователя или пароль, а также маркеры сеансов.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-105">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ff3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ff3c-106">Permissions</span></span>

<span data-ttu-id="6ff3c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ff3c-109">Permission type</span></span>      | <span data-ttu-id="6ff3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ff3c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="6ff3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ff3c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ff3c-112">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6ff3c-112">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="6ff3c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ff3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ff3c-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6ff3c-114">Not supported</span></span> |
| <span data-ttu-id="6ff3c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ff3c-115">Application</span></span> | <span data-ttu-id="6ff3c-116">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6ff3c-116">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="6ff3c-117">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="6ff3c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ff3c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ff3c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ff3c-119">Optional query parameters</span></span>

<span data-ttu-id="6ff3c-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="6ff3c-121">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="6ff3c-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ff3c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ff3c-122">Request headers</span></span>

| <span data-ttu-id="6ff3c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6ff3c-123">Name</span></span>      |<span data-ttu-id="6ff3c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6ff3c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ff3c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ff3c-125">Authorization</span></span> | <span data-ttu-id="6ff3c-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6ff3c-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ff3c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ff3c-127">Request body</span></span>

<span data-ttu-id="6ff3c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ff3c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff3c-129">Response</span></span>

<span data-ttu-id="6ff3c-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [SignIn](../resources/signin.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-130">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ff3c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ff3c-131">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="6ff3c-132">Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-132">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="6ff3c-133">Основной способ проверки подлинности — Фидо.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-133">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="6ff3c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ff3c-134">Request</span></span>

<span data-ttu-id="6ff3c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6ff3c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ff3c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ff3c-137">C#</span><span class="sxs-lookup"><span data-stu-id="6ff3c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ff3c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ff3c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ff3c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ff3c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6ff3c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff3c-140">Response</span></span>

<span data-ttu-id="6ff3c-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-141">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
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
          "result":"applied"
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

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="6ff3c-142">Пример 2: пользователь входит только с основной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-142">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="6ff3c-143">Первичная проверка подлинности осуществляется с помощью облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-143">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="6ff3c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ff3c-144">Request</span></span>

<span data-ttu-id="6ff3c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

#### <a name="response"></a><span data-ttu-id="6ff3c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ff3c-146">Response</span></span>

<span data-ttu-id="6ff3c-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-147">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
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
