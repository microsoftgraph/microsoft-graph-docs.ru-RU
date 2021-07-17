---
title: Get connectionOperation
description: Ознакомьтесь с свойствами и отношениями объекта connectionOperation.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7a5e5849e91b0d7816ba6b293838eb434e05c900
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467518"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="1494c-103">Get connectionOperation</span><span class="sxs-lookup"><span data-stu-id="1494c-103">Get connectionOperation</span></span>

<span data-ttu-id="1494c-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="1494c-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="1494c-105">Ознакомьтесь с свойствами и отношениями объекта [connectionOperation.](../resources/externalconnectors-connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="1494c-105">Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1494c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1494c-106">Permissions</span></span>
<span data-ttu-id="1494c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1494c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1494c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1494c-109">Permission type</span></span>|<span data-ttu-id="1494c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1494c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1494c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1494c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1494c-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="1494c-112">Not applicable</span></span>|
|<span data-ttu-id="1494c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1494c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1494c-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="1494c-114">Not applicable</span></span>|
|<span data-ttu-id="1494c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1494c-115">Application</span></span>| <span data-ttu-id="1494c-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1494c-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="1494c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1494c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections/{connectionsId}/operations/{connectionOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1494c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1494c-118">Optional query parameters</span></span>
<span data-ttu-id="1494c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1494c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1494c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1494c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1494c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1494c-121">Request headers</span></span>
|<span data-ttu-id="1494c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1494c-122">Name</span></span>|<span data-ttu-id="1494c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1494c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1494c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1494c-124">Authorization</span></span>|<span data-ttu-id="1494c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1494c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1494c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1494c-127">Request body</span></span>
<span data-ttu-id="1494c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1494c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1494c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1494c-129">Response</span></span>

<span data-ttu-id="1494c-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [connectionOperation](../resources/externalconnectors-connectionoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1494c-130">If successful, this method returns a `200 OK` response code and a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1494c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1494c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1494c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1494c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```


### <a name="response"></a><span data-ttu-id="1494c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1494c-133">Response</span></span>
<span data-ttu-id="1494c-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1494c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

