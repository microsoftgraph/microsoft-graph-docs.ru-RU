---
title: Удаление Принтершаре
description: Удаление общего принтера (отменяйте общий доступ к связанному принтеру). Это действие невозможно отменить. Если к принтеру предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался принтер, должны обнаружить и повторно установить его.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 78d81fe559d40f6d1244c4ea1c281d48a4337cde
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947701"
---
# <a name="delete-printershare"></a><span data-ttu-id="8d7e3-105">Удаление Принтершаре</span><span class="sxs-lookup"><span data-stu-id="8d7e3-105">Delete printerShare</span></span>

<span data-ttu-id="8d7e3-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d7e3-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d7e3-107">Удаление общего принтера (отменяйте общий доступ к связанному [принтеру](../resources/printer.md)).</span><span class="sxs-lookup"><span data-stu-id="8d7e3-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="8d7e3-108">Это действие невозможно отменить.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-108">This action cannot be undone.</span></span> <span data-ttu-id="8d7e3-109">Если к [принтеру](../resources/printer.md) предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался [принтер](../resources/printer.md) , должны обнаружить и переустановить его.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d7e3-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d7e3-110">Permissions</span></span>
<span data-ttu-id="8d7e3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d7e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8d7e3-113">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-113">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8d7e3-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d7e3-114">Permission type</span></span> | <span data-ttu-id="8d7e3-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d7e3-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8d7e3-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d7e3-116">Delegated (work or school account)</span></span>| <span data-ttu-id="8d7e3-117">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8d7e3-117">Users.Read.All</span></span> |
|<span data-ttu-id="8d7e3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d7e3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d7e3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-119">Not Supported.</span></span>|
|<span data-ttu-id="8d7e3-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d7e3-120">Application</span></span>|<span data-ttu-id="8d7e3-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d7e3-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d7e3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="8d7e3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d7e3-123">Request headers</span></span>
| <span data-ttu-id="8d7e3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8d7e3-124">Name</span></span>          | <span data-ttu-id="8d7e3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8d7e3-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d7e3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d7e3-126">Authorization</span></span> | <span data-ttu-id="8d7e3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d7e3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d7e3-129">Request body</span></span>
<span data-ttu-id="8d7e3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d7e3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d7e3-131">Response</span></span>
<span data-ttu-id="8d7e3-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d7e3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8d7e3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d7e3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d7e3-135">Request</span></span>
<span data-ttu-id="8d7e3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d7e3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d7e3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShares/{id}
```
# <a name="c"></a>[<span data-ttu-id="8d7e3-138">C#</span><span class="sxs-lookup"><span data-stu-id="8d7e3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d7e3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d7e3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d7e3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d7e3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8d7e3-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d7e3-141">Response</span></span>
<span data-ttu-id="8d7e3-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d7e3-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
