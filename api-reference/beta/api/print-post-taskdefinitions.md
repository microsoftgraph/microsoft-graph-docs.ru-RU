---
title: Создание taskDefinition
description: Создайте новое определение задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2e6a9eaca89e7ec68d2eee2053ead369cbcd5831
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053624"
---
# <a name="create-taskdefinition"></a><span data-ttu-id="28131-103">Создание taskDefinition</span><span class="sxs-lookup"><span data-stu-id="28131-103">Create taskDefinition</span></span>

<span data-ttu-id="28131-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28131-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28131-105">Создайте новое определение задачи.</span><span class="sxs-lookup"><span data-stu-id="28131-105">Create a new task definition.</span></span>

<span data-ttu-id="28131-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="28131-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="28131-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28131-107">Permissions</span></span>
<span data-ttu-id="28131-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="28131-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="28131-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="28131-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28131-111">Permission type</span></span> | <span data-ttu-id="28131-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28131-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="28131-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28131-113">Delegated (work or school account)</span></span>| <span data-ttu-id="28131-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28131-114">Not supported.</span></span> |
|<span data-ttu-id="28131-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28131-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28131-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28131-116">Not Supported.</span></span>|
|<span data-ttu-id="28131-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28131-117">Application</span></span>| <span data-ttu-id="28131-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28131-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28131-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28131-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="28131-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28131-120">Request headers</span></span>
| <span data-ttu-id="28131-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28131-121">Name</span></span>      |<span data-ttu-id="28131-122">Описание</span><span class="sxs-lookup"><span data-stu-id="28131-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28131-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28131-123">Authorization</span></span> | <span data-ttu-id="28131-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28131-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28131-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28131-126">Content-type</span></span>  | <span data-ttu-id="28131-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28131-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28131-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28131-129">Request body</span></span>
<span data-ttu-id="28131-130">В теле запроса поставляем представление JSON объекта [printTaskDefinition.](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28131-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="28131-131">Свойства id и **createdBy.appId** для [печатиTaskDefinition](../resources/printtaskdefinition.md)автоматически заданы при создании ресурсов. </span><span class="sxs-lookup"><span data-stu-id="28131-131">The [printTaskDefinition](../resources/printtaskdefinition.md)'s **id** and **createdBy.appId** properties are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="28131-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="28131-132">Response</span></span>
<span data-ttu-id="28131-133">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="28131-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28131-134">Пример</span><span class="sxs-lookup"><span data-stu-id="28131-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="28131-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="28131-135">Request</span></span>
<span data-ttu-id="28131-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28131-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="28131-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="28131-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_create_taskdefinition"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/print/taskDefinitions
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="28131-138">C#</span><span class="sxs-lookup"><span data-stu-id="28131-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-create-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28131-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28131-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-create-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28131-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28131-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-create-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28131-141">Java</span><span class="sxs-lookup"><span data-stu-id="28131-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-create-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="28131-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="28131-142">Response</span></span>
<span data-ttu-id="28131-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28131-143">The following is an example of the response.</span></span>
><span data-ttu-id="28131-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28131-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 322

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
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
  "description": "Create taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


