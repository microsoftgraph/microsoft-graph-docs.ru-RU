---
title: Список заданий
description: Получение списка заданий печати, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6b290d44801dc1ae234b1eadd6d1fd23426d186c
ms.sourcegitcommit: 9f1e02ab486a2c3e0a128e5d36f46cebe4961581
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2020
ms.locfileid: "45024437"
---
# <a name="list-jobs"></a><span data-ttu-id="80caa-103">Список заданий</span><span class="sxs-lookup"><span data-stu-id="80caa-103">List jobs</span></span>

<span data-ttu-id="80caa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80caa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80caa-105">Получение списка заданий печати, связанных с [принтером](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="80caa-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80caa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80caa-106">Permissions</span></span>
<span data-ttu-id="80caa-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="80caa-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="80caa-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80caa-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="80caa-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать, разрешение, предоставляющее доступ к [принтеру](printer-get.md) , а также одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="80caa-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="80caa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80caa-110">Permission type</span></span> | <span data-ttu-id="80caa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80caa-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="80caa-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80caa-112">Delegated (work or school account)</span></span>| <span data-ttu-id="80caa-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="80caa-113">Users.Read.All</span></span> |
|<span data-ttu-id="80caa-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80caa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80caa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80caa-115">Not Supported.</span></span>|
|<span data-ttu-id="80caa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80caa-116">Application</span></span>| <span data-ttu-id="80caa-117">PrintJob. ReadBasic. ALL, PrintJob. Read. ALL, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="80caa-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80caa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80caa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80caa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="80caa-119">Optional query parameters</span></span>
<span data-ttu-id="80caa-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="80caa-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="80caa-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="80caa-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="80caa-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="80caa-122">Exceptions</span></span>
<span data-ttu-id="80caa-123">Некоторые операторы не поддерживаются: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="80caa-123">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80caa-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80caa-124">Request headers</span></span>
| <span data-ttu-id="80caa-125">Имя</span><span class="sxs-lookup"><span data-stu-id="80caa-125">Name</span></span>      |<span data-ttu-id="80caa-126">Описание</span><span class="sxs-lookup"><span data-stu-id="80caa-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80caa-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80caa-127">Authorization</span></span> | <span data-ttu-id="80caa-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="80caa-128">Bearer {token}.</span></span> <span data-ttu-id="80caa-129">Required.</span><span class="sxs-lookup"><span data-stu-id="80caa-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80caa-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80caa-130">Request body</span></span>
<span data-ttu-id="80caa-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80caa-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="80caa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="80caa-132">Response</span></span>
<span data-ttu-id="80caa-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80caa-133">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80caa-134">Пример</span><span class="sxs-lookup"><span data-stu-id="80caa-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80caa-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="80caa-135">Request</span></span>
<span data-ttu-id="80caa-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80caa-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80caa-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="80caa-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="80caa-138">C#</span><span class="sxs-lookup"><span data-stu-id="80caa-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80caa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80caa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80caa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80caa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80caa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="80caa-141">Response</span></span>
<span data-ttu-id="80caa-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80caa-142">The following is an example of the response.</span></span>
><span data-ttu-id="80caa-143">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="80caa-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80caa-144">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="80caa-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->