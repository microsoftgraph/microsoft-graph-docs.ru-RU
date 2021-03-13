---
title: Перечисление задач
description: Извлечение списка задач, связанных с определением задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 38948e3a6844654b11f9af6b7ded7ea86b1afb3a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768675"
---
# <a name="list-tasks"></a><span data-ttu-id="4420f-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="4420f-103">List tasks</span></span>
<span data-ttu-id="4420f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4420f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4420f-105">Извлечение списка [задач, связанных](../resources/printtask.md) с [определением задач.](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4420f-105">Retrieve a list of [tasks](../resources/printtask.md) associated with a [task definition](../resources/printtaskdefinition.md).</span></span>

<span data-ttu-id="4420f-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="4420f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="4420f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4420f-107">Permissions</span></span>
<span data-ttu-id="4420f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4420f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4420f-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="4420f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4420f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4420f-111">Permission type</span></span> | <span data-ttu-id="4420f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4420f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4420f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4420f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4420f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4420f-114">Not supported.</span></span> |
|<span data-ttu-id="4420f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4420f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4420f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4420f-116">Not Supported.</span></span>|
|<span data-ttu-id="4420f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4420f-117">Application</span></span>| <span data-ttu-id="4420f-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4420f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4420f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4420f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4420f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4420f-120">Optional query parameters</span></span>
<span data-ttu-id="4420f-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4420f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4420f-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4420f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="4420f-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="4420f-123">Exceptions</span></span>
<span data-ttu-id="4420f-124">Некоторые операторы не поддерживаются: `$count` , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="4420f-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4420f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4420f-125">Request headers</span></span>
|<span data-ttu-id="4420f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4420f-126">Name</span></span>|<span data-ttu-id="4420f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4420f-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4420f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4420f-128">Authorization</span></span>|<span data-ttu-id="4420f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4420f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4420f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4420f-131">Request body</span></span>
<span data-ttu-id="4420f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4420f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4420f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4420f-133">Response</span></span>

<span data-ttu-id="4420f-134">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов printTask](../resources/printtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4420f-134">If successful, this method returns a `200 OK` response code and a collection of [printTask](../resources/printtask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4420f-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="4420f-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4420f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4420f-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4420f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4420f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks
```
# <a name="c"></a>[<span data-ttu-id="4420f-138">C#</span><span class="sxs-lookup"><span data-stu-id="4420f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4420f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4420f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4420f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4420f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4420f-141">Java</span><span class="sxs-lookup"><span data-stu-id="4420f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4420f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4420f-142">Response</span></span>
<span data-ttu-id="4420f-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4420f-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printTask)",
  "value": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

