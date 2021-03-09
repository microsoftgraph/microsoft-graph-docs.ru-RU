---
title: 'workbookApplication: вычислять'
description: Пересчитывает данные во всех открытых в текущий момент книгах Excel.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 10b3ecd3115b24a6bc614e83a11b48ee12e280d9
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575226"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="bc391-103">workbookApplication: вычислять</span><span class="sxs-lookup"><span data-stu-id="bc391-103">workbookApplication: calculate</span></span>

<span data-ttu-id="bc391-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc391-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc391-105">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="bc391-105">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc391-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc391-106">Permissions</span></span>
<span data-ttu-id="bc391-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc391-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc391-109">Permission type</span></span>      | <span data-ttu-id="bc391-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc391-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc391-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc391-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc391-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc391-112">Files.ReadWrite</span></span>     |
|<span data-ttu-id="bc391-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc391-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc391-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc391-114">Not supported.</span></span>    |
|<span data-ttu-id="bc391-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc391-115">Application</span></span> | <span data-ttu-id="bc391-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc391-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc391-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc391-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/application/calculate
POST /me/drive/root:/{item-path}:/workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="bc391-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc391-118">Request headers</span></span>
| <span data-ttu-id="bc391-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bc391-119">Name</span></span>       | <span data-ttu-id="bc391-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc391-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc391-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc391-121">Authorization</span></span>  | <span data-ttu-id="bc391-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc391-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc391-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc391-124">Content-type</span></span> | <span data-ttu-id="bc391-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc391-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc391-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc391-127">Request body</span></span>
<span data-ttu-id="bc391-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bc391-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bc391-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="bc391-129">Parameter</span></span>    | <span data-ttu-id="bc391-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bc391-130">Type</span></span>   |<span data-ttu-id="bc391-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bc391-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc391-132">calculationType</span><span class="sxs-lookup"><span data-stu-id="bc391-132">calculationType</span></span>|<span data-ttu-id="bc391-133">string</span><span class="sxs-lookup"><span data-stu-id="bc391-133">string</span></span>|<span data-ttu-id="bc391-134">Определяет тип расчета, который нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="bc391-134">Specifies the calculation type to use.</span></span>  <span data-ttu-id="bc391-135">Возможные значения: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="bc391-135">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="bc391-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc391-136">Response</span></span>

<span data-ttu-id="bc391-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bc391-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc391-139">Пример</span><span class="sxs-lookup"><span data-stu-id="bc391-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc391-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc391-140">Request</span></span>
<span data-ttu-id="bc391-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc391-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc391-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc391-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bc391-143">C#</span><span class="sxs-lookup"><span data-stu-id="bc391-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc391-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc391-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc391-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc391-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc391-146">Java</span><span class="sxs-lookup"><span data-stu-id="bc391-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc391-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc391-147">Response</span></span>
<span data-ttu-id="bc391-148">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc391-148">The following example shows the response.</span></span>

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


