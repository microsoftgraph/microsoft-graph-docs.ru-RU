---
title: Получение объекта signIn
description: Описывает метод Get ресурса SignIn (Entity) из API Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d1971a0c0dd85ab07ff7a23204b31c141c130a62
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629728"
---
# <a name="get-signin"></a><span data-ttu-id="fc368-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="fc368-103">Get signIn</span></span>

<span data-ttu-id="fc368-104">Получение определенного события входа пользователя Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc368-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="fc368-105">Интерактивные входы в природе (при условии, что имя пользователя и пароль передаются в составе маркера проверки подлинности); успешные Федеративные входы в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="fc368-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc368-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc368-106">Permissions</span></span>

<span data-ttu-id="fc368-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="fc368-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="fc368-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc368-109">Permission type</span></span>      | <span data-ttu-id="fc368-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc368-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc368-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc368-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc368-112">Аудитлог. Read. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fc368-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="fc368-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc368-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc368-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fc368-114">Not supported</span></span>   |
|<span data-ttu-id="fc368-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc368-115">Application</span></span> | <span data-ttu-id="fc368-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc368-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc368-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc368-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc368-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc368-118">Optional query parameters</span></span>

<span data-ttu-id="fc368-119">Этот метод поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fc368-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="fc368-120">Сведения о том, как использовать эти параметры, представлены в разделе [Параметры запроса OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="fc368-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc368-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc368-121">Request headers</span></span>

| <span data-ttu-id="fc368-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fc368-122">Name</span></span>      |<span data-ttu-id="fc368-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fc368-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc368-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc368-124">Authorization</span></span>  | <span data-ttu-id="fc368-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fc368-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc368-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc368-126">Request body</span></span>

<span data-ttu-id="fc368-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc368-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc368-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc368-128">Response</span></span>

<span data-ttu-id="fc368-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc368-129">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc368-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fc368-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc368-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc368-131">Request</span></span>

<span data-ttu-id="fc368-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc368-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="fc368-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc368-133">Response</span></span>

<span data-ttu-id="fc368-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc368-134">Here is an example of the response.</span></span>
><span data-ttu-id="fc368-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc368-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "id": "id",
    "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
    "appDisplayName": "Azure",
    "createdDateTime": "2018-01-09T21:17:21.5077253Z",
    "clientAppUsed": null,
    "conditionalAccessApplied": true,
    "conditionalAccessPolicies": [{
        "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
        "displayName": "capPolicy",
        "enforcedAccessControls": ["MFA", "TOU"],
        "enforcedSessionControls": ["CloudAppSecurity"],
        "result": "success"
    }],
    "correlationId": "17444d3c-563d-4b08-ac20-815892b87e42",
    "deviceDetail": {
        "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
        "displayName": "DeviceName",
        "operatingSystem": "Windows 10",
        "browser": "Rich Client v3.14.1592.7",
        "isCompliant": true,
        "isManaged": true,
        "trustType": ""
    },
    "ipAddress": "127.0.0.1",
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
    "status": {
        "errorCode": 0,
        "failureReason": null,
        "additionalDetails": "SignIn Success & CA Success"
    },
    "userDisplayName": "Jamie Doe",
    "userPrincipalName": "jdoe@wingtiptoys.com",
    "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302"
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
