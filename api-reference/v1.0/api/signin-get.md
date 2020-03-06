---
title: Получение объекта signIn
description: Описывает метод Get ресурса SignIn (Entity) из API Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2687a1aadcd3a39e329b4888f0941e44e44f7968
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509824"
---
# <a name="get-signin"></a><span data-ttu-id="b81cf-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="b81cf-103">Get signIn</span></span>

<span data-ttu-id="b81cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b81cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b81cf-105">Получение определенного события входа пользователя Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="b81cf-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="b81cf-106">Интерактивные входы в природе (при условии, что имя пользователя и пароль передаются в составе маркера проверки подлинности); успешные Федеративные входы в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="b81cf-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="b81cf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b81cf-107">Permissions</span></span>

<span data-ttu-id="b81cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="b81cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="b81cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b81cf-110">Permission type</span></span>      | <span data-ttu-id="b81cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b81cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b81cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b81cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b81cf-113">Аудитлог. Read. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b81cf-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="b81cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b81cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b81cf-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b81cf-115">Not supported</span></span>   |
|<span data-ttu-id="b81cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b81cf-116">Application</span></span> | <span data-ttu-id="b81cf-117">Аудитлог. Read. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b81cf-117">AuditLog.Read.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b81cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b81cf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b81cf-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b81cf-119">Optional query parameters</span></span>

<span data-ttu-id="b81cf-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b81cf-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="b81cf-121">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="b81cf-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b81cf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b81cf-122">Request headers</span></span>

| <span data-ttu-id="b81cf-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b81cf-123">Name</span></span>      |<span data-ttu-id="b81cf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b81cf-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b81cf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b81cf-125">Authorization</span></span>  | <span data-ttu-id="b81cf-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b81cf-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b81cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b81cf-127">Request body</span></span>

<span data-ttu-id="b81cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b81cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b81cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b81cf-129">Response</span></span>

<span data-ttu-id="b81cf-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b81cf-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b81cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b81cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b81cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b81cf-132">Request</span></span>

<span data-ttu-id="b81cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b81cf-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b81cf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b81cf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="b81cf-135">C#</span><span class="sxs-lookup"><span data-stu-id="b81cf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b81cf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b81cf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b81cf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b81cf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b81cf-138">Java</span><span class="sxs-lookup"><span data-stu-id="b81cf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b81cf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b81cf-139">Response</span></span>

<span data-ttu-id="b81cf-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b81cf-140">Here is an example of the response.</span></span>
><span data-ttu-id="b81cf-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b81cf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
