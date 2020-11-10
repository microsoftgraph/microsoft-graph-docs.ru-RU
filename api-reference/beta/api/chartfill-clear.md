---
title: 'ChartFill: clear'
description: Очищает цвет заливки элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 468d4e548d950b5b66b2a9633f8f555494437a96
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958773"
---
# <a name="chartfill-clear"></a><span data-ttu-id="16717-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="16717-103">ChartFill: clear</span></span>

<span data-ttu-id="16717-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16717-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16717-105">Очищает цвет заливки элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="16717-105">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="16717-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16717-106">Permissions</span></span>
<span data-ttu-id="16717-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16717-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16717-109">Permission type</span></span>      | <span data-ttu-id="16717-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16717-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16717-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16717-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16717-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16717-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16717-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16717-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16717-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16717-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16717-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16717-115">Application</span></span> | <span data-ttu-id="16717-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16717-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16717-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16717-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="16717-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16717-118">Request headers</span></span>
| <span data-ttu-id="16717-119">Имя</span><span class="sxs-lookup"><span data-stu-id="16717-119">Name</span></span>       | <span data-ttu-id="16717-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16717-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16717-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16717-121">Authorization</span></span>  | <span data-ttu-id="16717-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16717-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16717-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16717-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="16717-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="16717-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16717-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16717-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="16717-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="16717-128">Response</span></span>

<span data-ttu-id="16717-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="16717-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16717-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16717-131">Example</span></span>
<span data-ttu-id="16717-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16717-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="16717-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="16717-133">Request</span></span>
<span data-ttu-id="16717-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16717-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16717-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="16717-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```
# <a name="c"></a>[<span data-ttu-id="16717-136">C#</span><span class="sxs-lookup"><span data-stu-id="16717-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16717-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16717-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16717-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16717-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16717-139">Java</span><span class="sxs-lookup"><span data-stu-id="16717-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16717-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="16717-140">Response</span></span>
<span data-ttu-id="16717-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16717-141">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


