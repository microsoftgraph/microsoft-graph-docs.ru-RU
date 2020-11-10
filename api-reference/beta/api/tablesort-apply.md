---
title: 'TableSort: apply'
description: Выполнение сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b047f9f6d9203b11ad4306a20fa26b8056af0405
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978627"
---
# <a name="tablesort-apply"></a><span data-ttu-id="cae0a-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="cae0a-103">TableSort: apply</span></span>

<span data-ttu-id="cae0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae0a-105">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="cae0a-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="cae0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae0a-106">Permissions</span></span>
<span data-ttu-id="cae0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae0a-109">Permission type</span></span>      | <span data-ttu-id="cae0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cae0a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cae0a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cae0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae0a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cae0a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cae0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae0a-115">Application</span></span> | <span data-ttu-id="cae0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae0a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="cae0a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae0a-118">Request headers</span></span>
| <span data-ttu-id="cae0a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cae0a-119">Name</span></span>       | <span data-ttu-id="cae0a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cae0a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cae0a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cae0a-121">Authorization</span></span>  | <span data-ttu-id="cae0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae0a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cae0a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cae0a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="cae0a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cae0a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cae0a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae0a-127">Request body</span></span>
<span data-ttu-id="cae0a-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cae0a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cae0a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="cae0a-129">Parameter</span></span>    | <span data-ttu-id="cae0a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cae0a-130">Type</span></span>   |<span data-ttu-id="cae0a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cae0a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cae0a-132">fields</span><span class="sxs-lookup"><span data-stu-id="cae0a-132">fields</span></span>|<span data-ttu-id="cae0a-133">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="cae0a-133">workbookSortField collection</span></span>|<span data-ttu-id="cae0a-134">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="cae0a-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="cae0a-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="cae0a-135">matchCase</span></span>|<span data-ttu-id="cae0a-136">boolean</span><span class="sxs-lookup"><span data-stu-id="cae0a-136">boolean</span></span>|<span data-ttu-id="cae0a-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="cae0a-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="cae0a-139">method</span><span class="sxs-lookup"><span data-stu-id="cae0a-139">method</span></span>|<span data-ttu-id="cae0a-140">string</span><span class="sxs-lookup"><span data-stu-id="cae0a-140">string</span></span>|<span data-ttu-id="cae0a-p105">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="cae0a-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="cae0a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae0a-144">Response</span></span>

<span data-ttu-id="cae0a-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cae0a-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae0a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="cae0a-147">Example</span></span>
<span data-ttu-id="cae0a-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cae0a-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cae0a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae0a-149">Request</span></span>
<span data-ttu-id="cae0a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae0a-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cae0a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae0a-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cae0a-152">C#</span><span class="sxs-lookup"><span data-stu-id="cae0a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cae0a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae0a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae0a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae0a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cae0a-155">Java</span><span class="sxs-lookup"><span data-stu-id="cae0a-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cae0a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae0a-156">Response</span></span>
<span data-ttu-id="cae0a-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cae0a-157">Here is an example of the response.</span></span> 
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


