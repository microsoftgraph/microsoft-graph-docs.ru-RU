---
title: 'Воркбукаппликатион: Calculate'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fc82d01c7304ca566534d650f7fdda8dc6ca295e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448488"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="cb992-103">Воркбукаппликатион: Calculate</span><span class="sxs-lookup"><span data-stu-id="cb992-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb992-104">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="cb992-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb992-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb992-105">Permissions</span></span>
<span data-ttu-id="cb992-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb992-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb992-108">Permission type</span></span>      | <span data-ttu-id="cb992-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb992-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb992-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb992-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb992-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb992-111">Not supported.</span></span>    |
|<span data-ttu-id="cb992-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb992-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb992-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb992-113">Not supported.</span></span>    |
|<span data-ttu-id="cb992-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb992-114">Application</span></span> | <span data-ttu-id="cb992-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb992-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb992-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb992-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="cb992-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb992-117">Request headers</span></span>
| <span data-ttu-id="cb992-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cb992-118">Name</span></span>       | <span data-ttu-id="cb992-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cb992-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cb992-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb992-120">Authorization</span></span>  | <span data-ttu-id="cb992-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb992-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb992-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb992-123">Request body</span></span>
<span data-ttu-id="cb992-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cb992-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb992-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="cb992-125">Parameter</span></span>    | <span data-ttu-id="cb992-126">Тип</span><span class="sxs-lookup"><span data-stu-id="cb992-126">Type</span></span>   |<span data-ttu-id="cb992-127">Описание</span><span class="sxs-lookup"><span data-stu-id="cb992-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb992-128">Калкулатионтипе</span><span class="sxs-lookup"><span data-stu-id="cb992-128">calculationType</span></span>|<span data-ttu-id="cb992-129">string</span><span class="sxs-lookup"><span data-stu-id="cb992-129">string</span></span>|<span data-ttu-id="cb992-130">Определяет тип расчета, который нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="cb992-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="cb992-131">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="cb992-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="cb992-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb992-132">Response</span></span>

<span data-ttu-id="cb992-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cb992-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb992-135">Пример</span><span class="sxs-lookup"><span data-stu-id="cb992-135">Example</span></span>
<span data-ttu-id="cb992-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cb992-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cb992-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb992-137">Request</span></span>
<span data-ttu-id="cb992-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb992-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cb992-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb992-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb992-140">C#</span><span class="sxs-lookup"><span data-stu-id="cb992-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb992-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb992-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb992-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cb992-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cb992-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb992-143">Response</span></span>
<span data-ttu-id="cb992-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb992-144">Here is an example of the response.</span></span> 
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
