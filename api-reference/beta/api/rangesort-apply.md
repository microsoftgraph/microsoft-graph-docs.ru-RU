---
title: 'RangeSort: apply'
description: Выполнение операции сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3f98985591be30d1b5812765843abe433757997a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874201"
---
# <a name="rangesort-apply"></a><span data-ttu-id="6dd84-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="6dd84-103">RangeSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd84-104">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="6dd84-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="6dd84-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd84-105">Permissions</span></span>
<span data-ttu-id="6dd84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd84-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd84-108">Permission type</span></span>      | <span data-ttu-id="6dd84-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dd84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dd84-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dd84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6dd84-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dd84-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6dd84-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dd84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dd84-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dd84-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6dd84-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dd84-114">Application</span></span> | <span data-ttu-id="6dd84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd84-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dd84-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dd84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="6dd84-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dd84-117">Request headers</span></span>
| <span data-ttu-id="6dd84-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6dd84-118">Name</span></span>       | <span data-ttu-id="6dd84-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd84-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6dd84-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dd84-120">Authorization</span></span>  | <span data-ttu-id="6dd84-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6dd84-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6dd84-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6dd84-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dd84-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6dd84-126">Request body</span></span>
<span data-ttu-id="6dd84-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6dd84-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6dd84-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="6dd84-128">Parameter</span></span>    | <span data-ttu-id="6dd84-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6dd84-129">Type</span></span>   |<span data-ttu-id="6dd84-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd84-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dd84-131">fields</span><span class="sxs-lookup"><span data-stu-id="6dd84-131">fields</span></span>|<span data-ttu-id="6dd84-132">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="6dd84-132">workbookSortField collection</span></span>|<span data-ttu-id="6dd84-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="6dd84-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="6dd84-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="6dd84-134">matchCase</span></span>|<span data-ttu-id="6dd84-135">boolean</span><span class="sxs-lookup"><span data-stu-id="6dd84-135">boolean</span></span>|<span data-ttu-id="6dd84-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="6dd84-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="6dd84-138">hasHeaders</span></span>|<span data-ttu-id="6dd84-139">boolean</span><span class="sxs-lookup"><span data-stu-id="6dd84-139">boolean</span></span>|<span data-ttu-id="6dd84-p105">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="6dd84-142">orientation</span><span class="sxs-lookup"><span data-stu-id="6dd84-142">orientation</span></span>|<span data-ttu-id="6dd84-143">string</span><span class="sxs-lookup"><span data-stu-id="6dd84-143">string</span></span>|<span data-ttu-id="6dd84-p106">Необязательный параметр. Указывает направление сортировки: по строкам или по столбцам.  Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="6dd84-147">метод</span><span class="sxs-lookup"><span data-stu-id="6dd84-147">method</span></span>|<span data-ttu-id="6dd84-148">string</span><span class="sxs-lookup"><span data-stu-id="6dd84-148">string</span></span>|<span data-ttu-id="6dd84-p107">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="6dd84-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd84-152">Response</span></span>

<span data-ttu-id="6dd84-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6dd84-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dd84-155">Пример</span><span class="sxs-lookup"><span data-stu-id="6dd84-155">Example</span></span>
<span data-ttu-id="6dd84-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6dd84-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6dd84-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd84-157">Request</span></span>
<span data-ttu-id="6dd84-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dd84-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6dd84-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dd84-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6dd84-160">C#</span><span class="sxs-lookup"><span data-stu-id="6dd84-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dd84-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="6dd84-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6dd84-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6dd84-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6dd84-163">Java</span><span class="sxs-lookup"><span data-stu-id="6dd84-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6dd84-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd84-164">Response</span></span>
<span data-ttu-id="6dd84-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6dd84-165">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
