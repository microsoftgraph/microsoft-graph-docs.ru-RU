---
title: Обновление taskDefinition
description: Обновление определения задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5923c66eca2da9f2f2016434cfd0d92a0cfa7bef
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766492"
---
# <a name="update-taskdefinition"></a><span data-ttu-id="38fe3-103">Обновление taskDefinition</span><span class="sxs-lookup"><span data-stu-id="38fe3-103">Update taskDefinition</span></span>

<span data-ttu-id="38fe3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38fe3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38fe3-105">Обновление определения задачи.</span><span class="sxs-lookup"><span data-stu-id="38fe3-105">Update a task definition.</span></span>

<span data-ttu-id="38fe3-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="38fe3-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="38fe3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38fe3-107">Permissions</span></span>
<span data-ttu-id="38fe3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38fe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="38fe3-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="38fe3-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="38fe3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38fe3-111">Permission type</span></span> | <span data-ttu-id="38fe3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38fe3-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="38fe3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38fe3-113">Delegated (work or school account)</span></span>| <span data-ttu-id="38fe3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38fe3-114">Not supported.</span></span> |
|<span data-ttu-id="38fe3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38fe3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38fe3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38fe3-116">Not Supported.</span></span>|
|<span data-ttu-id="38fe3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="38fe3-117">Application</span></span>| <span data-ttu-id="38fe3-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38fe3-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38fe3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38fe3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38fe3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38fe3-120">Request headers</span></span>
| <span data-ttu-id="38fe3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="38fe3-121">Name</span></span>      |<span data-ttu-id="38fe3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="38fe3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38fe3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38fe3-123">Authorization</span></span> | <span data-ttu-id="38fe3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38fe3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38fe3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38fe3-126">Content-type</span></span>  | <span data-ttu-id="38fe3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38fe3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38fe3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38fe3-129">Request body</span></span>
<span data-ttu-id="38fe3-130">В теле запроса укажи значения для соответствующих полей [printTaskDefinition,](../resources/printtaskdefinition.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="38fe3-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="38fe3-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="38fe3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="38fe3-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="38fe3-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="38fe3-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="38fe3-133">Property</span></span>     | <span data-ttu-id="38fe3-134">Тип</span><span class="sxs-lookup"><span data-stu-id="38fe3-134">Type</span></span>        | <span data-ttu-id="38fe3-135">Описание</span><span class="sxs-lookup"><span data-stu-id="38fe3-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38fe3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="38fe3-136">displayName</span></span>|<span data-ttu-id="38fe3-137">String</span><span class="sxs-lookup"><span data-stu-id="38fe3-137">String</span></span>|<span data-ttu-id="38fe3-138">Имя печатиTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="38fe3-138">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="38fe3-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="38fe3-139">createdBy</span></span>|<span data-ttu-id="38fe3-140">String</span><span class="sxs-lookup"><span data-stu-id="38fe3-140">String</span></span>|<span data-ttu-id="38fe3-141">Сведения о приложении, создав определение задачи.</span><span class="sxs-lookup"><span data-stu-id="38fe3-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="38fe3-142">Только `createdBy.displayName` свойство может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="38fe3-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="38fe3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="38fe3-143">Response</span></span>
<span data-ttu-id="38fe3-144">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="38fe3-144">If successful, this method returns a `200 OK` response code and an updated [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38fe3-145">Пример</span><span class="sxs-lookup"><span data-stu-id="38fe3-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="38fe3-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="38fe3-146">Request</span></span>
<span data-ttu-id="38fe3-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38fe3-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="38fe3-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="38fe3-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_update_taskdefinition"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="38fe3-149">C#</span><span class="sxs-lookup"><span data-stu-id="38fe3-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-update-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38fe3-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38fe3-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-update-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38fe3-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38fe3-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-update-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38fe3-152">Java</span><span class="sxs-lookup"><span data-stu-id="38fe3-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-update-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="38fe3-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="38fe3-153">Response</span></span>
<span data-ttu-id="38fe3-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="38fe3-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId" : "479688a0-cc3a-4993-ab24-54c7c80b047e",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


