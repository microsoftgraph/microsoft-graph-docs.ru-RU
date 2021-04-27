---
title: Перечисление задач
description: Извлечение списка задач, связанных с определением задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e489a7a1c34a60d1f1da45d151a50e46511e6ca0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053582"
---
# <a name="list-tasks"></a><span data-ttu-id="7f865-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="7f865-103">List tasks</span></span>

<span data-ttu-id="7f865-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f865-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f865-105">Извлечение списка [задач, связанных](../resources/printtask.md) с [определением задач.](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f865-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="7f865-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="7f865-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f865-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f865-107">Permissions</span></span>
<span data-ttu-id="7f865-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7f865-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="7f865-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="7f865-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f865-111">Permission type</span></span> | <span data-ttu-id="7f865-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f865-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7f865-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f865-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7f865-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f865-114">Not supported.</span></span> |
|<span data-ttu-id="7f865-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f865-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f865-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f865-116">Not Supported.</span></span>|
|<span data-ttu-id="7f865-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f865-117">Application</span></span>| <span data-ttu-id="7f865-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f865-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f865-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f865-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f865-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f865-120">Optional query parameters</span></span>
<span data-ttu-id="7f865-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7f865-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7f865-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7f865-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="7f865-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="7f865-123">Exceptions</span></span>
<span data-ttu-id="7f865-124">Некоторые операторы не поддерживаются: `$count` , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="7f865-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f865-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f865-125">Request headers</span></span>
| <span data-ttu-id="7f865-126">Имя</span><span class="sxs-lookup"><span data-stu-id="7f865-126">Name</span></span>      |<span data-ttu-id="7f865-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7f865-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f865-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f865-128">Authorization</span></span> | <span data-ttu-id="7f865-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f865-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f865-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f865-131">Request body</span></span>
<span data-ttu-id="7f865-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f865-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7f865-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f865-133">Response</span></span>
<span data-ttu-id="7f865-134">В случае успешной работы этот метод возвращает код отклика и `200 OK` коллекцию [объектов printTask](../resources/printtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f865-134">If successful, this method returns a `200 OK` response code and collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f865-135">Пример</span><span class="sxs-lookup"><span data-stu-id="7f865-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f865-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f865-136">Request</span></span>
<span data-ttu-id="7f865-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f865-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f865-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f865-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks
```
# <a name="c"></a>[<span data-ttu-id="7f865-139">C#</span><span class="sxs-lookup"><span data-stu-id="7f865-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtaskdefinition-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f865-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f865-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtaskdefinition-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f865-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f865-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtaskdefinition-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f865-142">Java</span><span class="sxs-lookup"><span data-stu-id="7f865-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtaskdefinition-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="7f865-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f865-143">Response</span></span>
<span data-ttu-id="7f865-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7f865-144">The following is an example of the response.</span></span>
><span data-ttu-id="7f865-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f865-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 429

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printTask)",
  "value": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


