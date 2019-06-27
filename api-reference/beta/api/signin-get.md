---
title: Получение объекта signIn
description: Получение определенного события входа пользователя Azure AD для клиента.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13f95b67a76496f7695efb5d7ae11381c9647108
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271640"
---
# <a name="get-signin"></a><span data-ttu-id="edea5-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="edea5-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edea5-104">Получение определенного события входа пользователя Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="edea5-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="edea5-105">Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.</span><span class="sxs-lookup"><span data-stu-id="edea5-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="edea5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edea5-106">Permissions</span></span>

<span data-ttu-id="edea5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edea5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edea5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edea5-109">Permission type</span></span>      | <span data-ttu-id="edea5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edea5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edea5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edea5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="edea5-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="edea5-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="edea5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edea5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edea5-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="edea5-114">Not supported</span></span>   |
|<span data-ttu-id="edea5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edea5-115">Application</span></span> | <span data-ttu-id="edea5-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="edea5-116">AuditLog.Read.All</span></span> | 

<span data-ttu-id="edea5-117">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="edea5-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="edea5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edea5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="edea5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="edea5-119">Optional query parameters</span></span>

<span data-ttu-id="edea5-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="edea5-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="edea5-121">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="edea5-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="edea5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edea5-122">Request headers</span></span>

| <span data-ttu-id="edea5-123">Имя</span><span class="sxs-lookup"><span data-stu-id="edea5-123">Name</span></span>      |<span data-ttu-id="edea5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="edea5-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="edea5-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edea5-125">Authorization</span></span>  | <span data-ttu-id="edea5-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="edea5-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="edea5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edea5-127">Request body</span></span>

<span data-ttu-id="edea5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edea5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edea5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="edea5-129">Response</span></span>

<span data-ttu-id="edea5-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edea5-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edea5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="edea5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="edea5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="edea5-132">Request</span></span>

<span data-ttu-id="edea5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edea5-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="edea5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="edea5-134">Response</span></span>

<span data-ttu-id="edea5-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edea5-135">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="edea5-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="edea5-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="edea5-137">C#</span><span class="sxs-lookup"><span data-stu-id="edea5-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signin-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edea5-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="edea5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signin-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="edea5-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="edea5-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_signin-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
