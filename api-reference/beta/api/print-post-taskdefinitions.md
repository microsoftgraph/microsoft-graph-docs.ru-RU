---
title: Создание taskDefinition
description: Создайте новое определение задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4b2a655047ed3700d42e8c672115f0457cc879e9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966992"
---
# <a name="create-taskdefinition"></a><span data-ttu-id="20864-103">Создание taskDefinition</span><span class="sxs-lookup"><span data-stu-id="20864-103">Create taskDefinition</span></span>

<span data-ttu-id="20864-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20864-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20864-105">Создайте новое определение задачи.</span><span class="sxs-lookup"><span data-stu-id="20864-105">Create a new task definition.</span></span>

<span data-ttu-id="20864-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="20864-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="20864-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20864-107">Permissions</span></span>
<span data-ttu-id="20864-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="20864-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="20864-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="20864-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20864-111">Permission type</span></span> | <span data-ttu-id="20864-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20864-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="20864-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20864-113">Delegated (work or school account)</span></span>| <span data-ttu-id="20864-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20864-114">Not supported.</span></span> |
|<span data-ttu-id="20864-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20864-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20864-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20864-116">Not Supported.</span></span>|
|<span data-ttu-id="20864-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="20864-117">Application</span></span>| <span data-ttu-id="20864-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20864-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20864-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20864-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="20864-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20864-120">Request headers</span></span>
| <span data-ttu-id="20864-121">Имя</span><span class="sxs-lookup"><span data-stu-id="20864-121">Name</span></span>      |<span data-ttu-id="20864-122">Описание</span><span class="sxs-lookup"><span data-stu-id="20864-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20864-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20864-123">Authorization</span></span> | <span data-ttu-id="20864-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20864-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20864-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20864-126">Content-type</span></span>  | <span data-ttu-id="20864-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20864-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20864-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20864-129">Request body</span></span>
<span data-ttu-id="20864-130">В тексте запроса добавьте представление объекта [принттаскдефинитион](../resources/printtaskdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20864-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="20864-131">Свойства [принттаскдефинитион](../resources/printtaskdefinition.md) **ID** и **createdBy. AppID** задаются автоматически при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="20864-131">The [printTaskDefinition](../resources/printtaskdefinition.md)'s **id** and **createdBy.appId** properties are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="20864-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="20864-132">Response</span></span>
<span data-ttu-id="20864-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [принттаскдефинитион](../resources/printtaskdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20864-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20864-134">Пример</span><span class="sxs-lookup"><span data-stu-id="20864-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="20864-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="20864-135">Request</span></span>
<span data-ttu-id="20864-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20864-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="20864-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="20864-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="20864-138">C#</span><span class="sxs-lookup"><span data-stu-id="20864-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-create-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20864-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20864-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-create-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20864-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20864-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-create-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20864-141">Java</span><span class="sxs-lookup"><span data-stu-id="20864-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-create-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="20864-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="20864-142">Response</span></span>
<span data-ttu-id="20864-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20864-143">The following is an example of the response.</span></span>
><span data-ttu-id="20864-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20864-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


