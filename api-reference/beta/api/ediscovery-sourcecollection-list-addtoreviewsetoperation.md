---
title: Список addToReviewSetOperation
description: Получите последний объект addToReviewSetOperation, связанный с исходным собранием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c637a0e533d4229766fa293fdd4e372ee5527a41
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446882"
---
# <a name="list-addtoreviewsetoperation"></a><span data-ttu-id="8f860-103">Список addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="8f860-103">List addToReviewSetOperation</span></span>

<span data-ttu-id="8f860-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8f860-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f860-105">Получите последний [объект addToReviewSetOperation,](../resources/ediscovery-addtoreviewsetoperation.md) связанный с исходным собранием.</span><span class="sxs-lookup"><span data-stu-id="8f860-105">Get the last [addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object associated with a source collection.</span></span> 

><span data-ttu-id="8f860-106">**Примечание:** В этом методе перечислены только последние операции; он не возвращает историю всех операций.</span><span class="sxs-lookup"><span data-stu-id="8f860-106">**Note:** This method only lists the last operation; it does not return a history of all operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f860-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f860-107">Permissions</span></span>

<span data-ttu-id="8f860-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f860-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f860-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f860-110">Permission type</span></span>|<span data-ttu-id="8f860-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f860-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f860-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f860-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f860-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f860-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8f860-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f860-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f860-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f860-115">Not supported.</span></span>|
|<span data-ttu-id="8f860-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f860-116">Application</span></span>|<span data-ttu-id="8f860-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f860-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f860-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f860-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/addToReviewSetOperation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f860-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f860-119">Optional query parameters</span></span>

<span data-ttu-id="8f860-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8f860-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8f860-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8f860-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f860-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f860-122">Request headers</span></span>

|<span data-ttu-id="8f860-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8f860-123">Name</span></span>|<span data-ttu-id="8f860-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8f860-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8f860-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f860-125">Authorization</span></span>|<span data-ttu-id="8f860-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f860-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f860-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f860-128">Request body</span></span>

<span data-ttu-id="8f860-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f860-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f860-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f860-130">Response</span></span>

<span data-ttu-id="8f860-131">В случае успеха этот метод возвращает код ответа и `200 OK` [объект microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8f860-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f860-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f860-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f860-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f860-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_addtoreviewsetoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/addToReviewSetOperation
```

### <a name="response"></a><span data-ttu-id="8f860-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f860-134">Response</span></span>

<span data-ttu-id="8f860-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8f860-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.addToReviewSetOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
      "id": "9055c657-c657-9055-57c6-559057c65590",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
