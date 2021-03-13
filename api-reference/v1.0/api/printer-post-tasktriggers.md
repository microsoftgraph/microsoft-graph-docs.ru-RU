---
title: Создание printTaskTrigger
description: Создайте новый триггер задач на указанном принтере.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3ed74256934310df5f5ea99217f8f0956e109eda
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771836"
---
# <a name="create-printtasktrigger"></a><span data-ttu-id="64baa-103">Создание printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="64baa-103">Create printTaskTrigger</span></span>
<span data-ttu-id="64baa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64baa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="64baa-105">Создайте новый [триггер задач](../resources/printtasktrigger.md) на указанном [принтере.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="64baa-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="64baa-106">В настоящее **время на** принтере может быть указан только один триггер задач, но в будущем это ограничение может быть удалено.</span><span class="sxs-lookup"><span data-stu-id="64baa-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="64baa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64baa-107">Permissions</span></span>
<span data-ttu-id="64baa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64baa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="64baa-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="64baa-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="64baa-111">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="64baa-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="64baa-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64baa-112">Permission type</span></span> | <span data-ttu-id="64baa-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64baa-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="64baa-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64baa-114">Delegated (work or school account)</span></span>| <span data-ttu-id="64baa-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="64baa-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="64baa-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64baa-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64baa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64baa-117">Not Supported.</span></span>|
|<span data-ttu-id="64baa-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64baa-118">Application</span></span>|<span data-ttu-id="64baa-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64baa-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64baa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64baa-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="64baa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64baa-121">Request headers</span></span>
|<span data-ttu-id="64baa-122">Имя</span><span class="sxs-lookup"><span data-stu-id="64baa-122">Name</span></span>|<span data-ttu-id="64baa-123">Описание</span><span class="sxs-lookup"><span data-stu-id="64baa-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64baa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64baa-124">Authorization</span></span>|<span data-ttu-id="64baa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64baa-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="64baa-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64baa-127">Content-Type</span></span>|<span data-ttu-id="64baa-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64baa-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64baa-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64baa-130">Request body</span></span>
<span data-ttu-id="64baa-131">В теле запроса подарйте JSON-представление [объекта printTaskTrigger.](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="64baa-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="64baa-132">Поставляем ссылку на [печатьTaskDefinition](../resources/printtaskdefinition.md) с помощью `@odata.bind` формата, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="64baa-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="64baa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64baa-133">Response</span></span>
<span data-ttu-id="64baa-134">В случае успешной работы этот метод возвращает код отклика и `201 Created` [печатьTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="64baa-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64baa-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="64baa-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64baa-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="64baa-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64baa-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="64baa-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printtasktrigger_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
Content-Type: application/json
Content-length: 80

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
}
```
# <a name="c"></a>[<span data-ttu-id="64baa-138">C#</span><span class="sxs-lookup"><span data-stu-id="64baa-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printtasktrigger-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64baa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64baa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printtasktrigger-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64baa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64baa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printtasktrigger-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64baa-141">Java</span><span class="sxs-lookup"><span data-stu-id="64baa-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printtasktrigger-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64baa-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="64baa-142">Response</span></span>
<span data-ttu-id="64baa-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64baa-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

