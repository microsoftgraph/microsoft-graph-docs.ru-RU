---
title: Получение объекта signIn
description: Извлекает входы пользователей Azure AD для клиента. Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.
localization_priority: Priority
ms.openlocfilehash: 79bebfda40b15a5524aecfc99e5b6d83a168b28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335803"
---
# <a name="get-signin"></a><span data-ttu-id="d2643-104">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="d2643-104">Get signIn</span></span>
<span data-ttu-id="d2643-105">Извлекает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2643-105">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="d2643-106">Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.</span><span class="sxs-lookup"><span data-stu-id="d2643-106">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="d2643-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2643-107">Permissions</span></span>
<span data-ttu-id="d2643-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2643-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2643-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2643-110">Permission type</span></span>      | <span data-ttu-id="d2643-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2643-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2643-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2643-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2643-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2643-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="d2643-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2643-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2643-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d2643-115">Not supported</span></span>   |
|<span data-ttu-id="d2643-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2643-116">Application</span></span> | <span data-ttu-id="d2643-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2643-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="d2643-118">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2643-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2643-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2643-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2643-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2643-120">Optional query parameters</span></span>
<span data-ttu-id="d2643-121">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d2643-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="d2643-122">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="d2643-122">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2643-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2643-123">Request headers</span></span>
| <span data-ttu-id="d2643-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d2643-124">Name</span></span>      |<span data-ttu-id="d2643-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d2643-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2643-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2643-126">Authorization</span></span>  | <span data-ttu-id="d2643-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d2643-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2643-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2643-128">Request body</span></span>
<span data-ttu-id="d2643-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2643-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2643-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2643-130">Response</span></span>
<span data-ttu-id="d2643-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2643-131">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2643-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2643-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2643-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2643-133">Request</span></span>
<span data-ttu-id="d2643-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2643-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
##### <a name="response"></a><span data-ttu-id="d2643-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2643-135">Response</span></span>
<span data-ttu-id="d2643-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2643-136">Here is an example of the response.</span></span> 
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
            "additionalDetails": "SignIn Success & CA Sucess"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v1.0.2016.0",
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
  "tocPath": ""
}-->
