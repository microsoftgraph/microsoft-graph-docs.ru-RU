---
title: Перечисление taskDefinitions
description: Получение списка определений задач, которые запрашивает приложение, определенное в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d3a78ed94520477969bf1116cdafee0df20391d9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967037"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="c60ea-103">Перечисление taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c60ea-103">List taskDefinitions</span></span>

<span data-ttu-id="c60ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c60ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c60ea-105">Получение списка [определений задач](../resources/printtaskdefinition.md) , которые запрашивает приложение, определенное в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c60ea-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="c60ea-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="c60ea-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c60ea-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c60ea-107">Permissions</span></span>
<span data-ttu-id="c60ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c60ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c60ea-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="c60ea-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c60ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c60ea-111">Permission type</span></span> | <span data-ttu-id="c60ea-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c60ea-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c60ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c60ea-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c60ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c60ea-114">Not supported.</span></span> |
|<span data-ttu-id="c60ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c60ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c60ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c60ea-116">Not Supported.</span></span>|
|<span data-ttu-id="c60ea-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c60ea-117">Application</span></span>| <span data-ttu-id="c60ea-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c60ea-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c60ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c60ea-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c60ea-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c60ea-120">Optional query parameters</span></span>
<span data-ttu-id="c60ea-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c60ea-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c60ea-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c60ea-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="c60ea-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c60ea-123">Exceptions</span></span>
<span data-ttu-id="c60ea-124">Некоторые операторы не поддерживаются: `$count` , `$format` , `$search` , `$select` , `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="c60ea-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c60ea-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c60ea-125">Request headers</span></span>
| <span data-ttu-id="c60ea-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c60ea-126">Name</span></span>      |<span data-ttu-id="c60ea-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c60ea-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c60ea-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c60ea-128">Authorization</span></span> | <span data-ttu-id="c60ea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c60ea-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c60ea-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c60ea-131">Request body</span></span>
<span data-ttu-id="c60ea-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c60ea-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c60ea-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c60ea-133">Response</span></span>
<span data-ttu-id="c60ea-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принттаскдефинитион](../resources/printtaskdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c60ea-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c60ea-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c60ea-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="c60ea-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c60ea-136">Request</span></span>
<span data-ttu-id="c60ea-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c60ea-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c60ea-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c60ea-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```
# <a name="c"></a>[<span data-ttu-id="c60ea-139">C#</span><span class="sxs-lookup"><span data-stu-id="c60ea-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-list-taskdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c60ea-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c60ea-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-list-taskdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c60ea-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c60ea-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-list-taskdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c60ea-142">Java</span><span class="sxs-lookup"><span data-stu-id="c60ea-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-list-taskdefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c60ea-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c60ea-143">Response</span></span>
<span data-ttu-id="c60ea-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c60ea-144">The following is an example of the response.</span></span>
><span data-ttu-id="c60ea-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c60ea-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


