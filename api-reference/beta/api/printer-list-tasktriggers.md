---
title: Перечисление taskTriggers
description: Получение списка триггеров задач, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 189830fb76de676163a24a8166cff6017cceffc5
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565906"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="e3fed-103">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="e3fed-103">List taskTriggers</span></span>

<span data-ttu-id="e3fed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3fed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3fed-105">Получение списка [триггеров задач](../resources/printtasktrigger.md) , связанных с [принтером](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="e3fed-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="e3fed-106">Список триггеров задач определяет, какие задачи будут вызываться в результате событий, происходящих во время печати.</span><span class="sxs-lookup"><span data-stu-id="e3fed-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="e3fed-107">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="e3fed-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3fed-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3fed-108">Permissions</span></span>
<span data-ttu-id="e3fed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3fed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e3fed-111">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="e3fed-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e3fed-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3fed-112">Permission type</span></span> | <span data-ttu-id="e3fed-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3fed-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e3fed-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3fed-114">Delegated (work or school account)</span></span>| <span data-ttu-id="e3fed-115">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="e3fed-115">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="e3fed-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3fed-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3fed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3fed-117">Not Supported.</span></span>|
|<span data-ttu-id="e3fed-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3fed-118">Application</span></span>| <span data-ttu-id="e3fed-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3fed-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3fed-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3fed-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3fed-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3fed-121">Optional query parameters</span></span>
<span data-ttu-id="e3fed-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e3fed-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e3fed-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e3fed-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="e3fed-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e3fed-124">Exceptions</span></span>
<span data-ttu-id="e3fed-125">Некоторые операторы не поддерживаются: `$count` , `$format` , `$search` , `$select` , `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="e3fed-125">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3fed-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3fed-126">Request headers</span></span>
| <span data-ttu-id="e3fed-127">Имя</span><span class="sxs-lookup"><span data-stu-id="e3fed-127">Name</span></span>      |<span data-ttu-id="e3fed-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e3fed-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3fed-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3fed-129">Authorization</span></span> | <span data-ttu-id="e3fed-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3fed-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3fed-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3fed-132">Request body</span></span>
<span data-ttu-id="e3fed-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3fed-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e3fed-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3fed-134">Response</span></span>
<span data-ttu-id="e3fed-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принттасктригжер](../resources/printtasktrigger.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3fed-135">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3fed-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e3fed-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3fed-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3fed-137">Request</span></span>
<span data-ttu-id="e3fed-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3fed-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3fed-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3fed-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="e3fed-140">C#</span><span class="sxs-lookup"><span data-stu-id="e3fed-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3fed-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3fed-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3fed-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3fed-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="e3fed-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3fed-143">Response</span></span>
<span data-ttu-id="e3fed-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3fed-144">The following is an example of the response.</span></span>
><span data-ttu-id="e3fed-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3fed-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
