---
title: Список Тасктригжерс
description: Получение списка триггеров задач, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1278e84070bc78c6fb0ead350bd464e8a102ea98
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091714"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="60f29-103">Список Тасктригжерс</span><span class="sxs-lookup"><span data-stu-id="60f29-103">List taskTriggers</span></span>

<span data-ttu-id="60f29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60f29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60f29-105">Получение списка [триггеров задач](../resources/printtasktrigger.md) , связанных с [принтером](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="60f29-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="60f29-106">Список триггеров задач определяет, какие задачи будут вызываться в результате событий, происходящих во время печати.</span><span class="sxs-lookup"><span data-stu-id="60f29-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="60f29-107">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="60f29-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="60f29-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60f29-108">Permissions</span></span>
<span data-ttu-id="60f29-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="60f29-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="60f29-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60f29-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="60f29-111">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="60f29-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="60f29-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60f29-112">Permission type</span></span> | <span data-ttu-id="60f29-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60f29-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="60f29-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60f29-114">Delegated (work or school account)</span></span>| <span data-ttu-id="60f29-115">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="60f29-115">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="60f29-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60f29-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60f29-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60f29-117">Not Supported.</span></span>|
|<span data-ttu-id="60f29-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60f29-118">Application</span></span>| <span data-ttu-id="60f29-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60f29-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60f29-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60f29-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60f29-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60f29-121">Optional query parameters</span></span>
<span data-ttu-id="60f29-122">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60f29-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="60f29-123">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60f29-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="60f29-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="60f29-124">Exceptions</span></span>
<span data-ttu-id="60f29-125">Некоторые операторы не поддерживаются: `$count` , `$format` , `$search` , `$select` , `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="60f29-125">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60f29-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60f29-126">Request headers</span></span>
| <span data-ttu-id="60f29-127">Имя</span><span class="sxs-lookup"><span data-stu-id="60f29-127">Name</span></span>      |<span data-ttu-id="60f29-128">Описание</span><span class="sxs-lookup"><span data-stu-id="60f29-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60f29-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60f29-129">Authorization</span></span> | <span data-ttu-id="60f29-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="60f29-130">Bearer {token}.</span></span> <span data-ttu-id="60f29-131">Required.</span><span class="sxs-lookup"><span data-stu-id="60f29-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60f29-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60f29-132">Request body</span></span>
<span data-ttu-id="60f29-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60f29-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="60f29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="60f29-134">Response</span></span>
<span data-ttu-id="60f29-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принттасктригжер](../resources/printtasktrigger.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60f29-135">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60f29-136">Пример</span><span class="sxs-lookup"><span data-stu-id="60f29-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="60f29-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="60f29-137">Request</span></span>
<span data-ttu-id="60f29-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60f29-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```

---

### <a name="response"></a><span data-ttu-id="60f29-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="60f29-139">Response</span></span>
<span data-ttu-id="60f29-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60f29-140">The following is an example of the response.</span></span>
><span data-ttu-id="60f29-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="60f29-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60f29-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="60f29-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskTriggers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
