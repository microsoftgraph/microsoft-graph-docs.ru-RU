---
title: Get taskDefinition
description: Сведения об определении задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: fecc2653a3a37e44ab93b1b39ca7e8adf304b546
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768692"
---
# <a name="get-printtaskdefinition"></a><span data-ttu-id="6fa4c-103">Get printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6fa4c-103">Get printTaskDefinition</span></span>

<span data-ttu-id="6fa4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fa4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6fa4c-105">Сведения об определении задачи.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-105">Get details about a task definition.</span></span>

<span data-ttu-id="6fa4c-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="6fa4c-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fa4c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fa4c-107">Permissions</span></span>
<span data-ttu-id="6fa4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6fa4c-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="6fa4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fa4c-111">Permission type</span></span> | <span data-ttu-id="6fa4c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fa4c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6fa4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fa4c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6fa4c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-114">Not supported.</span></span> |
|<span data-ttu-id="6fa4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fa4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-116">Not Supported.</span></span>|
|<span data-ttu-id="6fa4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fa4c-117">Application</span></span>| <span data-ttu-id="6fa4c-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa4c-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fa4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fa4c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="6fa4c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fa4c-120">Request headers</span></span>
|<span data-ttu-id="6fa4c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6fa4c-121">Name</span></span>|<span data-ttu-id="6fa4c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6fa4c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6fa4c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fa4c-123">Authorization</span></span>|<span data-ttu-id="6fa4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa4c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fa4c-126">Request body</span></span>
<span data-ttu-id="6fa4c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fa4c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fa4c-128">Response</span></span>

<span data-ttu-id="6fa4c-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fa4c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6fa4c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fa4c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fa4c-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6fa4c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa4c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```
# <a name="c"></a>[<span data-ttu-id="6fa4c-133">C#</span><span class="sxs-lookup"><span data-stu-id="6fa4c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtaskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fa4c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fa4c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtaskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fa4c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fa4c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtaskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fa4c-136">Java</span><span class="sxs-lookup"><span data-stu-id="6fa4c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtaskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fa4c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fa4c-137">Response</span></span>
<span data-ttu-id="6fa4c-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6fa4c-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

