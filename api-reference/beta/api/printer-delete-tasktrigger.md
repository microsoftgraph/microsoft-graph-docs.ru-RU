---
title: Удаление Тасктригжер
description: Удаление триггера задачи принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c96edf3379e1d20e35070e4e131ffb08cce98d5f
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091723"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="b5c5d-103">Удаление Тасктригжер</span><span class="sxs-lookup"><span data-stu-id="b5c5d-103">Delete taskTrigger</span></span>

<span data-ttu-id="b5c5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5c5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5c5d-105">Удаление [триггера задачи](../resources/printtasktrigger.md) [принтера](../resources/printer.md)для предотвращения выполнения задач, связанных с печатью, на указанном принтере.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5c5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5c5d-106">Permissions</span></span>
<span data-ttu-id="b5c5d-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b5c5d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5c5d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b5c5d-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b5c5d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5c5d-110">Permission type</span></span> | <span data-ttu-id="b5c5d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5c5d-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b5c5d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5c5d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b5c5d-113">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="b5c5d-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="b5c5d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5c5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5c5d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-115">Not Supported.</span></span>|
|<span data-ttu-id="b5c5d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5c5d-116">Application</span></span>|<span data-ttu-id="b5c5d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5c5d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5c5d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b5c5d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5c5d-119">Request headers</span></span>
| <span data-ttu-id="b5c5d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b5c5d-120">Name</span></span>          | <span data-ttu-id="b5c5d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b5c5d-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b5c5d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5c5d-122">Authorization</span></span> | <span data-ttu-id="b5c5d-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-123">Bearer {token}.</span></span> <span data-ttu-id="b5c5d-124">Required.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5c5d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5c5d-125">Request body</span></span>
<span data-ttu-id="b5c5d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5c5d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5c5d-127">Response</span></span>
<span data-ttu-id="b5c5d-128">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-128">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="b5c5d-129">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-129">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5c5d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b5c5d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5c5d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5c5d-131">Request</span></span>
<span data-ttu-id="b5c5d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```

---

##### <a name="response"></a><span data-ttu-id="b5c5d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5c5d-133">Response</span></span>
<span data-ttu-id="b5c5d-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-134">The following is an example of the response.</span></span>
><span data-ttu-id="b5c5d-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b5c5d-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b5c5d-136">All the properties will be returned from an actual call.</span></span>
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
