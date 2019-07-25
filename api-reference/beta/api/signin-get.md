---
title: Получение объекта signIn
description: Получение определенного события входа пользователя Azure AD для клиента.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d79d7cbea2f054a5f6670c9de0f8f658507d7247
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869771"
---
# <a name="get-signin"></a><span data-ttu-id="bab5a-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="bab5a-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab5a-104">Получение определенного события входа пользователя Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="bab5a-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="bab5a-105">Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.</span><span class="sxs-lookup"><span data-stu-id="bab5a-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="bab5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bab5a-106">Permissions</span></span>

<span data-ttu-id="bab5a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab5a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bab5a-109">Permission type</span></span>      | <span data-ttu-id="bab5a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bab5a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bab5a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bab5a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bab5a-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab5a-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="bab5a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bab5a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bab5a-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab5a-114">Directory.Read.All</span></span> |
|<span data-ttu-id="bab5a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bab5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab5a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bab5a-116">Not supported</span></span>   |
|<span data-ttu-id="bab5a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bab5a-117">Application</span></span> | <span data-ttu-id="bab5a-118">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab5a-118">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="bab5a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bab5a-119">Application</span></span> | <span data-ttu-id="bab5a-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab5a-120">Directory.Read.All</span></span> | 


<span data-ttu-id="bab5a-121">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bab5a-121">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="bab5a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bab5a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bab5a-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bab5a-123">Optional query parameters</span></span>

<span data-ttu-id="bab5a-124">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bab5a-124">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="bab5a-125">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="bab5a-125">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab5a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bab5a-126">Request headers</span></span>

| <span data-ttu-id="bab5a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="bab5a-127">Name</span></span>      |<span data-ttu-id="bab5a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bab5a-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bab5a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bab5a-129">Authorization</span></span>  | <span data-ttu-id="bab5a-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bab5a-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab5a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bab5a-131">Request body</span></span>

<span data-ttu-id="bab5a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bab5a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab5a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bab5a-133">Response</span></span>

<span data-ttu-id="bab5a-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bab5a-134">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bab5a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bab5a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bab5a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bab5a-136">Request</span></span>

<span data-ttu-id="bab5a-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bab5a-137">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bab5a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bab5a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bab5a-139">C#</span><span class="sxs-lookup"><span data-stu-id="bab5a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bab5a-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="bab5a-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bab5a-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bab5a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bab5a-142">Java</span><span class="sxs-lookup"><span data-stu-id="bab5a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bab5a-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="bab5a-143">Response</span></span>

<span data-ttu-id="bab5a-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bab5a-144">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@contoso.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "ipAddress": "127.0.0.1",
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Success"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "location": {
            "city": "Redmond",
            "state": "WA",
            "countryOrRegion": "USA",
            "geoCoordinates": {
                "altitude": 41.589,
                "latitude": 41.589,
                "longitude": -93.6151
            }
        },
        "mfaDetail": {
            "mfaAuthMethod": "Phone Auth",
            "mfaAuthDetail": null
        },
        "correlationId": "17c47d3c-593d-4d08-ac20-813892b87e42",
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "isRisky": false,
        "riskLevel": "low"
    }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
