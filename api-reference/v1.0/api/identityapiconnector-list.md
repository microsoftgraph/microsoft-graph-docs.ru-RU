---
title: List identityApiConnectors
description: Получите список объектов identityApiConnector и их свойств.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0417726431261cd25fdc9ee5b58f7fbee8c9d7cd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883062"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="d25c7-103">List identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="d25c7-103">List identityApiConnectors</span></span>

<span data-ttu-id="d25c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d25c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d25c7-105">Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="d25c7-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d25c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d25c7-106">Permissions</span></span>

<span data-ttu-id="d25c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d25c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d25c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d25c7-109">Permission type</span></span>                        | <span data-ttu-id="d25c7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d25c7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d25c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d25c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d25c7-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25c7-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="d25c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d25c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d25c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d25c7-114">Not supported.</span></span>  |
| <span data-ttu-id="d25c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d25c7-115">Application</span></span>                            | <span data-ttu-id="d25c7-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25c7-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="d25c7-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d25c7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d25c7-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d25c7-118">Global administrator</span></span>
* <span data-ttu-id="d25c7-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="d25c7-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d25c7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d25c7-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d25c7-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d25c7-121">Optional query parameters</span></span>

<span data-ttu-id="d25c7-122">Вы можете использовать `$expand` для расширения определенных свойств, которые не расширяются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d25c7-122">You can use `$expand` to expand specific properties that are not expanded by default.</span></span> <span data-ttu-id="d25c7-123">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d25c7-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d25c7-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d25c7-124">Request headers</span></span>

|<span data-ttu-id="d25c7-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d25c7-125">Name</span></span>|<span data-ttu-id="d25c7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d25c7-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d25c7-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d25c7-127">Authorization</span></span>|<span data-ttu-id="d25c7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d25c7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d25c7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d25c7-130">Request body</span></span>

<span data-ttu-id="d25c7-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d25c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d25c7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d25c7-132">Response</span></span>

<span data-ttu-id="d25c7-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d25c7-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d25c7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d25c7-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d25c7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d25c7-135">Request</span></span>

<span data-ttu-id="d25c7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d25c7-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/apiConnectors
```

### <a name="response"></a><span data-ttu-id="d25c7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d25c7-137">Response</span></span>

<span data-ttu-id="d25c7-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d25c7-138">The following is an example of the response.</span></span>

<span data-ttu-id="d25c7-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d25c7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "be1f769b-9b13-437e-b540-79a905c4932c",
          "displayName": "Test API",
          "targetUrl": "https://someapi.com/api/endpoint",
          "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
          }
      }
   ]
}
```
