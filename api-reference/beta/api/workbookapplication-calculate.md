---
title: 'Воркбукаппликатион: Calculate'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 653fd377e59570948716c5e663c2802e729e673a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269820"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="94b77-103">Воркбукаппликатион: Calculate</span><span class="sxs-lookup"><span data-stu-id="94b77-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94b77-104">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="94b77-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="94b77-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94b77-105">Permissions</span></span>
<span data-ttu-id="94b77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94b77-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94b77-108">Permission type</span></span>      | <span data-ttu-id="94b77-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94b77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94b77-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94b77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94b77-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94b77-111">Not supported.</span></span>    |
|<span data-ttu-id="94b77-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94b77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b77-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94b77-113">Not supported.</span></span>    |
|<span data-ttu-id="94b77-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94b77-114">Application</span></span> | <span data-ttu-id="94b77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94b77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94b77-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94b77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="94b77-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94b77-117">Request headers</span></span>
| <span data-ttu-id="94b77-118">Имя</span><span class="sxs-lookup"><span data-stu-id="94b77-118">Name</span></span>       | <span data-ttu-id="94b77-119">Описание</span><span class="sxs-lookup"><span data-stu-id="94b77-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94b77-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94b77-120">Authorization</span></span>  | <span data-ttu-id="94b77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94b77-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94b77-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="94b77-123">Request body</span></span>
<span data-ttu-id="94b77-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="94b77-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94b77-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="94b77-125">Parameter</span></span>    | <span data-ttu-id="94b77-126">Тип</span><span class="sxs-lookup"><span data-stu-id="94b77-126">Type</span></span>   |<span data-ttu-id="94b77-127">Описание</span><span class="sxs-lookup"><span data-stu-id="94b77-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94b77-128">Калкулатионтипе</span><span class="sxs-lookup"><span data-stu-id="94b77-128">calculationType</span></span>|<span data-ttu-id="94b77-129">string</span><span class="sxs-lookup"><span data-stu-id="94b77-129">string</span></span>|<span data-ttu-id="94b77-130">Определяет тип расчета, который нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="94b77-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="94b77-131">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="94b77-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="94b77-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b77-132">Response</span></span>

<span data-ttu-id="94b77-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="94b77-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94b77-135">Пример</span><span class="sxs-lookup"><span data-stu-id="94b77-135">Example</span></span>
<span data-ttu-id="94b77-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="94b77-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94b77-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="94b77-137">Request</span></span>
<span data-ttu-id="94b77-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94b77-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="94b77-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b77-139">Response</span></span>
<span data-ttu-id="94b77-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94b77-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="94b77-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="94b77-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="94b77-142">C#</span><span class="sxs-lookup"><span data-stu-id="94b77-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94b77-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="94b77-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="94b77-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="94b77-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
