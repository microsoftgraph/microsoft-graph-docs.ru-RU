---
title: Обновление задачи
description: Обновление задачи печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 33c6078aa9265788409abd3e23d736fab9989b0b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053575"
---
# <a name="update-task"></a><span data-ttu-id="20e0a-103">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="20e0a-103">Update task</span></span>

<span data-ttu-id="20e0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20e0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20e0a-105">Обновление задачи печати.</span><span class="sxs-lookup"><span data-stu-id="20e0a-105">Update a print task.</span></span>

<span data-ttu-id="20e0a-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="20e0a-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="20e0a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20e0a-107">Permissions</span></span>
<span data-ttu-id="20e0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="20e0a-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="20e0a-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="20e0a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20e0a-111">Permission type</span></span> | <span data-ttu-id="20e0a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20e0a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="20e0a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20e0a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="20e0a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20e0a-114">Not supported.</span></span> |
|<span data-ttu-id="20e0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20e0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20e0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20e0a-116">Not Supported.</span></span>|
|<span data-ttu-id="20e0a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="20e0a-117">Application</span></span>| <span data-ttu-id="20e0a-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20e0a-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e0a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20e0a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20e0a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20e0a-120">Request headers</span></span>
| <span data-ttu-id="20e0a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="20e0a-121">Name</span></span>      |<span data-ttu-id="20e0a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="20e0a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20e0a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20e0a-123">Authorization</span></span> | <span data-ttu-id="20e0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20e0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20e0a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20e0a-126">Request body</span></span>
<span data-ttu-id="20e0a-127">В теле запроса укажи значения для соответствующих полей [printTask,](../resources/printtask.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="20e0a-127">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="20e0a-128">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="20e0a-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="20e0a-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="20e0a-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="20e0a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20e0a-130">Property</span></span>     | <span data-ttu-id="20e0a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20e0a-131">Type</span></span>        | <span data-ttu-id="20e0a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20e0a-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20e0a-133">status</span><span class="sxs-lookup"><span data-stu-id="20e0a-133">status</span></span>|<span data-ttu-id="20e0a-134">String</span><span class="sxs-lookup"><span data-stu-id="20e0a-134">String</span></span>|<span data-ttu-id="20e0a-135">`state` `description` Включай и значения, описывая текущее состояние задачи.</span><span class="sxs-lookup"><span data-stu-id="20e0a-135">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="20e0a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20e0a-136">Response</span></span>
<span data-ttu-id="20e0a-137">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект printTask](../resources/printtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="20e0a-137">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20e0a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="20e0a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="20e0a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="20e0a-139">Request</span></span>
<span data-ttu-id="20e0a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20e0a-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="20e0a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="20e0a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_task"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="20e0a-142">C#</span><span class="sxs-lookup"><span data-stu-id="20e0a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20e0a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e0a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20e0a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20e0a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20e0a-145">Java</span><span class="sxs-lookup"><span data-stu-id="20e0a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="20e0a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="20e0a-146">Response</span></span>
<span data-ttu-id="20e0a-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="20e0a-147">The following is an example of the response.</span></span>
><span data-ttu-id="20e0a-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="20e0a-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
}
-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "Task execution is completed."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


