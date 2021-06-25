---
title: Перечисление входов
doc_type: apiPageType
description: Получите список входных записей пользователя в Azure Active Directory клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: c85788d7ee1023e8f21097561105d7715f2074cd
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129497"
---
# <a name="list-signins"></a><span data-ttu-id="e8e21-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="e8e21-103">List signIns</span></span>

<span data-ttu-id="e8e21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8e21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8e21-105">Получите список [объектов signIn.](../resources/signin.md)</span><span class="sxs-lookup"><span data-stu-id="e8e21-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="e8e21-106">В списке содержатся входы пользователя для Azure Active Directory клиента.</span><span class="sxs-lookup"><span data-stu-id="e8e21-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="e8e21-107">Входы, в которых имя пользователя и пароль передаются в рамках маркера авторизации, и успешные федераированные входы в настоящее время включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="e8e21-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="e8e21-108">Максимальный и по умолчанию размер страницы — 1000 объектов, и по умолчанию самые последние входы возвращаются первыми.</span><span class="sxs-lookup"><span data-stu-id="e8e21-108">The maximum and default page size is 1,000 objects and by default, the most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e21-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8e21-109">Permissions</span></span>

<span data-ttu-id="e8e21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8e21-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8e21-112">Permission type</span></span> | <span data-ttu-id="e8e21-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8e21-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e8e21-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8e21-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e8e21-115">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8e21-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="e8e21-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8e21-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e21-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e8e21-117">Not supported</span></span> |
| <span data-ttu-id="e8e21-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8e21-118">Application</span></span> | <span data-ttu-id="e8e21-119">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8e21-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="e8e21-120">Приложения должны быть [правильно зарегистрированы в](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e8e21-120">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="e8e21-121">Помимо делегирования разрешений, пользователю, входиму в который, необходимо принадлежать к одной из следующих ролей каталога, которая позволяет ему читать отчеты о входе.</span><span class="sxs-lookup"><span data-stu-id="e8e21-121">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="e8e21-122">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="e8e21-122">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="e8e21-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e8e21-123">Global Administrator</span></span>
+ <span data-ttu-id="e8e21-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="e8e21-124">Global Reader</span></span>
+ <span data-ttu-id="e8e21-125">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="e8e21-125">Reports Reader</span></span>
+ <span data-ttu-id="e8e21-126">"Администратор безопасности"</span><span class="sxs-lookup"><span data-stu-id="e8e21-126">Security Administrator</span></span>
+ <span data-ttu-id="e8e21-127">Оператор безопасности</span><span class="sxs-lookup"><span data-stu-id="e8e21-127">Security Operator</span></span>
+ <span data-ttu-id="e8e21-128">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="e8e21-128">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="e8e21-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8e21-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8e21-130">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e8e21-130">Optional query parameters</span></span>

<span data-ttu-id="e8e21-131">Этот метод поддерживает `$top` параметры `$skiptoken` запроса OData и OData для настройки `$filter` ответа.</span><span class="sxs-lookup"><span data-stu-id="e8e21-131">This method supports the `$top`, `$skiptoken`, and `$filter` OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="e8e21-132">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="e8e21-132">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8e21-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8e21-133">Request headers</span></span>

| <span data-ttu-id="e8e21-134">Имя</span><span class="sxs-lookup"><span data-stu-id="e8e21-134">Name</span></span>      |<span data-ttu-id="e8e21-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e8e21-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8e21-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8e21-136">Authorization</span></span> | <span data-ttu-id="e8e21-137">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e8e21-137">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8e21-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8e21-138">Request body</span></span>

<span data-ttu-id="e8e21-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8e21-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8e21-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e21-140">Response</span></span>

<span data-ttu-id="e8e21-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8e21-141">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="e8e21-142">Коллекция объектов указана в порядке убывания на основе **createdDateTime.**</span><span class="sxs-lookup"><span data-stu-id="e8e21-142">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="e8e21-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8e21-143">Examples</span></span>

### <a name="example-1-list-all-sign-ins"></a><span data-ttu-id="e8e21-144">Пример 1. Список всех входов</span><span class="sxs-lookup"><span data-stu-id="e8e21-144">Example 1: List all sign-ins</span></span>
<span data-ttu-id="e8e21-145">В этом примере объект ответа показывает, как пользователь подписался с помощью MFA, который был вызван политикой условного доступа, а основной метод проверки подлинности — через FIDO.</span><span class="sxs-lookup"><span data-stu-id="e8e21-145">In this example, the response object shows the user signed in using MFA which was triggered by a conditional access policy, and the primary authentication method is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="e8e21-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8e21-146">Request</span></span>

<span data-ttu-id="e8e21-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8e21-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8e21-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e21-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="e8e21-149">C#</span><span class="sxs-lookup"><span data-stu-id="e8e21-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8e21-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8e21-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8e21-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8e21-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8e21-152">Java</span><span class="sxs-lookup"><span data-stu-id="e8e21-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e8e21-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e21-153">Response</span></span>
><span data-ttu-id="e8e21-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8e21-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "authenticationRequirement": "multiFactorAuthentication",
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
      "alternateSignInName": "testaccount2.contoso.com",
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
### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-azure"></a><span data-ttu-id="e8e21-155">Пример 2. Извлечение первых 10 входов в приложения с помощью appDisplayName, которое начинается с "Azure"</span><span class="sxs-lookup"><span data-stu-id="e8e21-155">Example 2: Retrieve the first 10 sign-ins to apps with the appDisplayName that starts with 'Azure'</span></span>

<span data-ttu-id="e8e21-156">В этом примере объект ответа показывает, что пользователь подписался только с помощью основного метода проверки подлинности — облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="e8e21-156">In this example, the response object shows the user signed in using only their primary authentication method—a cloud password.</span></span> <span data-ttu-id="e8e21-157">Ответ включает свойство, содержаное URL-адрес, который можно использовать для получения `@odata.nextLink` следующих 10 результатов.</span><span class="sxs-lookup"><span data-stu-id="e8e21-157">The response includes a `@odata.nextLink` property which contains a URL that can be used to retrieve the next 10 results.</span></span>

#### <a name="request"></a><span data-ttu-id="e8e21-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8e21-158">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signins?&$filter=startsWith(appDisplayName,'Azure')&top=10
```

#### <a name="response"></a><span data-ttu-id="e8e21-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8e21-159">Response</span></span>
><span data-ttu-id="e8e21-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8e21-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "@odata.nextLink": "https://graph.microsoft.com/beta/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Azure%27)&$top=10&$skiptoken=3cff228c89605cc89b0dc753668deef4153e8644caa6d83ed1bb5f711b21cba4",
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
      "ipAddress":"131.107.159.37",
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
      "resourceDisplayName":"Windows Azure Service Management API",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 10",
        "browser":"Chrome 90.0.4430",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
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
