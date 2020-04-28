---
title: 'Range: unmerge'
description: Разъединяет ячейки диапазона на отдельные ячейки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f9be0a1827e495895f9338d3f710637b810e39ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454703"
---
# <a name="range-unmerge"></a><span data-ttu-id="39667-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="39667-103">Range: unmerge</span></span>

<span data-ttu-id="39667-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39667-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39667-105">Разъединяет ячейки диапазона на отдельные ячейки.</span><span class="sxs-lookup"><span data-stu-id="39667-105">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="39667-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39667-106">Permissions</span></span>
<span data-ttu-id="39667-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39667-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39667-109">Permission type</span></span>      | <span data-ttu-id="39667-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39667-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39667-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39667-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39667-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39667-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39667-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39667-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39667-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39667-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39667-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39667-115">Application</span></span> | <span data-ttu-id="39667-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39667-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39667-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39667-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="39667-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39667-118">Request headers</span></span>
| <span data-ttu-id="39667-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39667-119">Name</span></span>       | <span data-ttu-id="39667-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39667-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39667-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39667-121">Authorization</span></span>  | <span data-ttu-id="39667-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39667-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39667-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39667-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="39667-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="39667-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39667-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39667-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="39667-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="39667-128">Response</span></span>

<span data-ttu-id="39667-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="39667-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39667-131">Пример</span><span class="sxs-lookup"><span data-stu-id="39667-131">Example</span></span>
<span data-ttu-id="39667-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="39667-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="39667-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="39667-133">Request</span></span>
<span data-ttu-id="39667-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39667-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39667-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="39667-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="c"></a>[<span data-ttu-id="39667-136">C#</span><span class="sxs-lookup"><span data-stu-id="39667-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39667-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39667-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39667-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39667-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="39667-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="39667-139">Response</span></span>
<span data-ttu-id="39667-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39667-140">Here is an example of the response.</span></span> 
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
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
