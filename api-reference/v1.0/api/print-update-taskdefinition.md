---
title: Обновление печатиTaskDefinition
description: Обновление определения задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: af00ba623907a8e5817208ca4a0f92d69ca2dddc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777112"
---
# <a name="update-printtaskdefinition"></a><span data-ttu-id="2a50b-103">Обновление печатиTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="2a50b-103">Update printTaskDefinition</span></span>

<span data-ttu-id="2a50b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a50b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2a50b-105">Обновление определения задачи.</span><span class="sxs-lookup"><span data-stu-id="2a50b-105">Update a task definition.</span></span>

<span data-ttu-id="2a50b-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="2a50b-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a50b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a50b-107">Permissions</span></span>
<span data-ttu-id="2a50b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a50b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2a50b-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="2a50b-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="2a50b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a50b-111">Permission type</span></span> | <span data-ttu-id="2a50b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a50b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2a50b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a50b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2a50b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a50b-114">Not supported.</span></span> |
|<span data-ttu-id="2a50b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a50b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a50b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a50b-116">Not Supported.</span></span>|
|<span data-ttu-id="2a50b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a50b-117">Application</span></span>| <span data-ttu-id="2a50b-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a50b-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a50b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a50b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="2a50b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a50b-120">Request headers</span></span>
|<span data-ttu-id="2a50b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2a50b-121">Name</span></span>|<span data-ttu-id="2a50b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2a50b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a50b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a50b-123">Authorization</span></span>|<span data-ttu-id="2a50b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a50b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a50b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a50b-126">Content-Type</span></span>|<span data-ttu-id="2a50b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a50b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a50b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a50b-129">Request body</span></span>
<span data-ttu-id="2a50b-130">В теле запроса укажи значения для соответствующих полей [printTaskDefinition,](../resources/printtaskdefinition.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="2a50b-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="2a50b-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="2a50b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2a50b-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2a50b-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2a50b-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a50b-133">Property</span></span>     | <span data-ttu-id="2a50b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="2a50b-134">Type</span></span>        | <span data-ttu-id="2a50b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="2a50b-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a50b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2a50b-136">displayName</span></span>|<span data-ttu-id="2a50b-137">String</span><span class="sxs-lookup"><span data-stu-id="2a50b-137">String</span></span>|<span data-ttu-id="2a50b-138">Имя **печатиTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="2a50b-138">The name of the **printTaskDefinition**.</span></span>|
|<span data-ttu-id="2a50b-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="2a50b-139">createdBy</span></span>|<span data-ttu-id="2a50b-140">String</span><span class="sxs-lookup"><span data-stu-id="2a50b-140">String</span></span>|<span data-ttu-id="2a50b-141">Сведения о приложении, создав определение задачи.</span><span class="sxs-lookup"><span data-stu-id="2a50b-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="2a50b-142">Только `createdBy.displayName` свойство может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="2a50b-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="2a50b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a50b-143">Response</span></span>

<span data-ttu-id="2a50b-144">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a50b-144">If successful, this method returns a `200 OK` response code and an updated [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a50b-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a50b-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a50b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a50b-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2a50b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a50b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printtaskdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2a50b-148">C#</span><span class="sxs-lookup"><span data-stu-id="2a50b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printtaskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a50b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a50b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printtaskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a50b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a50b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printtaskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a50b-151">Java</span><span class="sxs-lookup"><span data-stu-id="2a50b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printtaskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a50b-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a50b-152">Response</span></span>
<span data-ttu-id="2a50b-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a50b-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId" : "479688a0-cc3a-4993-ab24-54c7c80b047e",
    "displayName": "Requesting App Display Name"
  }
}
```

