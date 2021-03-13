---
title: Обновление задачи
description: Обновление задачи печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1375b48ccecc800111b0e84065f58324124021d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771297"
---
# <a name="update-printtask"></a><span data-ttu-id="c5715-103">Обновление printTask</span><span class="sxs-lookup"><span data-stu-id="c5715-103">Update printTask</span></span>
<span data-ttu-id="c5715-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5715-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c5715-105">Обновление задачи печати.</span><span class="sxs-lookup"><span data-stu-id="c5715-105">Update a print task.</span></span>

<span data-ttu-id="c5715-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="c5715-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5715-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5715-107">Permissions</span></span>
<span data-ttu-id="c5715-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c5715-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c5715-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c5715-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5715-111">Permission type</span></span> | <span data-ttu-id="c5715-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5715-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c5715-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5715-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c5715-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5715-114">Not supported.</span></span> |
|<span data-ttu-id="c5715-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5715-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5715-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5715-116">Not Supported.</span></span>|
|<span data-ttu-id="c5715-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5715-117">Application</span></span>| <span data-ttu-id="c5715-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5715-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5715-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5715-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="c5715-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5715-120">Request headers</span></span>
|<span data-ttu-id="c5715-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c5715-121">Name</span></span>|<span data-ttu-id="c5715-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c5715-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5715-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5715-123">Authorization</span></span>|<span data-ttu-id="c5715-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5715-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c5715-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5715-126">Content-Type</span></span>|<span data-ttu-id="c5715-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5715-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5715-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5715-129">Request body</span></span>

<span data-ttu-id="c5715-130">В теле запроса укажи значения для соответствующих полей [printTask,](../resources/printtask.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="c5715-130">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="c5715-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="c5715-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c5715-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c5715-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c5715-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5715-133">Property</span></span>     | <span data-ttu-id="c5715-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c5715-134">Type</span></span>        | <span data-ttu-id="c5715-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c5715-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c5715-136">status</span><span class="sxs-lookup"><span data-stu-id="c5715-136">status</span></span>|<span data-ttu-id="c5715-137">String</span><span class="sxs-lookup"><span data-stu-id="c5715-137">String</span></span>|<span data-ttu-id="c5715-138">`state` `description` Включай и значения, описывая текущее состояние задачи.</span><span class="sxs-lookup"><span data-stu-id="c5715-138">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="c5715-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5715-139">Response</span></span>

<span data-ttu-id="c5715-140">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект printTask](../resources/printtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c5715-140">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5715-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="c5715-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5715-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5715-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c5715-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5715-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printtask"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
Content-Type: application/json
Content-length: 152

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c5715-144">C#</span><span class="sxs-lookup"><span data-stu-id="c5715-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printtask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5715-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5715-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printtask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5715-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5715-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printtask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5715-147">Java</span><span class="sxs-lookup"><span data-stu-id="c5715-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printtask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5715-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5715-148">Response</span></span>
<span data-ttu-id="c5715-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c5715-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "Task execution is completed."
  }
}
```

