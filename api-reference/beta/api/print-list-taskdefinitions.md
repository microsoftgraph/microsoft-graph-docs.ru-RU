---
title: Перечисление taskDefinitions
description: Извлечение списка определений задач, определенных приложением-запросом в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 68de2409013cff88752f5a26f1ea06e2a25bb755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053638"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="b6a7f-103">Перечисление taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="b6a7f-103">List taskDefinitions</span></span>

<span data-ttu-id="b6a7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a7f-105">Извлечение списка [определений задач,](../resources/printtaskdefinition.md) определенных приложением-запросом в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="b6a7f-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="b6a7f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a7f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a7f-107">Permissions</span></span>
<span data-ttu-id="b6a7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b6a7f-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b6a7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a7f-111">Permission type</span></span> | <span data-ttu-id="b6a7f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6a7f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b6a7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a7f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b6a7f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-114">Not supported.</span></span> |
|<span data-ttu-id="b6a7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6a7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-116">Not Supported.</span></span>|
|<span data-ttu-id="b6a7f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b6a7f-117">Application</span></span>| <span data-ttu-id="b6a7f-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a7f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6a7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6a7f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6a7f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6a7f-120">Optional query parameters</span></span>
<span data-ttu-id="b6a7f-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b6a7f-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6a7f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="b6a7f-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b6a7f-123">Exceptions</span></span>
<span data-ttu-id="b6a7f-124">Некоторые операторы не поддерживаются: `$count` , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="b6a7f-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6a7f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6a7f-125">Request headers</span></span>
| <span data-ttu-id="b6a7f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b6a7f-126">Name</span></span>      |<span data-ttu-id="b6a7f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a7f-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6a7f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6a7f-128">Authorization</span></span> | <span data-ttu-id="b6a7f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6a7f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6a7f-131">Request body</span></span>
<span data-ttu-id="b6a7f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b6a7f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a7f-133">Response</span></span>
<span data-ttu-id="b6a7f-134">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6a7f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b6a7f-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6a7f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6a7f-136">Request</span></span>
<span data-ttu-id="b6a7f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6a7f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a7f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```
# <a name="c"></a>[<span data-ttu-id="b6a7f-139">C#</span><span class="sxs-lookup"><span data-stu-id="b6a7f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-list-taskdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6a7f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6a7f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-list-taskdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6a7f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6a7f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-list-taskdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6a7f-142">Java</span><span class="sxs-lookup"><span data-stu-id="b6a7f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-list-taskdefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="b6a7f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6a7f-143">Response</span></span>
<span data-ttu-id="b6a7f-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-144">The following is an example of the response.</span></span>
><span data-ttu-id="b6a7f-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b6a7f-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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


