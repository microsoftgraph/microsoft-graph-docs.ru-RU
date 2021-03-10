---
title: 'workbookApplication: вычислять'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 75a3888def2b292ffe4aed1aa178cd4c8709b4e3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577697"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="16285-103">workbookApplication: вычислять</span><span class="sxs-lookup"><span data-stu-id="16285-103">workbookApplication: calculate</span></span>

<span data-ttu-id="16285-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16285-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16285-105">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="16285-105">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="16285-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16285-106">Permissions</span></span>
<span data-ttu-id="16285-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16285-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16285-109">Permission type</span></span>      | <span data-ttu-id="16285-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16285-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16285-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16285-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16285-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16285-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16285-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16285-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16285-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16285-114">Not supported.</span></span>    |
|<span data-ttu-id="16285-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16285-115">Application</span></span> | <span data-ttu-id="16285-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16285-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16285-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16285-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/application/calculate
POST /me/drive/root:/{item-path}:/workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="16285-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16285-118">Request headers</span></span>
| <span data-ttu-id="16285-119">Имя</span><span class="sxs-lookup"><span data-stu-id="16285-119">Name</span></span>       | <span data-ttu-id="16285-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16285-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16285-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16285-121">Authorization</span></span>  | <span data-ttu-id="16285-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16285-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16285-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16285-124">Content-type</span></span> | <span data-ttu-id="16285-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16285-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16285-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16285-127">Request body</span></span>
<span data-ttu-id="16285-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="16285-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16285-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="16285-129">Parameter</span></span>    | <span data-ttu-id="16285-130">Тип</span><span class="sxs-lookup"><span data-stu-id="16285-130">Type</span></span>   |<span data-ttu-id="16285-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16285-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16285-132">calculationType</span><span class="sxs-lookup"><span data-stu-id="16285-132">calculationType</span></span>|<span data-ttu-id="16285-133">string</span><span class="sxs-lookup"><span data-stu-id="16285-133">string</span></span>|<span data-ttu-id="16285-134">Определяет тип расчета, который нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="16285-134">Specifies the calculation type to use.</span></span>  <span data-ttu-id="16285-135">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="16285-135">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="16285-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="16285-136">Response</span></span>

<span data-ttu-id="16285-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16285-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16285-139">Пример</span><span class="sxs-lookup"><span data-stu-id="16285-139">Example</span></span>
<span data-ttu-id="16285-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16285-140">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="16285-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="16285-141">Request</span></span>
<span data-ttu-id="16285-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16285-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16285-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="16285-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="16285-144">C#</span><span class="sxs-lookup"><span data-stu-id="16285-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16285-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16285-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16285-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16285-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16285-147">Java</span><span class="sxs-lookup"><span data-stu-id="16285-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16285-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="16285-148">Response</span></span>
<span data-ttu-id="16285-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16285-149">Here is an example of the response.</span></span> 
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

