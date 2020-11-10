---
title: Получение taskTrigger
description: Получение триггера задачи для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c985552c56caf5a3396a75d54485c67166696b89
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970240"
---
# <a name="get-tasktrigger"></a><span data-ttu-id="fb915-103">Получение taskTrigger</span><span class="sxs-lookup"><span data-stu-id="fb915-103">Get taskTrigger</span></span>

<span data-ttu-id="fb915-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb915-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb915-105">Получение [триггера задачи](../resources/printtasktrigger.md) для [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="fb915-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="fb915-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="fb915-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb915-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb915-107">Permissions</span></span>
<span data-ttu-id="fb915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fb915-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="fb915-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="fb915-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb915-111">Permission type</span></span> | <span data-ttu-id="fb915-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb915-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fb915-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb915-113">Delegated (work or school account)</span></span>| <span data-ttu-id="fb915-114">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="fb915-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="fb915-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb915-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb915-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb915-116">Not Supported.</span></span>|
|<span data-ttu-id="fb915-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fb915-117">Application</span></span>|<span data-ttu-id="fb915-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb915-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb915-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb915-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb915-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb915-120">Request headers</span></span>
| <span data-ttu-id="fb915-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fb915-121">Name</span></span>      |<span data-ttu-id="fb915-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fb915-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fb915-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb915-123">Authorization</span></span> | <span data-ttu-id="fb915-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb915-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb915-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb915-126">Request body</span></span>
<span data-ttu-id="fb915-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb915-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fb915-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb915-128">Response</span></span>
<span data-ttu-id="fb915-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принттасктригжер](../resources/printtasktrigger.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb915-129">If successful, this method returns a `200 OK` response code and [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb915-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb915-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb915-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb915-131">Request</span></span>
<span data-ttu-id="fb915-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb915-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fb915-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb915-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktrigger"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{printerId}/taskTriggers/{taskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="fb915-134">C#</span><span class="sxs-lookup"><span data-stu-id="fb915-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb915-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb915-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb915-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb915-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb915-137">Java</span><span class="sxs-lookup"><span data-stu-id="fb915-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="fb915-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb915-138">Response</span></span>
<span data-ttu-id="fb915-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb915-139">The following is an example of the response.</span></span>
><span data-ttu-id="fb915-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb915-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 181

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


