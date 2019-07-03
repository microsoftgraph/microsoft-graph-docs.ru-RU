---
title: 'TableSort: apply'
description: Выполнение сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1501ede20bf48ff97f131d1635c553cfaee0fc47
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451495"
---
# <a name="tablesort-apply"></a><span data-ttu-id="a87e9-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="a87e9-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a87e9-104">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="a87e9-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="a87e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a87e9-105">Permissions</span></span>
<span data-ttu-id="a87e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a87e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a87e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a87e9-108">Permission type</span></span>      | <span data-ttu-id="a87e9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a87e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a87e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a87e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a87e9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a87e9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a87e9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a87e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a87e9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a87e9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a87e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a87e9-114">Application</span></span> | <span data-ttu-id="a87e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a87e9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a87e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a87e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="a87e9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a87e9-117">Request headers</span></span>
| <span data-ttu-id="a87e9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a87e9-118">Name</span></span>       | <span data-ttu-id="a87e9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a87e9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a87e9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a87e9-120">Authorization</span></span>  | <span data-ttu-id="a87e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a87e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a87e9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a87e9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a87e9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a87e9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a87e9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a87e9-126">Request body</span></span>
<span data-ttu-id="a87e9-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a87e9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a87e9-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="a87e9-128">Parameter</span></span>    | <span data-ttu-id="a87e9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a87e9-129">Type</span></span>   |<span data-ttu-id="a87e9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a87e9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a87e9-131">fields</span><span class="sxs-lookup"><span data-stu-id="a87e9-131">fields</span></span>|<span data-ttu-id="a87e9-132">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="a87e9-132">workbookSortField collection</span></span>|<span data-ttu-id="a87e9-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="a87e9-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="a87e9-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="a87e9-134">matchCase</span></span>|<span data-ttu-id="a87e9-135">boolean</span><span class="sxs-lookup"><span data-stu-id="a87e9-135">boolean</span></span>|<span data-ttu-id="a87e9-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="a87e9-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="a87e9-138">method</span><span class="sxs-lookup"><span data-stu-id="a87e9-138">method</span></span>|<span data-ttu-id="a87e9-139">string</span><span class="sxs-lookup"><span data-stu-id="a87e9-139">string</span></span>|<span data-ttu-id="a87e9-p105">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="a87e9-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="a87e9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a87e9-143">Response</span></span>

<span data-ttu-id="a87e9-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a87e9-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a87e9-146">Пример</span><span class="sxs-lookup"><span data-stu-id="a87e9-146">Example</span></span>
<span data-ttu-id="a87e9-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a87e9-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a87e9-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a87e9-148">Request</span></span>
<span data-ttu-id="a87e9-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a87e9-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a87e9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a87e9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a87e9-151">C#</span><span class="sxs-lookup"><span data-stu-id="a87e9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a87e9-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="a87e9-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a87e9-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a87e9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a87e9-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a87e9-154">Response</span></span>
<span data-ttu-id="a87e9-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a87e9-155">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
