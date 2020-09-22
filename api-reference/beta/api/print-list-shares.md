---
title: Получение общих папок
description: Получение списка общих принтеров.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 80da97475b6d8f79107034b441a06e58de9dc806
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022264"
---
# <a name="list-shares"></a><span data-ttu-id="2ce52-103">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="2ce52-103">List shares</span></span>

<span data-ttu-id="2ce52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ce52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ce52-105">Получение списка **принтершарес**.</span><span class="sxs-lookup"><span data-stu-id="2ce52-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ce52-106">Permissions</span></span>
<span data-ttu-id="2ce52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2ce52-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2ce52-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="2ce52-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ce52-110">Permission type</span></span> | <span data-ttu-id="2ce52-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ce52-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2ce52-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ce52-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2ce52-113">Принтершаре. Read. ALL, Принтершаре. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2ce52-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="2ce52-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ce52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce52-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ce52-115">Not Supported.</span></span>|
|<span data-ttu-id="2ce52-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ce52-116">Application</span></span>|<span data-ttu-id="2ce52-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ce52-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce52-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ce52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ce52-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ce52-119">Optional query parameters</span></span>
<span data-ttu-id="2ce52-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2ce52-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ce52-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ce52-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="2ce52-122">Чтобы просмотреть список всех возможностей общего доступа к принтерам, включите необязательный `$select=capabilities` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce52-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="2ce52-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="2ce52-123">Exceptions</span></span>
<span data-ttu-id="2ce52-124">Некоторые операторы не поддерживаются: `$count` , `$orderby` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="2ce52-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ce52-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ce52-125">Request headers</span></span>
| <span data-ttu-id="2ce52-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2ce52-126">Name</span></span>      |<span data-ttu-id="2ce52-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce52-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ce52-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ce52-128">Authorization</span></span> | <span data-ttu-id="2ce52-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ce52-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ce52-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ce52-131">Request body</span></span>
<span data-ttu-id="2ce52-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ce52-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2ce52-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ce52-133">Response</span></span>
<span data-ttu-id="2ce52-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ce52-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ce52-135">Пример</span><span class="sxs-lookup"><span data-stu-id="2ce52-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ce52-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ce52-136">Request</span></span>
<span data-ttu-id="2ce52-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce52-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ce52-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ce52-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="2ce52-139">C#</span><span class="sxs-lookup"><span data-stu-id="2ce52-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ce52-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ce52-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ce52-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ce52-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2ce52-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ce52-142">Response</span></span>
<span data-ttu-id="2ce52-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ce52-143">The following is an example of the response.</span></span>
><span data-ttu-id="2ce52-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ce52-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterShareName",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List shares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


