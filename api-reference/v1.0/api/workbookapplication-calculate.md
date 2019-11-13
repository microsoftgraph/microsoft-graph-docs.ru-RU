---
title: 'Воркбукаппликатион: Calculate'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 288476706d1569a71827dc1441e1ec362ac6ca89
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302298"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="3b7f3-103">Воркбукаппликатион: Calculate</span><span class="sxs-lookup"><span data-stu-id="3b7f3-103">workbookApplication: calculate</span></span>

<span data-ttu-id="3b7f3-104">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-104">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b7f3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b7f3-105">Permissions</span></span>
<span data-ttu-id="3b7f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b7f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b7f3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b7f3-108">Permission type</span></span>      | <span data-ttu-id="3b7f3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b7f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b7f3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b7f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b7f3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b7f3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b7f3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b7f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b7f3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-113">Not supported.</span></span>    |
|<span data-ttu-id="3b7f3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b7f3-114">Application</span></span> | <span data-ttu-id="3b7f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b7f3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b7f3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="3b7f3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b7f3-117">Request headers</span></span>
| <span data-ttu-id="3b7f3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3b7f3-118">Name</span></span>       | <span data-ttu-id="3b7f3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3b7f3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3b7f3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b7f3-120">Authorization</span></span>  | <span data-ttu-id="3b7f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b7f3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b7f3-123">Content-type</span></span> | <span data-ttu-id="3b7f3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b7f3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b7f3-126">Request body</span></span>
<span data-ttu-id="3b7f3-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3b7f3-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="3b7f3-128">Parameter</span></span>    | <span data-ttu-id="3b7f3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3b7f3-129">Type</span></span>   |<span data-ttu-id="3b7f3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b7f3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b7f3-131">калкулатионтипе</span><span class="sxs-lookup"><span data-stu-id="3b7f3-131">calculationType</span></span>|<span data-ttu-id="3b7f3-132">string</span><span class="sxs-lookup"><span data-stu-id="3b7f3-132">string</span></span>|<span data-ttu-id="3b7f3-133">Определяет тип расчета, который нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-133">Specifies the calculation type to use.</span></span>  <span data-ttu-id="3b7f3-134">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-134">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="3b7f3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b7f3-135">Response</span></span>

<span data-ttu-id="3b7f3-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b7f3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3b7f3-138">Example</span></span>
<span data-ttu-id="3b7f3-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="3b7f3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b7f3-140">Request</span></span>
<span data-ttu-id="3b7f3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-141">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3b7f3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b7f3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b7f3-143">C#</span><span class="sxs-lookup"><span data-stu-id="3b7f3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b7f3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b7f3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b7f3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b7f3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3b7f3-146">Java</span><span class="sxs-lookup"><span data-stu-id="3b7f3-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3b7f3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b7f3-147">Response</span></span>
<span data-ttu-id="3b7f3-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b7f3-148">Here is an example of the response.</span></span> 
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
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
