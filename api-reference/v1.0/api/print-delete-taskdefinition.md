---
title: Удаление taskDefinition
description: Удаление определения задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a9f51962e97bad28f3c30048e826c28d60f15455
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777280"
---
# <a name="delete-printtaskdefinition"></a><span data-ttu-id="c6130-103">Удаление печатиTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c6130-103">Delete printTaskDefinition</span></span>
<span data-ttu-id="c6130-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6130-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c6130-105">Удаление **taskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="c6130-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="c6130-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="c6130-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6130-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6130-107">Permissions</span></span>
<span data-ttu-id="c6130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c6130-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c6130-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c6130-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6130-111">Permission type</span></span> | <span data-ttu-id="c6130-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6130-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c6130-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6130-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c6130-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6130-114">Not supported.</span></span> |
|<span data-ttu-id="c6130-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6130-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6130-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6130-116">Not Supported.</span></span>|
|<span data-ttu-id="c6130-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c6130-117">Application</span></span>| <span data-ttu-id="c6130-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6130-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6130-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6130-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c6130-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6130-120">Request headers</span></span>
|<span data-ttu-id="c6130-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6130-121">Name</span></span>|<span data-ttu-id="c6130-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c6130-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c6130-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6130-123">Authorization</span></span>|<span data-ttu-id="c6130-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6130-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6130-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6130-126">Request body</span></span>
<span data-ttu-id="c6130-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6130-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6130-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6130-128">Response</span></span>
<span data-ttu-id="c6130-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c6130-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6130-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c6130-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c6130-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6130-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c6130-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6130-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printtaskdefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```
# <a name="c"></a>[<span data-ttu-id="c6130-134">C#</span><span class="sxs-lookup"><span data-stu-id="c6130-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printtaskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6130-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6130-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printtaskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6130-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6130-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printtaskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6130-137">Java</span><span class="sxs-lookup"><span data-stu-id="c6130-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printtaskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c6130-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6130-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

