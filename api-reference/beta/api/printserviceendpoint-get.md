---
title: Получение Принтсервицеендпоинт
description: Получение свойств и связей конечной точки службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fbdb6f7748f990fa0c6dc66f63aa4fd15a21f99d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896173"
---
# <a name="get-printserviceendpoint"></a><span data-ttu-id="c03ca-103">Получение Принтсервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="c03ca-103">Get printServiceEndpoint</span></span>

<span data-ttu-id="c03ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c03ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c03ca-105">Получение свойств и связей конечной точки службы печати.</span><span class="sxs-lookup"><span data-stu-id="c03ca-105">Retrieve the properties and relationships of a print service endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="c03ca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c03ca-106">Permissions</span></span>
<span data-ttu-id="c03ca-107">Для вызова этого API не требуется никаких разрешений, но у клиента пользователя должна быть активная универсальная подписка на печать.</span><span class="sxs-lookup"><span data-stu-id="c03ca-107">No permissions are needed to call this API, but the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c03ca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c03ca-108">Permission type</span></span> | <span data-ttu-id="c03ca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c03ca-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c03ca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c03ca-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c03ca-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c03ca-111">None.</span></span>|
|<span data-ttu-id="c03ca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c03ca-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c03ca-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="c03ca-113">None.</span></span>|
|<span data-ttu-id="c03ca-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="c03ca-114">Application</span></span>|<span data-ttu-id="c03ca-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="c03ca-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c03ca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c03ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints/{name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c03ca-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c03ca-117">Optional query parameters</span></span>
<span data-ttu-id="c03ca-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c03ca-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c03ca-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c03ca-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c03ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c03ca-120">Request headers</span></span>
| <span data-ttu-id="c03ca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c03ca-121">Name</span></span>      |<span data-ttu-id="c03ca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c03ca-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c03ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c03ca-123">Authorization</span></span> | <span data-ttu-id="c03ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c03ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c03ca-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c03ca-126">Request body</span></span>
<span data-ttu-id="c03ca-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c03ca-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c03ca-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c03ca-128">Response</span></span>
<span data-ttu-id="c03ca-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтсервицеендпоинт](../resources/printserviceendpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c03ca-129">If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c03ca-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c03ca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c03ca-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c03ca-131">Request</span></span>
<span data-ttu-id="c03ca-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c03ca-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}-->
```http
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints/{name}
```
##### <a name="response"></a><span data-ttu-id="c03ca-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c03ca-133">Response</span></span>
<span data-ttu-id="c03ca-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c03ca-134">The following is an example of the response.</span></span>
><span data-ttu-id="c03ca-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c03ca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "id": "mpsdiscovery",
  "displayName": "Microsoft Universal Print Discovery Service",
  "uri": "https://discovery.print.microsoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printServiceEndpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->