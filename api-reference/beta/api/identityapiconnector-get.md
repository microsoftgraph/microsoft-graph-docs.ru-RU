---
title: Get identityApiConnector
description: Ознакомьтесь с свойствами соединитетеля API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3dbf991dc10d1f7d13c25b7b4e7b4c9d26505045
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435604"
---
# <a name="get-identityapiconnector"></a><span data-ttu-id="950e3-103">Get identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="950e3-103">Get identityApiConnector</span></span>

<span data-ttu-id="950e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="950e3-105">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="950e3-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="950e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="950e3-106">Permissions</span></span>

<span data-ttu-id="950e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="950e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="950e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="950e3-109">Permission type</span></span>                        | <span data-ttu-id="950e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="950e3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="950e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="950e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="950e3-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950e3-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="950e3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="950e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="950e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950e3-114">Not supported.</span></span>  |
| <span data-ttu-id="950e3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="950e3-115">Application</span></span>                            | <span data-ttu-id="950e3-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950e3-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="950e3-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="950e3-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="950e3-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="950e3-118">Global administrator</span></span>
* <span data-ttu-id="950e3-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="950e3-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="950e3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="950e3-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="950e3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="950e3-121">Optional query parameters</span></span>
<span data-ttu-id="950e3-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="950e3-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="950e3-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="950e3-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="950e3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="950e3-124">Request headers</span></span>
|<span data-ttu-id="950e3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="950e3-125">Name</span></span>|<span data-ttu-id="950e3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="950e3-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="950e3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="950e3-127">Authorization</span></span>|<span data-ttu-id="950e3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="950e3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="950e3-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="950e3-130">Request body</span></span>
<span data-ttu-id="950e3-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="950e3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="950e3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="950e3-132">Response</span></span>

<span data-ttu-id="950e3-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="950e3-133">If successful, this method returns a `200 OK` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="950e3-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="950e3-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="950e3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="950e3-135">Request</span></span>

<span data-ttu-id="950e3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="950e3-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="950e3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="950e3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityapiconnector"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="950e3-138">C#</span><span class="sxs-lookup"><span data-stu-id="950e3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="950e3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="950e3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="950e3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="950e3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="950e3-141">Java</span><span class="sxs-lookup"><span data-stu-id="950e3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="950e3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="950e3-142">Response</span></span>

<span data-ttu-id="950e3-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="950e3-143">The following is an example of the response.</span></span>

<span data-ttu-id="950e3-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="950e3-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
