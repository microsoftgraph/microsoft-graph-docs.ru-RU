---
title: Вывод задачи
description: Получение сведений о задаче печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cc3c56a1fed1c61a41bacd009d9b85d3ee906029
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565195"
---
# <a name="get-task"></a><span data-ttu-id="eabfe-103">Вывод задачи</span><span class="sxs-lookup"><span data-stu-id="eabfe-103">Get task</span></span>

<span data-ttu-id="eabfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eabfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eabfe-105">Получение сведений о задаче печати.</span><span class="sxs-lookup"><span data-stu-id="eabfe-105">Get details about a print task.</span></span>

<span data-ttu-id="eabfe-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="eabfe-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="eabfe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eabfe-107">Permissions</span></span>
<span data-ttu-id="eabfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eabfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eabfe-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="eabfe-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="eabfe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eabfe-111">Permission type</span></span> | <span data-ttu-id="eabfe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eabfe-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eabfe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eabfe-113">Delegated (work or school account)</span></span>| <span data-ttu-id="eabfe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eabfe-114">Not supported.</span></span> |
|<span data-ttu-id="eabfe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eabfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eabfe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eabfe-116">Not Supported.</span></span>|
|<span data-ttu-id="eabfe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eabfe-117">Application</span></span>| <span data-ttu-id="eabfe-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="eabfe-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eabfe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eabfe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eabfe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eabfe-120">Request headers</span></span>
| <span data-ttu-id="eabfe-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eabfe-121">Name</span></span>      |<span data-ttu-id="eabfe-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eabfe-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eabfe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eabfe-123">Authorization</span></span> | <span data-ttu-id="eabfe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eabfe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eabfe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eabfe-126">Request body</span></span>
<span data-ttu-id="eabfe-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eabfe-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eabfe-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="eabfe-128">Response</span></span>
<span data-ttu-id="eabfe-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принттаск](../resources/printtask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eabfe-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eabfe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eabfe-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="eabfe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eabfe-131">Request</span></span>
<span data-ttu-id="eabfe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eabfe-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eabfe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eabfe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_task"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3
```
# <a name="c"></a>[<span data-ttu-id="eabfe-134">C#</span><span class="sxs-lookup"><span data-stu-id="eabfe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eabfe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eabfe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eabfe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eabfe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="eabfe-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eabfe-137">Response</span></span>
<span data-ttu-id="eabfe-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eabfe-138">The following is an example of the response.</span></span>
><span data-ttu-id="eabfe-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eabfe-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
