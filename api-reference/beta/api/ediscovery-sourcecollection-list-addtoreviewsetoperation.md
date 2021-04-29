---
title: Список addToReviewSetOperation
description: Получите последний объект addToReviewSetOperation, связанный с исходным собранием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3f10d0da7498863d3cf7c507a2e52a05542f003d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080346"
---
# <a name="list-addtoreviewsetoperation"></a><span data-ttu-id="78020-103">Список addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="78020-103">List addToReviewSetOperation</span></span>

<span data-ttu-id="78020-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="78020-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78020-105">Получите последний [объект addToReviewSetOperation,](../resources/ediscovery-addtoreviewsetoperation.md) связанный с исходным собранием.</span><span class="sxs-lookup"><span data-stu-id="78020-105">Get the last [addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object associated with a source collection.</span></span> 

><span data-ttu-id="78020-106">**Примечание:** В этом методе перечислены только последние операции; он не возвращает историю всех операций.</span><span class="sxs-lookup"><span data-stu-id="78020-106">**Note:** This method only lists the last operation; it does not return a history of all operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="78020-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78020-107">Permissions</span></span>

<span data-ttu-id="78020-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78020-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78020-110">Permission type</span></span>|<span data-ttu-id="78020-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78020-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78020-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78020-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78020-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78020-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="78020-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78020-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78020-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78020-115">Not supported.</span></span>|
|<span data-ttu-id="78020-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78020-116">Application</span></span>|<span data-ttu-id="78020-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78020-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78020-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78020-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/addToReviewSetOperation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78020-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78020-119">Optional query parameters</span></span>

<span data-ttu-id="78020-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="78020-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="78020-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="78020-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="78020-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78020-122">Request headers</span></span>

|<span data-ttu-id="78020-123">Имя</span><span class="sxs-lookup"><span data-stu-id="78020-123">Name</span></span>|<span data-ttu-id="78020-124">Описание</span><span class="sxs-lookup"><span data-stu-id="78020-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="78020-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78020-125">Authorization</span></span>|<span data-ttu-id="78020-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78020-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78020-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78020-128">Request body</span></span>

<span data-ttu-id="78020-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78020-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78020-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="78020-130">Response</span></span>

<span data-ttu-id="78020-131">В случае успеха этот метод возвращает код ответа и `200 OK` [объект microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="78020-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78020-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="78020-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78020-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="78020-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="78020-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="78020-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_addtoreviewsetoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/addToReviewSetOperation
```
# <a name="c"></a>[<span data-ttu-id="78020-135">C#</span><span class="sxs-lookup"><span data-stu-id="78020-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-addtoreviewsetoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78020-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78020-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-addtoreviewsetoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78020-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78020-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-addtoreviewsetoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78020-138">Java</span><span class="sxs-lookup"><span data-stu-id="78020-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-addtoreviewsetoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="78020-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="78020-139">Response</span></span>

> <span data-ttu-id="78020-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="78020-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
