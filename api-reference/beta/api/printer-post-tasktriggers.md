---
title: Создание taskTrigger
description: Создайте новый триггер задач на указанном принтере.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cd654963b8aa5dc5ce30c2fadc644fb3aaa03568
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052028"
---
# <a name="create-tasktrigger"></a><span data-ttu-id="c8fdd-103">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="c8fdd-103">Create taskTrigger</span></span>

<span data-ttu-id="c8fdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8fdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8fdd-105">Создайте новый [триггер задач](../resources/printtasktrigger.md) на указанном [принтере.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c8fdd-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="c8fdd-106">В настоящее **время на** принтере может быть указан только один триггер задач, но в будущем это ограничение может быть удалено.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c8fdd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8fdd-107">Permissions</span></span>
<span data-ttu-id="c8fdd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8fdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c8fdd-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="c8fdd-111">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c8fdd-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c8fdd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8fdd-112">Permission type</span></span> | <span data-ttu-id="c8fdd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8fdd-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c8fdd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8fdd-114">Delegated (work or school account)</span></span>| <span data-ttu-id="c8fdd-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c8fdd-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="c8fdd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8fdd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8fdd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-117">Not Supported.</span></span>|
|<span data-ttu-id="c8fdd-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8fdd-118">Application</span></span>|<span data-ttu-id="c8fdd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8fdd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8fdd-120">HTTP request</span></span>

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="c8fdd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8fdd-121">Request headers</span></span>
| <span data-ttu-id="c8fdd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c8fdd-122">Name</span></span>      |<span data-ttu-id="c8fdd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c8fdd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8fdd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8fdd-124">Authorization</span></span> | <span data-ttu-id="c8fdd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8fdd-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8fdd-127">Content-type</span></span>  | <span data-ttu-id="c8fdd-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8fdd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8fdd-130">Request body</span></span>
<span data-ttu-id="c8fdd-131">В теле запроса подарйте JSON-представление [объекта printTaskTrigger.](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="c8fdd-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="c8fdd-132">Поставляем ссылку на [печатьTaskDefinition](../resources/printtaskdefinition.md) с помощью `@odata.bind` формата, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="c8fdd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8fdd-133">Response</span></span>
<span data-ttu-id="c8fdd-134">В случае успешной работы этот метод возвращает код отклика и `201 Created` [печатьTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8fdd-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c8fdd-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8fdd-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8fdd-136">Request</span></span>
<span data-ttu-id="c8fdd-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c8fdd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8fdd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer_tasktrigger"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
}
```
# <a name="c"></a>[<span data-ttu-id="c8fdd-139">C#</span><span class="sxs-lookup"><span data-stu-id="c8fdd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8fdd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8fdd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8fdd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8fdd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8fdd-142">Java</span><span class="sxs-lookup"><span data-stu-id="c8fdd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c8fdd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8fdd-143">Response</span></span>
<span data-ttu-id="c8fdd-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-144">The following is an example of the response.</span></span>
><span data-ttu-id="c8fdd-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8fdd-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 196

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```
