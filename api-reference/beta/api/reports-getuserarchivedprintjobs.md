---
title: 'отчеты: getUserArchivedPrintJobs'
description: Получите список архивных заданий печати для конкретного пользователя.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3a1ed3c1e1965d88db9ab7fd9493c9c747f6b6df
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869579"
---
# <a name="reports-getuserarchivedprintjobs"></a><span data-ttu-id="c2577-103">отчеты: getUserArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="c2577-103">reports: getUserArchivedPrintJobs</span></span>

<span data-ttu-id="c2577-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2577-105">Получите список архивных заданий печати для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2577-105">Get a list of archived print jobs for a particular user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2577-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2577-106">Permissions</span></span>
<span data-ttu-id="c2577-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c2577-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c2577-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c2577-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2577-110">Permission type</span></span> | <span data-ttu-id="c2577-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2577-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c2577-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2577-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c2577-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2577-113">Reports.Read.All</span></span> |
|<span data-ttu-id="c2577-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2577-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2577-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2577-115">Not Supported.</span></span>|
|<span data-ttu-id="c2577-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2577-116">Application</span></span>|<span data-ttu-id="c2577-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2577-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2577-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2577-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getUserArchivedPrintJobs(userId=userId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getUserArchivedPrintJobs(userId=userId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="c2577-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2577-119">Request headers</span></span>
| <span data-ttu-id="c2577-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c2577-120">Name</span></span>          | <span data-ttu-id="c2577-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c2577-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2577-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2577-122">Authorization</span></span> | <span data-ttu-id="c2577-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2577-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="c2577-125">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c2577-125">Function Parameters</span></span>

| <span data-ttu-id="c2577-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2577-126">Parameter</span></span>     | <span data-ttu-id="c2577-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c2577-127">Type</span></span>                 | <span data-ttu-id="c2577-128">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="c2577-128">Required?</span></span> | <span data-ttu-id="c2577-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c2577-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | <span data-ttu-id="c2577-130">Да</span><span class="sxs-lookup"><span data-stu-id="c2577-130">Yes</span></span>       | <span data-ttu-id="c2577-131">ID пользователя для возврата данных.</span><span class="sxs-lookup"><span data-stu-id="c2577-131">The ID of the user to return data for.</span></span>                               |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="c2577-132">Нет</span><span class="sxs-lookup"><span data-stu-id="c2577-132">No</span></span>        | <span data-ttu-id="c2577-133">Дата начала (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="c2577-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="c2577-134">Нет</span><span class="sxs-lookup"><span data-stu-id="c2577-134">No</span></span>        | <span data-ttu-id="c2577-135">Дата окончания (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="c2577-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="c2577-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2577-136">Response</span></span>
<span data-ttu-id="c2577-137">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c2577-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2577-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c2577-138">Example</span></span>
<span data-ttu-id="c2577-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c2577-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2577-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2577-140">Request</span></span>
<span data-ttu-id="c2577-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2577-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2577-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2577-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reports-getuserarchivedprintjobs",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/getUserArchivedPrintJobs(userId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)
```
# <a name="c"></a>[<span data-ttu-id="c2577-143">C#</span><span class="sxs-lookup"><span data-stu-id="c2577-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reports-getuserarchivedprintjobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2577-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2577-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reports-getuserarchivedprintjobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2577-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2577-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reports-getuserarchivedprintjobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2577-146">Java</span><span class="sxs-lookup"><span data-stu-id="c2577-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reports-getuserarchivedprintjobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2577-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2577-147">Response</span></span>
<span data-ttu-id="c2577-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2577-148">The following is an example of the response.</span></span>
><span data-ttu-id="c2577-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2577-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 236

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printer": {
        "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6"
      },
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: getUserArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

