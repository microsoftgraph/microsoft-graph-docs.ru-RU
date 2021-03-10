---
title: 'RangeSort: apply'
description: Выполнение операции сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 23e71091a9758fd3cef821985c7443e07a3945b6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573903"
---
# <a name="rangesort-apply"></a><span data-ttu-id="b2a77-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="b2a77-103">RangeSort: apply</span></span>

<span data-ttu-id="b2a77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2a77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2a77-105">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="b2a77-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2a77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a77-106">Permissions</span></span>
<span data-ttu-id="b2a77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2a77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2a77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a77-109">Permission type</span></span>      | <span data-ttu-id="b2a77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2a77-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2a77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2a77-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2a77-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2a77-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2a77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2a77-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2a77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2a77-114">Not supported.</span></span>    |
|<span data-ttu-id="b2a77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2a77-115">Application</span></span> | <span data-ttu-id="b2a77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2a77-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2a77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2a77-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/sort/apply
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/sort/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/sort/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="b2a77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2a77-118">Request headers</span></span>
| <span data-ttu-id="b2a77-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b2a77-119">Name</span></span>       | <span data-ttu-id="b2a77-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b2a77-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2a77-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2a77-121">Authorization</span></span>  | <span data-ttu-id="b2a77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2a77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2a77-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2a77-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2a77-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b2a77-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2a77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2a77-127">Request body</span></span>
<span data-ttu-id="b2a77-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b2a77-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b2a77-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="b2a77-129">Parameter</span></span>    | <span data-ttu-id="b2a77-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b2a77-130">Type</span></span>   |<span data-ttu-id="b2a77-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b2a77-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2a77-132">fields</span><span class="sxs-lookup"><span data-stu-id="b2a77-132">fields</span></span>|<span data-ttu-id="b2a77-133">Коллекция WorkbookSortField</span><span class="sxs-lookup"><span data-stu-id="b2a77-133">WorkbookSortField collection</span></span>|<span data-ttu-id="b2a77-134">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="b2a77-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="b2a77-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="b2a77-135">matchCase</span></span>|<span data-ttu-id="b2a77-136">boolean</span><span class="sxs-lookup"><span data-stu-id="b2a77-136">boolean</span></span>|<span data-ttu-id="b2a77-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="b2a77-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="b2a77-139">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="b2a77-139">hasHeaders</span></span>|<span data-ttu-id="b2a77-140">boolean</span><span class="sxs-lookup"><span data-stu-id="b2a77-140">boolean</span></span>|<span data-ttu-id="b2a77-p105">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="b2a77-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="b2a77-143">orientation</span><span class="sxs-lookup"><span data-stu-id="b2a77-143">orientation</span></span>|<span data-ttu-id="b2a77-144">string</span><span class="sxs-lookup"><span data-stu-id="b2a77-144">string</span></span>|<span data-ttu-id="b2a77-145">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b2a77-145">Optional.</span></span> <span data-ttu-id="b2a77-146">Указывает направление сортировки: по строкам или по столбцам.</span><span class="sxs-lookup"><span data-stu-id="b2a77-146">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="b2a77-147">Возможные значения: `Rows` , `Columns` .</span><span class="sxs-lookup"><span data-stu-id="b2a77-147">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="b2a77-148">method</span><span class="sxs-lookup"><span data-stu-id="b2a77-148">method</span></span>|<span data-ttu-id="b2a77-149">string</span><span class="sxs-lookup"><span data-stu-id="b2a77-149">string</span></span>|<span data-ttu-id="b2a77-150">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b2a77-150">Optional.</span></span> <span data-ttu-id="b2a77-151">Метод сортировки, используемый для китайских символов.</span><span class="sxs-lookup"><span data-stu-id="b2a77-151">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="b2a77-152">Возможные значения: `PinYin` , `StrokeCount` .</span><span class="sxs-lookup"><span data-stu-id="b2a77-152">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="b2a77-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2a77-153">Response</span></span>

<span data-ttu-id="b2a77-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b2a77-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2a77-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b2a77-156">Example</span></span>
<span data-ttu-id="b2a77-157">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b2a77-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b2a77-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2a77-158">Request</span></span>
<span data-ttu-id="b2a77-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2a77-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2a77-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2a77-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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
# <a name="c"></a>[<span data-ttu-id="b2a77-161">C#</span><span class="sxs-lookup"><span data-stu-id="b2a77-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2a77-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2a77-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2a77-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2a77-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2a77-164">Java</span><span class="sxs-lookup"><span data-stu-id="b2a77-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b2a77-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2a77-165">Response</span></span>
<span data-ttu-id="b2a77-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2a77-166">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

