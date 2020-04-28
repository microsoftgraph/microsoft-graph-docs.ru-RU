---
title: Удаление принтера
description: Удаление (Отмена регистрации) принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4f77c6564e321c1e250f89547e7dabad5d1305db
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948038"
---
# <a name="delete-printer"></a><span data-ttu-id="03653-103">Удаление принтера</span><span class="sxs-lookup"><span data-stu-id="03653-103">Delete printer</span></span>

<span data-ttu-id="03653-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03653-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03653-105">Удаление (Отмена регистрации) [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="03653-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03653-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03653-106">Permissions</span></span>
<span data-ttu-id="03653-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="03653-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="03653-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="03653-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03653-110">Permission type</span></span> | <span data-ttu-id="03653-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03653-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="03653-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03653-112">Delegated (work or school account)</span></span>| <span data-ttu-id="03653-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="03653-113">Users.Read.All</span></span> |
|<span data-ttu-id="03653-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03653-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03653-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03653-115">Not Supported.</span></span>|
|<span data-ttu-id="03653-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03653-116">Application</span></span>|<span data-ttu-id="03653-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03653-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03653-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03653-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="03653-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03653-119">Request headers</span></span>
| <span data-ttu-id="03653-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03653-120">Name</span></span>          | <span data-ttu-id="03653-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03653-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03653-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03653-122">Authorization</span></span> | <span data-ttu-id="03653-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03653-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03653-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03653-125">Request body</span></span>
<span data-ttu-id="03653-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03653-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03653-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="03653-127">Response</span></span>
<span data-ttu-id="03653-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03653-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03653-130">Пример</span><span class="sxs-lookup"><span data-stu-id="03653-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03653-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="03653-131">Request</span></span>
<span data-ttu-id="03653-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03653-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03653-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="03653-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="03653-134">C#</span><span class="sxs-lookup"><span data-stu-id="03653-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03653-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03653-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03653-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03653-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03653-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="03653-137">Response</span></span>
<span data-ttu-id="03653-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03653-138">The following is an example of the response.</span></span>
><span data-ttu-id="03653-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03653-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
