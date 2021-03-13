---
title: Создание printTaskDefinition
description: Создайте новое определение задачи.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ee7172c76863cb62a24c44ba73de2f02bb27e30c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772214"
---
# <a name="create-printtaskdefinition"></a><span data-ttu-id="1df02-103">Создание printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="1df02-103">Create printTaskDefinition</span></span>
<span data-ttu-id="1df02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1df02-105">Создайте новое определение задачи.</span><span class="sxs-lookup"><span data-stu-id="1df02-105">Create a new task definition.</span></span>

<span data-ttu-id="1df02-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="1df02-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="1df02-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1df02-107">Permissions</span></span>
<span data-ttu-id="1df02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1df02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1df02-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="1df02-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="1df02-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1df02-111">Permission type</span></span> | <span data-ttu-id="1df02-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1df02-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1df02-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1df02-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1df02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df02-114">Not supported.</span></span> |
|<span data-ttu-id="1df02-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1df02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1df02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df02-116">Not Supported.</span></span>|
|<span data-ttu-id="1df02-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1df02-117">Application</span></span>| <span data-ttu-id="1df02-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1df02-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1df02-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1df02-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="1df02-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1df02-120">Request headers</span></span>
|<span data-ttu-id="1df02-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1df02-121">Name</span></span>|<span data-ttu-id="1df02-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1df02-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1df02-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1df02-123">Authorization</span></span>|<span data-ttu-id="1df02-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1df02-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1df02-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1df02-126">Content-Type</span></span>|<span data-ttu-id="1df02-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1df02-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1df02-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1df02-129">Request body</span></span>
<span data-ttu-id="1df02-130">В теле запроса поставляем представление JSON объекта [printTaskDefinition.](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1df02-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="1df02-131">Свойства **id** **и createdBy.appId** объекта [printTaskDefinition](../resources/printtaskdefinition.md) автоматически заданы при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="1df02-131">The **id** and **createdBy.appId** properties of the [printTaskDefinition](../resources/printtaskdefinition.md) object are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="1df02-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df02-132">Response</span></span>

<span data-ttu-id="1df02-133">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1df02-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1df02-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="1df02-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1df02-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1df02-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1df02-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1df02-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printtaskdefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/taskDefinitions
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1df02-137">C#</span><span class="sxs-lookup"><span data-stu-id="1df02-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printtaskdefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1df02-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1df02-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printtaskdefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1df02-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1df02-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printtaskdefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1df02-140">Java</span><span class="sxs-lookup"><span data-stu-id="1df02-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printtaskdefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1df02-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df02-141">Response</span></span>
<span data-ttu-id="1df02-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1df02-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

