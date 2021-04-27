---
title: Удаление taskTrigger
description: Удаление триггера задач принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f98e73a7cf6d1da759ba933d685f72fbf11f2035
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051090"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="26942-103">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="26942-103">Delete taskTrigger</span></span>

<span data-ttu-id="26942-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26942-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26942-105">Удаление [триггера](../resources/printer.md)задач [принтера,](../resources/printtasktrigger.md) чтобы предотвратить запуск связанных событий печати на указанном принтере.</span><span class="sxs-lookup"><span data-stu-id="26942-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="26942-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26942-106">Permissions</span></span>
<span data-ttu-id="26942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="26942-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="26942-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="26942-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26942-110">Permission type</span></span> | <span data-ttu-id="26942-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26942-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="26942-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26942-112">Delegated (work or school account)</span></span>| <span data-ttu-id="26942-113">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="26942-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="26942-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26942-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26942-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26942-115">Not Supported.</span></span>|
|<span data-ttu-id="26942-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="26942-116">Application</span></span>|<span data-ttu-id="26942-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26942-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26942-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26942-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26942-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26942-119">Request headers</span></span>
| <span data-ttu-id="26942-120">Имя</span><span class="sxs-lookup"><span data-stu-id="26942-120">Name</span></span>          | <span data-ttu-id="26942-121">Описание</span><span class="sxs-lookup"><span data-stu-id="26942-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26942-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26942-122">Authorization</span></span> | <span data-ttu-id="26942-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26942-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26942-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26942-125">Request body</span></span>
<span data-ttu-id="26942-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26942-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26942-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="26942-127">Response</span></span>
<span data-ttu-id="26942-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26942-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26942-130">Пример</span><span class="sxs-lookup"><span data-stu-id="26942-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26942-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="26942-131">Request</span></span>
<span data-ttu-id="26942-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26942-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26942-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="26942-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```
# <a name="c"></a>[<span data-ttu-id="26942-134">C#</span><span class="sxs-lookup"><span data-stu-id="26942-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26942-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26942-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26942-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26942-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26942-137">Java</span><span class="sxs-lookup"><span data-stu-id="26942-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="26942-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="26942-138">Response</span></span>
<span data-ttu-id="26942-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26942-139">The following is an example of the response.</span></span>
><span data-ttu-id="26942-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26942-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


