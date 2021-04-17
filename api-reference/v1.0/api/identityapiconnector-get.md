---
title: Get identityApiConnector
description: Ознакомьтесь с свойствами соединитетеля API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 52acb028462d83c6cf555659fbada6234eb90363
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883073"
---
# <a name="get-identityapiconnector"></a><span data-ttu-id="de159-103">Get identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="de159-103">Get identityApiConnector</span></span>

<span data-ttu-id="de159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de159-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de159-105">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="de159-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de159-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de159-106">Permissions</span></span>

<span data-ttu-id="de159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de159-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de159-109">Permission type</span></span>                        | <span data-ttu-id="de159-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de159-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="de159-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de159-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de159-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de159-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="de159-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de159-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de159-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de159-114">Not supported.</span></span>  |
| <span data-ttu-id="de159-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de159-115">Application</span></span>                            | <span data-ttu-id="de159-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de159-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="de159-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="de159-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="de159-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="de159-118">Global administrator</span></span>
* <span data-ttu-id="de159-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="de159-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="de159-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de159-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de159-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="de159-121">Optional query parameters</span></span>

<span data-ttu-id="de159-122">Вы можете использовать `$expand` для расширения определенных свойств, которые не расширяются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="de159-122">You can use `$expand` to expand specific properties that are not expanded by default.</span></span> <span data-ttu-id="de159-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="de159-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="de159-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de159-124">Request headers</span></span>

|<span data-ttu-id="de159-125">Имя</span><span class="sxs-lookup"><span data-stu-id="de159-125">Name</span></span>|<span data-ttu-id="de159-126">Описание</span><span class="sxs-lookup"><span data-stu-id="de159-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de159-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de159-127">Authorization</span></span>|<span data-ttu-id="de159-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de159-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de159-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de159-130">Request body</span></span>

<span data-ttu-id="de159-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de159-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de159-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="de159-132">Response</span></span>

<span data-ttu-id="de159-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de159-133">If successful, this method returns a `200 OK` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de159-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="de159-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de159-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="de159-135">Request</span></span>

<span data-ttu-id="de159-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de159-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityapiconnector"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321
```

### <a name="response"></a><span data-ttu-id="de159-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="de159-137">Response</span></span>

<span data-ttu-id="de159-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de159-138">The following is an example of the response.</span></span>

<span data-ttu-id="de159-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de159-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"370eeb68-dfd3-4a47-8160-8824c2358321",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
