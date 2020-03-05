---
title: Получение объекта signIn
doc_type: apiPageType
description: Получение объекта SignIn, содержащего все входные сведения о клиенте Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 43a8faae65b3994645b7ef273fdacb74888825e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453277"
---
# <a name="get-signin"></a><span data-ttu-id="5cfd0-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="5cfd0-103">Get signIn</span></span>

<span data-ttu-id="5cfd0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5cfd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cfd0-105">Получение объекта [SignIn](../resources/signin.md) , содержащего конкретное пользовательское событие входа для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="5cfd0-106">Сюда входят входы, в которых пользователю предлагается ввести имя пользователя или пароль, а также маркеры сеансов.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cfd0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cfd0-107">Permissions</span></span>

<span data-ttu-id="5cfd0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cfd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cfd0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cfd0-110">Permission type</span></span>      | <span data-ttu-id="5cfd0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cfd0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="5cfd0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cfd0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5cfd0-113">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5cfd0-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="5cfd0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cfd0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cfd0-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5cfd0-115">Not supported</span></span> |
| <span data-ttu-id="5cfd0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cfd0-116">Application</span></span> | <span data-ttu-id="5cfd0-117">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5cfd0-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="5cfd0-118">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="5cfd0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cfd0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cfd0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cfd0-120">Optional query parameters</span></span>

<span data-ttu-id="5cfd0-121">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="5cfd0-122">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="5cfd0-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cfd0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cfd0-123">Request headers</span></span>

| <span data-ttu-id="5cfd0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5cfd0-124">Name</span></span>      |<span data-ttu-id="5cfd0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5cfd0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5cfd0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cfd0-126">Authorization</span></span> | <span data-ttu-id="5cfd0-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5cfd0-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cfd0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cfd0-128">Request body</span></span>

<span data-ttu-id="5cfd0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cfd0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cfd0-130">Response</span></span>

<span data-ttu-id="5cfd0-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [SignIn](../resources/signin.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-131">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5cfd0-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5cfd0-132">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="5cfd0-133">Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-133">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="5cfd0-134">Основной способ проверки подлинности — Фидо.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-134">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="5cfd0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cfd0-135">Request</span></span>

<span data-ttu-id="5cfd0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5cfd0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cfd0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="5cfd0-138">C#</span><span class="sxs-lookup"><span data-stu-id="5cfd0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cfd0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cfd0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cfd0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cfd0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5cfd0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cfd0-141">Response</span></span>

<span data-ttu-id="5cfd0-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-142">The following is an example of the response.</span></span>

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

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="5cfd0-143">Пример 2: пользователь входит только с основной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-143">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="5cfd0-144">Первичная проверка подлинности осуществляется с помощью облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-144">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="5cfd0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cfd0-145">Request</span></span>

<span data-ttu-id="5cfd0-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5cfd0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cfd0-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="5cfd0-148">C#</span><span class="sxs-lookup"><span data-stu-id="5cfd0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cfd0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cfd0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cfd0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cfd0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5cfd0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cfd0-151">Response</span></span>

<span data-ttu-id="5cfd0-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5cfd0-152">The following is an example of the response.</span></span>

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
