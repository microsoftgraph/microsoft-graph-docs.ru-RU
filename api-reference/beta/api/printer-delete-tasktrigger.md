---
title: Удаление taskTrigger
description: Удаление триггера задачи принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c63dad5a4367eb7cf196cf5a6aaf6e1350eef70f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566340"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="12a59-103">Удаление taskTrigger</span><span class="sxs-lookup"><span data-stu-id="12a59-103">Delete taskTrigger</span></span>

<span data-ttu-id="12a59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12a59-105">Удаление [триггера задачи](../resources/printtasktrigger.md) [принтера](../resources/printer.md)для предотвращения выполнения задач, связанных с печатью, на указанном принтере.</span><span class="sxs-lookup"><span data-stu-id="12a59-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="12a59-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12a59-106">Permissions</span></span>
<span data-ttu-id="12a59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="12a59-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="12a59-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="12a59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a59-110">Permission type</span></span> | <span data-ttu-id="12a59-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a59-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="12a59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a59-112">Delegated (work or school account)</span></span>| <span data-ttu-id="12a59-113">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="12a59-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="12a59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a59-115">Not Supported.</span></span>|
|<span data-ttu-id="12a59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a59-116">Application</span></span>|<span data-ttu-id="12a59-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a59-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a59-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="12a59-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a59-119">Request headers</span></span>
| <span data-ttu-id="12a59-120">Имя</span><span class="sxs-lookup"><span data-stu-id="12a59-120">Name</span></span>          | <span data-ttu-id="12a59-121">Описание</span><span class="sxs-lookup"><span data-stu-id="12a59-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="12a59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a59-122">Authorization</span></span> | <span data-ttu-id="12a59-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a59-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12a59-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a59-125">Request body</span></span>
<span data-ttu-id="12a59-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12a59-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a59-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a59-127">Response</span></span>
<span data-ttu-id="12a59-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12a59-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a59-130">Пример</span><span class="sxs-lookup"><span data-stu-id="12a59-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12a59-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a59-131">Request</span></span>
<span data-ttu-id="12a59-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a59-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="12a59-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="12a59-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```
# <a name="c"></a>[<span data-ttu-id="12a59-134">C#</span><span class="sxs-lookup"><span data-stu-id="12a59-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12a59-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12a59-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12a59-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12a59-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="12a59-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a59-137">Response</span></span>
<span data-ttu-id="12a59-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12a59-138">The following is an example of the response.</span></span>
><span data-ttu-id="12a59-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a59-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
