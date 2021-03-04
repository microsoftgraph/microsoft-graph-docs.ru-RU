---
title: Get userFlowApiConnectorConfiguration
description: Получите свойство userFlowApiConnectorConfiguration b2xIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 937e102e05b4b7e2a1b03538a0b023ae583ef3c6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438143"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="c50e9-103">Get userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="c50e9-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="c50e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c50e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c50e9-105">Получите свойство [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [потоке b2xIdentityUserFlow,](../resources/userFlowApiConnectorConfiguration.md) чтобы подробно уобразить соединители API, включенные для потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="c50e9-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="c50e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c50e9-106">Permissions</span></span>

<span data-ttu-id="c50e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c50e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c50e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c50e9-109">Permission type</span></span>      | <span data-ttu-id="c50e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c50e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c50e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c50e9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c50e9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c50e9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c50e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c50e9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c50e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c50e9-114">Not supported.</span></span>|
|<span data-ttu-id="c50e9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c50e9-115">Application</span></span>|<span data-ttu-id="c50e9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c50e9-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c50e9-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c50e9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c50e9-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c50e9-118">Global administrator</span></span>
* <span data-ttu-id="c50e9-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="c50e9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c50e9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c50e9-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c50e9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c50e9-121">Optional query parameters</span></span>

<span data-ttu-id="c50e9-122">Этот метод поддерживает параметр `$expand` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c50e9-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="c50e9-123">Например, чтобы получить соединителю API для действий `postFederationSignup` и `postAttributeCollection` действий, добавьте `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="c50e9-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="c50e9-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c50e9-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c50e9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c50e9-125">Request headers</span></span>

|<span data-ttu-id="c50e9-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c50e9-126">Name</span></span>|<span data-ttu-id="c50e9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c50e9-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c50e9-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c50e9-128">Authorization</span></span>|<span data-ttu-id="c50e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c50e9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c50e9-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c50e9-131">Request body</span></span>

<span data-ttu-id="c50e9-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c50e9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c50e9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c50e9-133">Response</span></span>

<span data-ttu-id="c50e9-134">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект apiConnectorConfiguration.](../resources/userflowapiconnectorconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c50e9-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="c50e9-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="c50e9-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c50e9-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c50e9-136">Request</span></span>

<span data-ttu-id="c50e9-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c50e9-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c50e9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c50e9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```
# <a name="c"></a>[<span data-ttu-id="c50e9-139">C#</span><span class="sxs-lookup"><span data-stu-id="c50e9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-apiconnectorconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c50e9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c50e9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-apiconnectorconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c50e9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c50e9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-apiconnectorconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c50e9-142">Java</span><span class="sxs-lookup"><span data-stu-id="c50e9-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-apiconnectorconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c50e9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c50e9-143">Response</span></span>

<span data-ttu-id="c50e9-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c50e9-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration(postFederationSignup(),postAttributeCollection())",
    "postFederationSignup@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postFederationSignup/$entity",
    "postFederationSignup": {
        "id": "<guid1>",
        "displayName": "Test API Connector 1",
        "targetUrl": "https://someapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
        }
    },
    "postAttributeCollection@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postAttributeCollection/$entity",
    "postAttributeCollection": {
        "id": "<guid2>",
        "displayName": "Test API Connector 2",
        "targetUrl": "https://someotherapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME2>",
            "password": "******"
        }
    }
}
```
