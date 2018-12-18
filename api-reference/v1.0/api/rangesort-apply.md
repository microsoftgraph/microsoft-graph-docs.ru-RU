---
title: 'RangeSort: apply'
description: Выполняет сортировку.
author: lumine2008
ms.openlocfilehash: 98585be62b8aa227ea5e648d1e24e2a09cb023d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352110"
---
# <a name="rangesort-apply"></a><span data-ttu-id="e0710-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="e0710-103">RangeSort: apply</span></span>

<span data-ttu-id="e0710-104">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="e0710-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0710-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0710-105">Permissions</span></span>
<span data-ttu-id="e0710-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0710-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0710-108">Permission type</span></span>      | <span data-ttu-id="e0710-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0710-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0710-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0710-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0710-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0710-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0710-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0710-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0710-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0710-113">Not supported.</span></span>    |
|<span data-ttu-id="e0710-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0710-114">Application</span></span> | <span data-ttu-id="e0710-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0710-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0710-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0710-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="e0710-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0710-117">Request headers</span></span>
| <span data-ttu-id="e0710-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e0710-118">Name</span></span>       | <span data-ttu-id="e0710-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e0710-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0710-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0710-120">Authorization</span></span>  | <span data-ttu-id="e0710-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0710-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0710-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0710-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0710-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0710-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0710-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0710-126">Request body</span></span>
<span data-ttu-id="e0710-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e0710-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0710-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e0710-128">Parameter</span></span>    | <span data-ttu-id="e0710-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e0710-129">Type</span></span>   |<span data-ttu-id="e0710-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e0710-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0710-131">fields</span><span class="sxs-lookup"><span data-stu-id="e0710-131">fields</span></span>|<span data-ttu-id="e0710-132">WorkbookSortField коллекции</span><span class="sxs-lookup"><span data-stu-id="e0710-132">WorkbookSortField collection</span></span>|<span data-ttu-id="e0710-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="e0710-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="e0710-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="e0710-134">matchCase</span></span>|<span data-ttu-id="e0710-135">boolean</span><span class="sxs-lookup"><span data-stu-id="e0710-135">boolean</span></span>|<span data-ttu-id="e0710-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="e0710-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="e0710-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="e0710-138">hasHeaders</span></span>|<span data-ttu-id="e0710-139">boolean</span><span class="sxs-lookup"><span data-stu-id="e0710-139">boolean</span></span>|<span data-ttu-id="e0710-p105">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="e0710-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="e0710-142">orientation</span><span class="sxs-lookup"><span data-stu-id="e0710-142">orientation</span></span>|<span data-ttu-id="e0710-143">string</span><span class="sxs-lookup"><span data-stu-id="e0710-143">string</span></span>|<span data-ttu-id="e0710-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e0710-144">Optional.</span></span> <span data-ttu-id="e0710-145">Является ли операция сортировки, строк или столбцов.</span><span class="sxs-lookup"><span data-stu-id="e0710-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="e0710-146">Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="e0710-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="e0710-147">метод</span><span class="sxs-lookup"><span data-stu-id="e0710-147">method</span></span>|<span data-ttu-id="e0710-148">string</span><span class="sxs-lookup"><span data-stu-id="e0710-148">string</span></span>|<span data-ttu-id="e0710-149">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e0710-149">Optional.</span></span> <span data-ttu-id="e0710-150">Метода упорядочения, используемый для китайских знаков.</span><span class="sxs-lookup"><span data-stu-id="e0710-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="e0710-151">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="e0710-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="e0710-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0710-152">Response</span></span>

<span data-ttu-id="e0710-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e0710-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0710-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e0710-155">Example</span></span>
<span data-ttu-id="e0710-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e0710-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0710-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0710-157">Request</span></span>
<span data-ttu-id="e0710-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0710-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="e0710-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0710-159">Response</span></span>
<span data-ttu-id="e0710-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0710-160">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->