---
title: 'Worksheet: delete'
description: Удаляет лист из книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ce10683421dd5011b57de55a235c14ded6d5647a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777764"
---
# <a name="worksheet-delete"></a><span data-ttu-id="b7755-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="b7755-103">Worksheet: delete</span></span>

<span data-ttu-id="b7755-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7755-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7755-105">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="b7755-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7755-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7755-106">Permissions</span></span>
<span data-ttu-id="b7755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7755-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7755-109">Permission type</span></span>      | <span data-ttu-id="b7755-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7755-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7755-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7755-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7755-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7755-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7755-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7755-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7755-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7755-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7755-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7755-115">Application</span></span> | <span data-ttu-id="b7755-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7755-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7755-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7755-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="b7755-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7755-118">Request headers</span></span>
| <span data-ttu-id="b7755-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b7755-119">Name</span></span>       | <span data-ttu-id="b7755-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b7755-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7755-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7755-121">Authorization</span></span>  | <span data-ttu-id="b7755-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7755-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7755-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7755-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7755-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b7755-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7755-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7755-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b7755-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7755-128">Response</span></span>

<span data-ttu-id="b7755-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b7755-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7755-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7755-131">Example</span></span>
<span data-ttu-id="b7755-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b7755-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7755-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7755-133">Request</span></span>
<span data-ttu-id="b7755-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7755-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7755-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7755-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="b7755-136">C#</span><span class="sxs-lookup"><span data-stu-id="b7755-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7755-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7755-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7755-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7755-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7755-139">Java</span><span class="sxs-lookup"><span data-stu-id="b7755-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b7755-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7755-140">Response</span></span>
<span data-ttu-id="b7755-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7755-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


