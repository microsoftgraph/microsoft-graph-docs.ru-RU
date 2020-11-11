---
title: Создание taskTrigger
description: Создание нового триггера задачи на указанном принтере.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 28f3d5890cce55e10d51892e98c8ff5ddf6e6a45
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993983"
---
# <a name="create-tasktrigger"></a><span data-ttu-id="10eef-103">Создание taskTrigger</span><span class="sxs-lookup"><span data-stu-id="10eef-103">Create taskTrigger</span></span>

<span data-ttu-id="10eef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10eef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10eef-105">Создание нового [триггера задачи](../resources/printtasktrigger.md) на указанном [принтере](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="10eef-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="10eef-106">В настоящее время для каждого принтера можно указать только **один** триггер задачи, но это предельное значение может быть удалено в будущем.</span><span class="sxs-lookup"><span data-stu-id="10eef-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="10eef-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10eef-107">Permissions</span></span>
<span data-ttu-id="10eef-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10eef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="10eef-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="10eef-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="10eef-111">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="10eef-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="10eef-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10eef-112">Permission type</span></span> | <span data-ttu-id="10eef-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10eef-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="10eef-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10eef-114">Delegated (work or school account)</span></span>| <span data-ttu-id="10eef-115">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="10eef-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="10eef-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10eef-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10eef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10eef-117">Not Supported.</span></span>|
|<span data-ttu-id="10eef-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="10eef-118">Application</span></span>|<span data-ttu-id="10eef-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10eef-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10eef-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10eef-120">HTTP request</span></span>

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="10eef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10eef-121">Request headers</span></span>
| <span data-ttu-id="10eef-122">Имя</span><span class="sxs-lookup"><span data-stu-id="10eef-122">Name</span></span>      |<span data-ttu-id="10eef-123">Описание</span><span class="sxs-lookup"><span data-stu-id="10eef-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10eef-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10eef-124">Authorization</span></span> | <span data-ttu-id="10eef-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10eef-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10eef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10eef-127">Content-type</span></span>  | <span data-ttu-id="10eef-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10eef-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10eef-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10eef-130">Request body</span></span>
<span data-ttu-id="10eef-131">В тексте запроса добавьте представление объекта [принттасктригжер](../resources/printtasktrigger.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10eef-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="10eef-132">Предоставьте ссылку на [принттаскдефинитион](../resources/printtaskdefinition.md) с помощью `@odata.bind` формата, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="10eef-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="10eef-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="10eef-133">Response</span></span>
<span data-ttu-id="10eef-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [принттасктригжер](../resources/printtasktrigger.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10eef-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10eef-135">Пример</span><span class="sxs-lookup"><span data-stu-id="10eef-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="10eef-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="10eef-136">Request</span></span>
<span data-ttu-id="10eef-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10eef-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10eef-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="10eef-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="10eef-139">C#</span><span class="sxs-lookup"><span data-stu-id="10eef-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10eef-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10eef-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10eef-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10eef-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10eef-142">Java</span><span class="sxs-lookup"><span data-stu-id="10eef-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="10eef-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="10eef-143">Response</span></span>
<span data-ttu-id="10eef-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10eef-144">The following is an example of the response.</span></span>
><span data-ttu-id="10eef-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10eef-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
