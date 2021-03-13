---
title: Удаление печатиTaskTrigger
description: Удаление триггера задач принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bba66bb6c11d930b1b9065769181f55efc114dd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772018"
---
# <a name="delete-printtasktrigger"></a><span data-ttu-id="23cbc-103">Удаление печатиTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="23cbc-103">Delete printTaskTrigger</span></span>
<span data-ttu-id="23cbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23cbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="23cbc-105">Удалите [триггер задач](../resources/printtasktrigger.md) [принтера, чтобы](../resources/printer.md) предотвратить связанные события печати для запуска задач на указанном принтере.</span><span class="sxs-lookup"><span data-stu-id="23cbc-105">Delete the [task trigger](../resources/printtasktrigger.md) of a [printer](../resources/printer.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="23cbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23cbc-106">Permissions</span></span>
<span data-ttu-id="23cbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="23cbc-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="23cbc-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="23cbc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23cbc-110">Permission type</span></span> | <span data-ttu-id="23cbc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23cbc-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="23cbc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23cbc-112">Delegated (work or school account)</span></span>| <span data-ttu-id="23cbc-113">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="23cbc-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="23cbc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23cbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cbc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23cbc-115">Not Supported.</span></span>|
|<span data-ttu-id="23cbc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23cbc-116">Application</span></span>|<span data-ttu-id="23cbc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23cbc-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23cbc-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="23cbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23cbc-119">Request headers</span></span>
|<span data-ttu-id="23cbc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="23cbc-120">Name</span></span>|<span data-ttu-id="23cbc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="23cbc-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23cbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23cbc-122">Authorization</span></span>|<span data-ttu-id="23cbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23cbc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23cbc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23cbc-125">Request body</span></span>
<span data-ttu-id="23cbc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23cbc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23cbc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="23cbc-127">Response</span></span>

<span data-ttu-id="23cbc-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23cbc-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="23cbc-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="23cbc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23cbc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="23cbc-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="23cbc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="23cbc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printtasktrigger"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="23cbc-132">C#</span><span class="sxs-lookup"><span data-stu-id="23cbc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printtasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23cbc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23cbc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printtasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23cbc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23cbc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printtasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23cbc-135">Java</span><span class="sxs-lookup"><span data-stu-id="23cbc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printtasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="23cbc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="23cbc-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

