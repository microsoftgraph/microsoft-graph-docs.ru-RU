---
title: Get userFlowApiConnectorConfiguration
description: Получите свойство userFlowApiConnectorConfiguration объекта b2xIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59d3e7afb85511abca1575c0a8251811c1e84239
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720301"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="60d82-103">Get userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="60d82-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="60d82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60d82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60d82-105">Получите свойство [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [потоке b2xIdentityUserFlow,](../resources/userFlowApiConnectorConfiguration.md) чтобы получить подробные данные о соединителях API, включенных для пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="60d82-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="60d82-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60d82-106">Permissions</span></span>

<span data-ttu-id="60d82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60d82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60d82-109">Permission type</span></span>      | <span data-ttu-id="60d82-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60d82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60d82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60d82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60d82-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d82-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="60d82-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60d82-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="60d82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60d82-114">Not supported.</span></span>|
|<span data-ttu-id="60d82-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="60d82-115">Application</span></span>|<span data-ttu-id="60d82-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d82-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="60d82-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="60d82-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="60d82-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="60d82-118">Global administrator</span></span>
* <span data-ttu-id="60d82-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="60d82-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="60d82-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60d82-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60d82-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60d82-121">Optional query parameters</span></span>

<span data-ttu-id="60d82-122">Этот метод поддерживает параметр `$expand` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60d82-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="60d82-123">Например, чтобы получить соединителю API для этих `postFederationSignup` действий и `postAttributeCollection` действий, добавьте `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="60d82-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="60d82-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60d82-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60d82-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60d82-125">Request headers</span></span>

|<span data-ttu-id="60d82-126">Имя</span><span class="sxs-lookup"><span data-stu-id="60d82-126">Name</span></span>|<span data-ttu-id="60d82-127">Описание</span><span class="sxs-lookup"><span data-stu-id="60d82-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60d82-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60d82-128">Authorization</span></span>|<span data-ttu-id="60d82-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60d82-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d82-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60d82-131">Request body</span></span>

<span data-ttu-id="60d82-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60d82-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60d82-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="60d82-133">Response</span></span>

<span data-ttu-id="60d82-134">В случае успеха этот метод возвращает код отклика и объект `200 OK` [apiConnectorConfiguration.](../resources/userflowapiconnectorconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60d82-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="60d82-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="60d82-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60d82-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="60d82-136">Request</span></span>

<span data-ttu-id="60d82-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60d82-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```

### <a name="response"></a><span data-ttu-id="60d82-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="60d82-138">Response</span></span>

<span data-ttu-id="60d82-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60d82-139">The following is an example of the response.</span></span>

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
