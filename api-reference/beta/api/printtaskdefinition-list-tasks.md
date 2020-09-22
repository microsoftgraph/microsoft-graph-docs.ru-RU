---
title: Перечисление задач
description: Получение списка задач, связанных с определением задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0bb661870b69565d1f692dc2d5406224112968d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035345"
---
# <a name="list-tasks"></a><span data-ttu-id="bc336-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="bc336-103">List tasks</span></span>

<span data-ttu-id="bc336-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc336-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc336-105">Получение списка [задач](../resources/printtask.md) , связанных с [определением задачи](../resources/printtaskdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="bc336-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="bc336-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="bc336-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc336-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc336-107">Permissions</span></span>
<span data-ttu-id="bc336-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bc336-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="bc336-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="bc336-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc336-111">Permission type</span></span> | <span data-ttu-id="bc336-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc336-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bc336-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc336-113">Delegated (work or school account)</span></span>| <span data-ttu-id="bc336-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc336-114">Not supported.</span></span> |
|<span data-ttu-id="bc336-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc336-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc336-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc336-116">Not Supported.</span></span>|
|<span data-ttu-id="bc336-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc336-117">Application</span></span>| <span data-ttu-id="bc336-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc336-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc336-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc336-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc336-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc336-120">Optional query parameters</span></span>
<span data-ttu-id="bc336-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bc336-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bc336-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bc336-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="bc336-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="bc336-123">Exceptions</span></span>
<span data-ttu-id="bc336-124">Некоторые операторы не поддерживаются: `$count` , `$format` , `$search` , `$select` , `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="bc336-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc336-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc336-125">Request headers</span></span>
| <span data-ttu-id="bc336-126">Имя</span><span class="sxs-lookup"><span data-stu-id="bc336-126">Name</span></span>      |<span data-ttu-id="bc336-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bc336-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc336-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc336-128">Authorization</span></span> | <span data-ttu-id="bc336-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc336-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc336-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc336-131">Request body</span></span>
<span data-ttu-id="bc336-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc336-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc336-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc336-133">Response</span></span>
<span data-ttu-id="bc336-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принттаск](../resources/printtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc336-134">If successful, this method returns a `200 OK` response code and collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc336-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bc336-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc336-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc336-136">Request</span></span>
<span data-ttu-id="bc336-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc336-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bc336-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc336-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks
```
# <a name="c"></a>[<span data-ttu-id="bc336-139">C#</span><span class="sxs-lookup"><span data-stu-id="bc336-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtaskdefinition-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc336-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc336-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtaskdefinition-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc336-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc336-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtaskdefinition-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="bc336-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc336-142">Response</span></span>
<span data-ttu-id="bc336-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc336-143">The following is an example of the response.</span></span>
><span data-ttu-id="bc336-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc336-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


