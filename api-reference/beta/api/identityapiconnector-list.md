---
title: Список identityApiConnectors
description: Получить список объектов identityApiConnector и их свойств
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee208f75ce3629ea4217ae992e365578861d9aed
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874314"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="93690-103">Список identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="93690-103">List identityApiConnectors</span></span>

<span data-ttu-id="93690-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93690-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93690-105">Чтение свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="93690-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93690-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93690-106">Permissions</span></span>

<span data-ttu-id="93690-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93690-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93690-109">Permission type</span></span>                        | <span data-ttu-id="93690-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93690-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="93690-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93690-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93690-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93690-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="93690-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93690-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93690-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93690-114">Not supported.</span></span>  |
| <span data-ttu-id="93690-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="93690-115">Application</span></span>                            | <span data-ttu-id="93690-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93690-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="93690-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="93690-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="93690-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="93690-118">Global administrator</span></span>
* <span data-ttu-id="93690-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="93690-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="93690-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93690-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93690-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93690-121">Optional query parameters</span></span>
<span data-ttu-id="93690-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="93690-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="93690-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="93690-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="93690-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93690-124">Request headers</span></span>
|<span data-ttu-id="93690-125">Имя</span><span class="sxs-lookup"><span data-stu-id="93690-125">Name</span></span>|<span data-ttu-id="93690-126">Описание</span><span class="sxs-lookup"><span data-stu-id="93690-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="93690-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93690-127">Authorization</span></span>|<span data-ttu-id="93690-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93690-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93690-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93690-130">Request body</span></span>
<span data-ttu-id="93690-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93690-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93690-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="93690-132">Response</span></span>

<span data-ttu-id="93690-133">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [identityApiConnector](../resources/identityapiconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93690-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93690-134">Пример</span><span class="sxs-lookup"><span data-stu-id="93690-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="93690-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="93690-135">Request</span></span>

<span data-ttu-id="93690-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93690-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93690-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="93690-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[<span data-ttu-id="93690-138">C#</span><span class="sxs-lookup"><span data-stu-id="93690-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93690-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93690-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93690-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93690-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93690-141">Java</span><span class="sxs-lookup"><span data-stu-id="93690-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93690-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="93690-142">Response</span></span>

<span data-ttu-id="93690-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93690-143">The following is an example of the response.</span></span>

<span data-ttu-id="93690-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93690-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "<guid>",
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
