---
title: 'Worksheet: UsedRange'
description: Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 444a88dfaad3983948a139f2a3db304c200a1153
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569748"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="cd84a-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="cd84a-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="cd84a-p102">Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.</span><span class="sxs-lookup"><span data-stu-id="cd84a-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd84a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd84a-107">Permissions</span></span>
<span data-ttu-id="cd84a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd84a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd84a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd84a-110">Permission type</span></span>      | <span data-ttu-id="cd84a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd84a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd84a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd84a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd84a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd84a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd84a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd84a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd84a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd84a-115">Not supported.</span></span>    |
|<span data-ttu-id="cd84a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd84a-116">Application</span></span> | <span data-ttu-id="cd84a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd84a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd84a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd84a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="cd84a-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cd84a-119">Function parameters</span></span>
<span data-ttu-id="cd84a-120">В URL-АДРЕСе запроса можно указать необязательные параметры.</span><span class="sxs-lookup"><span data-stu-id="cd84a-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="cd84a-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="cd84a-121">Parameter</span></span>    | <span data-ttu-id="cd84a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="cd84a-122">Type</span></span>   |<span data-ttu-id="cd84a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cd84a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd84a-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="cd84a-124">valuesOnly</span></span>|<span data-ttu-id="cd84a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd84a-125">Boolean</span></span>|<span data-ttu-id="cd84a-p104">Необязательный параметр. Учитывает только ячейки со значениями (игнорирует форматирование).</span><span class="sxs-lookup"><span data-stu-id="cd84a-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="cd84a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd84a-128">Request headers</span></span>
| <span data-ttu-id="cd84a-129">Имя</span><span class="sxs-lookup"><span data-stu-id="cd84a-129">Name</span></span>       | <span data-ttu-id="cd84a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cd84a-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd84a-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd84a-131">Authorization</span></span>  | <span data-ttu-id="cd84a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd84a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd84a-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cd84a-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd84a-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cd84a-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd84a-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd84a-137">Request body</span></span>
<span data-ttu-id="cd84a-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd84a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd84a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd84a-139">Response</span></span>

<span data-ttu-id="cd84a-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cd84a-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd84a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="cd84a-141">Example</span></span>
<span data-ttu-id="cd84a-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cd84a-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cd84a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd84a-143">Request</span></span>
<span data-ttu-id="cd84a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd84a-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="cd84a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd84a-145">Response</span></span>
<span data-ttu-id="cd84a-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd84a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="cd84a-149">Кроме того, эта функция может вызываться с необязательным `valuesOnly` параметром.</span><span class="sxs-lookup"><span data-stu-id="cd84a-149">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="cd84a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd84a-150">Request</span></span>
<span data-ttu-id="cd84a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd84a-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="cd84a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd84a-152">Response</span></span>
<span data-ttu-id="cd84a-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd84a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
