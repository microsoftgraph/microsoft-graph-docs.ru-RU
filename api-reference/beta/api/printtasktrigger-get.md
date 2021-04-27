---
title: Получение taskTrigger
description: Получите триггер задачи с принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3976b61801d6f7bff3a1355666849a8e46f56c70
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053568"
---
# <a name="get-tasktrigger"></a><span data-ttu-id="a45a7-103">Получение taskTrigger</span><span class="sxs-lookup"><span data-stu-id="a45a7-103">Get taskTrigger</span></span>

<span data-ttu-id="a45a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a45a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a45a7-105">Получите [триггер задачи](../resources/printtasktrigger.md) с [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="a45a7-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="a45a7-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="a45a7-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="a45a7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a45a7-107">Permissions</span></span>
<span data-ttu-id="a45a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a45a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a45a7-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="a45a7-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="a45a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a45a7-111">Permission type</span></span> | <span data-ttu-id="a45a7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a45a7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a45a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a45a7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a45a7-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a45a7-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a45a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a45a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a45a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a45a7-116">Not Supported.</span></span>|
|<span data-ttu-id="a45a7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a45a7-117">Application</span></span>|<span data-ttu-id="a45a7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a45a7-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a45a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a45a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a45a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a45a7-120">Request headers</span></span>
| <span data-ttu-id="a45a7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a45a7-121">Name</span></span>      |<span data-ttu-id="a45a7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a45a7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a45a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a45a7-123">Authorization</span></span> | <span data-ttu-id="a45a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a45a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a45a7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a45a7-126">Request body</span></span>
<span data-ttu-id="a45a7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a45a7-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a45a7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a45a7-128">Response</span></span>
<span data-ttu-id="a45a7-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [печать объектаTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a45a7-129">If successful, this method returns a `200 OK` response code and [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a45a7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a45a7-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="a45a7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a45a7-131">Request</span></span>
<span data-ttu-id="a45a7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a45a7-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a45a7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a45a7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktrigger"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{printerId}/taskTriggers/{taskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="a45a7-134">C#</span><span class="sxs-lookup"><span data-stu-id="a45a7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a45a7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a45a7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a45a7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a45a7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a45a7-137">Java</span><span class="sxs-lookup"><span data-stu-id="a45a7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="a45a7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a45a7-138">Response</span></span>
<span data-ttu-id="a45a7-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a45a7-139">The following is an example of the response.</span></span>
><span data-ttu-id="a45a7-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a45a7-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


