---
title: Список externalConnections
description: Получите список объектов externalConnection и их свойств.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 07b0db1eb735999263bc5d2855e7c263351f02e0
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467498"
---
# <a name="list-externalconnections"></a><span data-ttu-id="42097-103">Список externalConnections</span><span class="sxs-lookup"><span data-stu-id="42097-103">List externalConnections</span></span>
<span data-ttu-id="42097-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="42097-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="42097-105">Получите список объектов [externalConnection](../resources/externalconnectors-externalconnection.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="42097-105">Get a list of the [externalConnection](../resources/externalconnectors-externalconnection.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="42097-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42097-106">Permissions</span></span>
<span data-ttu-id="42097-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42097-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42097-109">Permission type</span></span>|<span data-ttu-id="42097-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42097-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42097-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42097-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42097-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="42097-112">Not applicable</span></span>|
|<span data-ttu-id="42097-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42097-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42097-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="42097-114">Not applicable</span></span>|
|<span data-ttu-id="42097-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="42097-115">Application</span></span>| <span data-ttu-id="42097-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="42097-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="42097-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42097-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42097-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42097-118">Optional query parameters</span></span>
<span data-ttu-id="42097-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="42097-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="42097-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="42097-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42097-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42097-121">Request headers</span></span>
|<span data-ttu-id="42097-122">Имя</span><span class="sxs-lookup"><span data-stu-id="42097-122">Name</span></span>|<span data-ttu-id="42097-123">Описание</span><span class="sxs-lookup"><span data-stu-id="42097-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="42097-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42097-124">Authorization</span></span>|<span data-ttu-id="42097-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42097-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42097-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42097-127">Request body</span></span>
<span data-ttu-id="42097-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42097-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42097-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="42097-129">Response</span></span>

<span data-ttu-id="42097-130">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов externalConnection](../resources/externalconnectors-externalconnection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42097-130">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnectors-externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42097-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="42097-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42097-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="42097-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections
```


### <a name="response"></a><span data-ttu-id="42097-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="42097-133">Response</span></span>
<span data-ttu-id="42097-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42097-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.externalConnectors.externalConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    }
  ]
}
```

