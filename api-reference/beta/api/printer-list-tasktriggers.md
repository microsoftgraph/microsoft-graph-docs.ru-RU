---
title: Перечисление taskTriggers
description: Извлечение списка триггеров задач, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dbea7cf06139ca976a76a2716f9cba783498f4d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052924"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="c3e6b-103">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="c3e6b-103">List taskTriggers</span></span>

<span data-ttu-id="c3e6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e6b-105">Извлечение списка [триггеров задач,](../resources/printtasktrigger.md) связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c3e6b-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="c3e6b-106">Список триггеров задач определяет, какие задачи будут запускаться в результате событий, которые происходят во время печати.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="c3e6b-107">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="c3e6b-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3e6b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e6b-108">Permissions</span></span>
<span data-ttu-id="c3e6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c3e6b-111">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="c3e6b-112">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c3e6b-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c3e6b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e6b-113">Permission type</span></span> | <span data-ttu-id="c3e6b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3e6b-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c3e6b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3e6b-115">Delegated (work or school account)</span></span>| <span data-ttu-id="c3e6b-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c3e6b-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="c3e6b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3e6b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3e6b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-118">Not Supported.</span></span>|
|<span data-ttu-id="c3e6b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3e6b-119">Application</span></span>| <span data-ttu-id="c3e6b-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3e6b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3e6b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3e6b-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3e6b-122">Optional query parameters</span></span>
<span data-ttu-id="c3e6b-123">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c3e6b-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c3e6b-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="c3e6b-125">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c3e6b-125">Exceptions</span></span>
<span data-ttu-id="c3e6b-126">Некоторые операторы не поддерживаются: `$count` , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="c3e6b-126">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3e6b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3e6b-127">Request headers</span></span>
| <span data-ttu-id="c3e6b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="c3e6b-128">Name</span></span>      |<span data-ttu-id="c3e6b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e6b-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3e6b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3e6b-130">Authorization</span></span> | <span data-ttu-id="c3e6b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3e6b-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3e6b-133">Request body</span></span>
<span data-ttu-id="c3e6b-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c3e6b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e6b-135">Response</span></span>
<span data-ttu-id="c3e6b-136">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов printTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-136">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3e6b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c3e6b-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3e6b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3e6b-138">Request</span></span>
<span data-ttu-id="c3e6b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c3e6b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3e6b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="c3e6b-141">C#</span><span class="sxs-lookup"><span data-stu-id="c3e6b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3e6b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3e6b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3e6b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3e6b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3e6b-144">Java</span><span class="sxs-lookup"><span data-stu-id="c3e6b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-tasktriggers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c3e6b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e6b-145">Response</span></span>
<span data-ttu-id="c3e6b-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-146">The following is an example of the response.</span></span>
><span data-ttu-id="c3e6b-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3e6b-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
