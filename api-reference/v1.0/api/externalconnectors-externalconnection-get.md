---
title: Get externalConnection
description: Ознакомьтесь с свойствами и отношениями объекта externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ca5dc2d998cfa327f3c263222583de0c42aaaab4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467437"
---
# <a name="get-externalconnection"></a><span data-ttu-id="2cd1a-103">Get externalConnection</span><span class="sxs-lookup"><span data-stu-id="2cd1a-103">Get externalConnection</span></span>
<span data-ttu-id="2cd1a-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="2cd1a-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="2cd1a-105">Ознакомьтесь с свойствами и отношениями [объекта externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="2cd1a-105">Read the properties and relationships of an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cd1a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cd1a-106">Permissions</span></span>
<span data-ttu-id="2cd1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cd1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cd1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cd1a-109">Permission type</span></span>|<span data-ttu-id="2cd1a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cd1a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cd1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cd1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2cd1a-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="2cd1a-112">Not applicable</span></span>|
|<span data-ttu-id="2cd1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cd1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cd1a-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="2cd1a-114">Not applicable</span></span>|
|<span data-ttu-id="2cd1a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2cd1a-115">Application</span></span>| <span data-ttu-id="2cd1a-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2cd1a-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cd1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cd1a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2cd1a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2cd1a-118">Optional query parameters</span></span>
<span data-ttu-id="2cd1a-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2cd1a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2cd1a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2cd1a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cd1a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cd1a-121">Request headers</span></span>
|<span data-ttu-id="2cd1a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2cd1a-122">Name</span></span>|<span data-ttu-id="2cd1a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2cd1a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2cd1a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cd1a-124">Authorization</span></span>|<span data-ttu-id="2cd1a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cd1a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cd1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cd1a-127">Request body</span></span>
<span data-ttu-id="2cd1a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cd1a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cd1a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cd1a-129">Response</span></span>

<span data-ttu-id="2cd1a-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект externalConnection](../resources/externalconnectors-externalconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2cd1a-130">If successful, this method returns a `200 OK` response code and an [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cd1a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2cd1a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2cd1a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cd1a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr
```


### <a name="response"></a><span data-ttu-id="2cd1a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cd1a-133">Response</span></span>
<span data-ttu-id="2cd1a-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cd1a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```

