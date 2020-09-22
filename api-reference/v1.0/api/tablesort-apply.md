---
title: 'TableSort: apply'
description: Выполнение сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6fb2cff67ca14baca6dfb9f4bebbb7a79bfe8d3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012775"
---
# <a name="tablesort-apply"></a><span data-ttu-id="c81b0-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="c81b0-103">TableSort: apply</span></span>

<span data-ttu-id="c81b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c81b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c81b0-105">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="c81b0-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="c81b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c81b0-106">Permissions</span></span>
<span data-ttu-id="c81b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c81b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c81b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c81b0-109">Permission type</span></span>      | <span data-ttu-id="c81b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c81b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c81b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c81b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c81b0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c81b0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c81b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c81b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c81b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c81b0-114">Not supported.</span></span>    |
|<span data-ttu-id="c81b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c81b0-115">Application</span></span> | <span data-ttu-id="c81b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c81b0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c81b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c81b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="c81b0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c81b0-118">Request headers</span></span>
| <span data-ttu-id="c81b0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c81b0-119">Name</span></span>       | <span data-ttu-id="c81b0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c81b0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c81b0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c81b0-121">Authorization</span></span>  | <span data-ttu-id="c81b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c81b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c81b0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c81b0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c81b0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c81b0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c81b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c81b0-127">Request body</span></span>
<span data-ttu-id="c81b0-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c81b0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c81b0-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="c81b0-129">Parameter</span></span>    | <span data-ttu-id="c81b0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c81b0-130">Type</span></span>   |<span data-ttu-id="c81b0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c81b0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c81b0-132">fields</span><span class="sxs-lookup"><span data-stu-id="c81b0-132">fields</span></span>|<span data-ttu-id="c81b0-133">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="c81b0-133">WorkbookSortField collection</span></span>|<span data-ttu-id="c81b0-134">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="c81b0-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="c81b0-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="c81b0-135">matchCase</span></span>|<span data-ttu-id="c81b0-136">boolean</span><span class="sxs-lookup"><span data-stu-id="c81b0-136">boolean</span></span>|<span data-ttu-id="c81b0-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="c81b0-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="c81b0-139">method</span><span class="sxs-lookup"><span data-stu-id="c81b0-139">method</span></span>|<span data-ttu-id="c81b0-140">string</span><span class="sxs-lookup"><span data-stu-id="c81b0-140">string</span></span>|<span data-ttu-id="c81b0-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c81b0-141">Optional.</span></span> <span data-ttu-id="c81b0-142">Метод сортировки, используемый для китайских символов.</span><span class="sxs-lookup"><span data-stu-id="c81b0-142">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="c81b0-143">Возможные значения: `PinYin` , `StrokeCount` .</span><span class="sxs-lookup"><span data-stu-id="c81b0-143">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c81b0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c81b0-144">Response</span></span>

<span data-ttu-id="c81b0-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c81b0-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c81b0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c81b0-147">Example</span></span>
<span data-ttu-id="c81b0-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c81b0-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c81b0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c81b0-149">Request</span></span>
<span data-ttu-id="c81b0-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c81b0-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c81b0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="c81b0-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

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
  "method": "method-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c81b0-152">C#</span><span class="sxs-lookup"><span data-stu-id="c81b0-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c81b0-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c81b0-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c81b0-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c81b0-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c81b0-155">Java</span><span class="sxs-lookup"><span data-stu-id="c81b0-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c81b0-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c81b0-156">Response</span></span>
<span data-ttu-id="c81b0-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c81b0-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

