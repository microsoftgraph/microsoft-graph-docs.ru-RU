---
title: Get taskDefinition
description: Сведения об определении задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 40e3b2c32545cebc548cbaec27463904ea5ce384
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053589"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="f40d8-103">Get taskDefinition</span><span class="sxs-lookup"><span data-stu-id="f40d8-103">Get taskDefinition</span></span>

<span data-ttu-id="f40d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f40d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f40d8-105">Сведения об определении задачи.</span><span class="sxs-lookup"><span data-stu-id="f40d8-105">Get details about a task definition.</span></span>

<span data-ttu-id="f40d8-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="f40d8-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f40d8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f40d8-107">Permissions</span></span>
<span data-ttu-id="f40d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f40d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f40d8-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="f40d8-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f40d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f40d8-111">Permission type</span></span> | <span data-ttu-id="f40d8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f40d8-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f40d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f40d8-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f40d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f40d8-114">Not supported.</span></span> |
|<span data-ttu-id="f40d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f40d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f40d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f40d8-116">Not Supported.</span></span>|
|<span data-ttu-id="f40d8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f40d8-117">Application</span></span>| <span data-ttu-id="f40d8-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f40d8-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f40d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f40d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f40d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f40d8-120">Request headers</span></span>
| <span data-ttu-id="f40d8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f40d8-121">Name</span></span>      |<span data-ttu-id="f40d8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f40d8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f40d8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f40d8-123">Authorization</span></span> | <span data-ttu-id="f40d8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f40d8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f40d8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f40d8-126">Request body</span></span>
<span data-ttu-id="f40d8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f40d8-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f40d8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f40d8-128">Response</span></span>
<span data-ttu-id="f40d8-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f40d8-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f40d8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f40d8-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="f40d8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f40d8-131">Request</span></span>
<span data-ttu-id="f40d8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f40d8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f40d8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f40d8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```
# <a name="c"></a>[<span data-ttu-id="f40d8-134">C#</span><span class="sxs-lookup"><span data-stu-id="f40d8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f40d8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f40d8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f40d8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f40d8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f40d8-137">Java</span><span class="sxs-lookup"><span data-stu-id="f40d8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f40d8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f40d8-138">Response</span></span>
<span data-ttu-id="f40d8-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f40d8-139">The following is an example of the response.</span></span>
><span data-ttu-id="f40d8-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f40d8-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


