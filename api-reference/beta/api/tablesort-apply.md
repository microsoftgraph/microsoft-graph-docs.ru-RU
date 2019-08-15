---
title: 'TableSort: apply'
description: Выполнение сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8a2e0d8910e0933c86c8a4112c41a5ab53253383
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421351"
---
# <a name="tablesort-apply"></a><span data-ttu-id="739b3-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="739b3-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="739b3-104">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="739b3-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="739b3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="739b3-105">Permissions</span></span>
<span data-ttu-id="739b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="739b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="739b3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="739b3-108">Permission type</span></span>      | <span data-ttu-id="739b3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="739b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="739b3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="739b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="739b3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="739b3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="739b3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="739b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="739b3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="739b3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="739b3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="739b3-114">Application</span></span> | <span data-ttu-id="739b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="739b3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="739b3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="739b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="739b3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="739b3-117">Request headers</span></span>
| <span data-ttu-id="739b3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="739b3-118">Name</span></span>       | <span data-ttu-id="739b3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="739b3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="739b3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="739b3-120">Authorization</span></span>  | <span data-ttu-id="739b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="739b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="739b3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="739b3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="739b3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="739b3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="739b3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="739b3-126">Request body</span></span>
<span data-ttu-id="739b3-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="739b3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="739b3-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="739b3-128">Parameter</span></span>    | <span data-ttu-id="739b3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="739b3-129">Type</span></span>   |<span data-ttu-id="739b3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="739b3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="739b3-131">fields</span><span class="sxs-lookup"><span data-stu-id="739b3-131">fields</span></span>|<span data-ttu-id="739b3-132">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="739b3-132">workbookSortField collection</span></span>|<span data-ttu-id="739b3-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="739b3-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="739b3-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="739b3-134">matchCase</span></span>|<span data-ttu-id="739b3-135">boolean</span><span class="sxs-lookup"><span data-stu-id="739b3-135">boolean</span></span>|<span data-ttu-id="739b3-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="739b3-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="739b3-138">method</span><span class="sxs-lookup"><span data-stu-id="739b3-138">method</span></span>|<span data-ttu-id="739b3-139">string</span><span class="sxs-lookup"><span data-stu-id="739b3-139">string</span></span>|<span data-ttu-id="739b3-p105">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="739b3-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="739b3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="739b3-143">Response</span></span>

<span data-ttu-id="739b3-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="739b3-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="739b3-146">Пример</span><span class="sxs-lookup"><span data-stu-id="739b3-146">Example</span></span>
<span data-ttu-id="739b3-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="739b3-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="739b3-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="739b3-148">Request</span></span>
<span data-ttu-id="739b3-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="739b3-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="739b3-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="739b3-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="739b3-151">C#</span><span class="sxs-lookup"><span data-stu-id="739b3-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="739b3-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="739b3-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="739b3-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="739b3-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="739b3-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="739b3-154">Response</span></span>
<span data-ttu-id="739b3-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="739b3-155">Here is an example of the response.</span></span> 
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
