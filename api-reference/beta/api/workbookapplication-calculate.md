---
title: 'Воркбукаппликатион: Calculate'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2e3a980ae7eab1dd3032ae68b180019ae4c7ceee
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636977"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="08e68-103">Воркбукаппликатион: Calculate</span><span class="sxs-lookup"><span data-stu-id="08e68-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08e68-104">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="08e68-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="08e68-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08e68-105">Permissions</span></span>
<span data-ttu-id="08e68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08e68-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08e68-108">Permission type</span></span>      | <span data-ttu-id="08e68-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08e68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08e68-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08e68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08e68-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e68-111">Not supported.</span></span>    |
|<span data-ttu-id="08e68-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08e68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08e68-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e68-113">Not supported.</span></span>    |
|<span data-ttu-id="08e68-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08e68-114">Application</span></span> | <span data-ttu-id="08e68-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e68-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08e68-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08e68-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="08e68-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08e68-117">Request headers</span></span>
| <span data-ttu-id="08e68-118">Имя</span><span class="sxs-lookup"><span data-stu-id="08e68-118">Name</span></span>       | <span data-ttu-id="08e68-119">Описание</span><span class="sxs-lookup"><span data-stu-id="08e68-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08e68-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08e68-120">Authorization</span></span>  | <span data-ttu-id="08e68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08e68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08e68-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08e68-123">Request body</span></span>
<span data-ttu-id="08e68-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="08e68-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08e68-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="08e68-125">Parameter</span></span>    | <span data-ttu-id="08e68-126">Тип</span><span class="sxs-lookup"><span data-stu-id="08e68-126">Type</span></span>   |<span data-ttu-id="08e68-127">Описание</span><span class="sxs-lookup"><span data-stu-id="08e68-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08e68-128">Калкулатионтипе</span><span class="sxs-lookup"><span data-stu-id="08e68-128">calculationType</span></span>|<span data-ttu-id="08e68-129">string</span><span class="sxs-lookup"><span data-stu-id="08e68-129">string</span></span>|<span data-ttu-id="08e68-130">Определяет тип расчета, который нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="08e68-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="08e68-131">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="08e68-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="08e68-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="08e68-132">Response</span></span>

<span data-ttu-id="08e68-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="08e68-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e68-135">Пример</span><span class="sxs-lookup"><span data-stu-id="08e68-135">Example</span></span>
<span data-ttu-id="08e68-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="08e68-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08e68-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="08e68-137">Request</span></span>
<span data-ttu-id="08e68-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08e68-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="08e68-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="08e68-139">Response</span></span>
<span data-ttu-id="08e68-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08e68-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="08e68-141">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="08e68-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="08e68-142">Языках</span><span class="sxs-lookup"><span data-stu-id="08e68-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08e68-143">Язык</span><span class="sxs-lookup"><span data-stu-id="08e68-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
