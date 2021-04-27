---
title: Вывод задачи
description: Сведения о задаче печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 06e83c3ca75c0e0e0f2a7fda730456388a43d7bb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053596"
---
# <a name="get-task"></a><span data-ttu-id="5e548-103">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="5e548-103">Get task</span></span>

<span data-ttu-id="5e548-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e548-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e548-105">Сведения о задаче печати.</span><span class="sxs-lookup"><span data-stu-id="5e548-105">Get details about a print task.</span></span>

<span data-ttu-id="5e548-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="5e548-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e548-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e548-107">Permissions</span></span>
<span data-ttu-id="5e548-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5e548-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="5e548-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5e548-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e548-111">Permission type</span></span> | <span data-ttu-id="5e548-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e548-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5e548-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e548-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5e548-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e548-114">Not supported.</span></span> |
|<span data-ttu-id="5e548-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e548-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e548-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e548-116">Not Supported.</span></span>|
|<span data-ttu-id="5e548-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5e548-117">Application</span></span>| <span data-ttu-id="5e548-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e548-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e548-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e548-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e548-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e548-120">Request headers</span></span>
| <span data-ttu-id="5e548-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5e548-121">Name</span></span>      |<span data-ttu-id="5e548-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5e548-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e548-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e548-123">Authorization</span></span> | <span data-ttu-id="5e548-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e548-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e548-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e548-126">Request body</span></span>
<span data-ttu-id="5e548-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e548-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5e548-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e548-128">Response</span></span>
<span data-ttu-id="5e548-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printTask](../resources/printtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5e548-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e548-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5e548-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e548-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e548-131">Request</span></span>
<span data-ttu-id="5e548-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e548-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5e548-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e548-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_task"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3
```
# <a name="c"></a>[<span data-ttu-id="5e548-134">C#</span><span class="sxs-lookup"><span data-stu-id="5e548-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e548-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e548-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e548-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e548-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e548-137">Java</span><span class="sxs-lookup"><span data-stu-id="5e548-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="5e548-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e548-138">Response</span></span>
<span data-ttu-id="5e548-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5e548-139">The following is an example of the response.</span></span>
><span data-ttu-id="5e548-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5e548-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 392

{

  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions('3203656e-6069-4e10-8147-d25290b00a3c')/tasks/$entity",
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


