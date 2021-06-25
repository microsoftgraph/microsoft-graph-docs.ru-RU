---
title: Получение объекта signIn
doc_type: apiPageType
description: Получите объект signIn, содержащий все входы для Azure Active Directory клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: d9cf2f0e6a03a490c1818712bf230120ff37311f
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129493"
---
# <a name="get-signin"></a><span data-ttu-id="5ea4e-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="5ea4e-103">Get signIn</span></span>

<span data-ttu-id="5ea4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ea4e-105">Получите [объект signIn,](../resources/signin.md) содержащий определенное событие для регистрации пользователя для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="5ea4e-106">Это включает входы, в которых пользователю будет предложено ввести имя пользователя или пароль, а также маркеры сеанса.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea4e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea4e-107">Permissions</span></span>

<span data-ttu-id="5ea4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea4e-110">Permission type</span></span>      | <span data-ttu-id="5ea4e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ea4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="5ea4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ea4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea4e-113">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ea4e-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="5ea4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ea4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea4e-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5ea4e-115">Not supported</span></span> |
| <span data-ttu-id="5ea4e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ea4e-116">Application</span></span> | <span data-ttu-id="5ea4e-117">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ea4e-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="5ea4e-118">Приложения должны быть [правильно зарегистрированы в](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-118">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="5ea4e-119">Помимо делегирования разрешений, пользователю, входиму в который, необходимо принадлежать к одной из следующих ролей каталога, которая позволяет ему читать отчеты о входе.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-119">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="5ea4e-120">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="5ea4e-120">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="5ea4e-121">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5ea4e-121">Global Administrator</span></span>
+ <span data-ttu-id="5ea4e-122">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="5ea4e-122">Global Reader</span></span>
+ <span data-ttu-id="5ea4e-123">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="5ea4e-123">Reports Reader</span></span>
+ <span data-ttu-id="5ea4e-124">"Администратор безопасности"</span><span class="sxs-lookup"><span data-stu-id="5ea4e-124">Security Administrator</span></span>
+ <span data-ttu-id="5ea4e-125">Оператор безопасности</span><span class="sxs-lookup"><span data-stu-id="5ea4e-125">Security Operator</span></span>
+ <span data-ttu-id="5ea4e-126">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="5ea4e-126">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="5ea4e-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ea4e-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ea4e-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ea4e-128">Optional query parameters</span></span>

<span data-ttu-id="5ea4e-129">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-129">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ea4e-130">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="5ea4e-130">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ea4e-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ea4e-131">Request headers</span></span>

| <span data-ttu-id="5ea4e-132">Имя</span><span class="sxs-lookup"><span data-stu-id="5ea4e-132">Name</span></span>      |<span data-ttu-id="5ea4e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5ea4e-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ea4e-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ea4e-134">Authorization</span></span> | <span data-ttu-id="5ea4e-135">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5ea4e-135">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ea4e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ea4e-136">Request body</span></span>

<span data-ttu-id="5ea4e-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ea4e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea4e-138">Response</span></span>

<span data-ttu-id="5ea4e-139">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект signIn](../resources/signin.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-139">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea4e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="5ea4e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ea4e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ea4e-141">Request</span></span>

<span data-ttu-id="5ea4e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ea4e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea4e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[<span data-ttu-id="5ea4e-144">C#</span><span class="sxs-lookup"><span data-stu-id="5ea4e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ea4e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ea4e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ea4e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ea4e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ea4e-147">Java</span><span class="sxs-lookup"><span data-stu-id="5ea4e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ea4e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea4e-148">Response</span></span>

<span data-ttu-id="5ea4e-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-149">The following is an example of the response.</span></span>
><span data-ttu-id="5ea4e-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5ea4e-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "authenticationStepDateTime": "2018-11-06T18:48:03.8313489Z",
      "authenticationMethod": "FIDO2",
      "authenticationMethodDetail": "1G54395783",
      "succeeded": true,
      "authenticationStepResultDetail": "methodSucceeded",
      "authenticationStepRequirement": "Primary authentication"
    },
    {
      "authenticationStepDateTime": "2018-11-06T18:48:12.94725647Z",
      "authenticationMethod": "Claim in access token",
      "authenticationMethodDetail": null,
      "succeeded": true,
      "authenticationStepResultDetail": "methodSucceeded",
      "authenticationStepRequirement": "MFA"
    }
  ],
  "authenticationRequirementPolicies": []
}
```
