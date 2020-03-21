---
title: Список Монслипринтусажесуммариесбюсер
description: Получение списка ежемесячных сводок использования печати, сгруппированных по пользователям.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0d9246a6206e37600578cc836fe7f476c06e486b
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896137"
---
# <a name="list-monthlyprintusagesummariesbyuser"></a><span data-ttu-id="eaa3b-103">Список Монслипринтусажесуммариесбюсер</span><span class="sxs-lookup"><span data-stu-id="eaa3b-103">List monthlyPrintUsageSummariesByUser</span></span>

<span data-ttu-id="eaa3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaa3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaa3b-105">Получение списка ежемесячных сводок использования печати, сгруппированных по пользователям.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-105">Retrieve a list of monthly print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eaa3b-106">Permissions</span></span>
<span data-ttu-id="eaa3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eaa3b-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="eaa3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaa3b-110">Permission type</span></span> | <span data-ttu-id="eaa3b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaa3b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eaa3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaa3b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="eaa3b-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="eaa3b-113">Users.Read.All</span></span> |
|<span data-ttu-id="eaa3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaa3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaa3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-115">Not Supported.</span></span>|
|<span data-ttu-id="eaa3b-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="eaa3b-116">Application</span></span>|<span data-ttu-id="eaa3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaa3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaa3b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByUser
GET /print/reports/monthlyPrintUsageSummariesByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eaa3b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eaa3b-119">Optional query parameters</span></span>
<span data-ttu-id="eaa3b-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="eaa3b-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eaa3b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eaa3b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaa3b-122">Request headers</span></span>
| <span data-ttu-id="eaa3b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="eaa3b-123">Name</span></span>      |<span data-ttu-id="eaa3b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="eaa3b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eaa3b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eaa3b-125">Authorization</span></span> | <span data-ttu-id="eaa3b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaa3b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eaa3b-128">Request body</span></span>
<span data-ttu-id="eaa3b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eaa3b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaa3b-130">Response</span></span>
<span data-ttu-id="eaa3b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтусажесуммарибюсер](../resources/printusagesummarybyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eaa3b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eaa3b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaa3b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaa3b-133">Request</span></span>
<span data-ttu-id="eaa3b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByUser
```
##### <a name="response"></a><span data-ttu-id="eaa3b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaa3b-135">Response</span></span>
<span data-ttu-id="eaa3b-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-136">The following is an example of the response.</span></span>
><span data-ttu-id="eaa3b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaa3b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 268

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "userPrincipalName": "username@microsoft.com",
      "usageDate": "2020-02-04T00:00:00.0000000Z",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List monthlyPrintUsageSummariesByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->