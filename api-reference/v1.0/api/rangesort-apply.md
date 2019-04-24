---
title: 'RangeSort: apply'
description: Выполнение операции сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be024f3eacbb4e2d1178ec7b82a8e8ca604aff60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32452708"
---
# <a name="rangesort-apply"></a><span data-ttu-id="d3c4c-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="d3c4c-103">RangeSort: apply</span></span>

<span data-ttu-id="d3c4c-104">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3c4c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3c4c-105">Permissions</span></span>
<span data-ttu-id="d3c4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c4c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3c4c-108">Permission type</span></span>      | <span data-ttu-id="d3c4c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3c4c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3c4c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3c4c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3c4c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3c4c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3c4c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3c4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3c4c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-113">Not supported.</span></span>    |
|<span data-ttu-id="d3c4c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3c4c-114">Application</span></span> | <span data-ttu-id="d3c4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3c4c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3c4c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="d3c4c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3c4c-117">Request headers</span></span>
| <span data-ttu-id="d3c4c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d3c4c-118">Name</span></span>       | <span data-ttu-id="d3c4c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c4c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3c4c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3c4c-120">Authorization</span></span>  | <span data-ttu-id="d3c4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3c4c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3c4c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3c4c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c4c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3c4c-126">Request body</span></span>
<span data-ttu-id="d3c4c-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3c4c-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="d3c4c-128">Parameter</span></span>    | <span data-ttu-id="d3c4c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d3c4c-129">Type</span></span>   |<span data-ttu-id="d3c4c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c4c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c4c-131">fields</span><span class="sxs-lookup"><span data-stu-id="d3c4c-131">fields</span></span>|<span data-ttu-id="d3c4c-132">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="d3c4c-132">WorkbookSortField collection</span></span>|<span data-ttu-id="d3c4c-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="d3c4c-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="d3c4c-134">matchCase</span></span>|<span data-ttu-id="d3c4c-135">логический</span><span class="sxs-lookup"><span data-stu-id="d3c4c-135">boolean</span></span>|<span data-ttu-id="d3c4c-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="d3c4c-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="d3c4c-138">hasHeaders</span></span>|<span data-ttu-id="d3c4c-139">boolean</span><span class="sxs-lookup"><span data-stu-id="d3c4c-139">boolean</span></span>|<span data-ttu-id="d3c4c-p105">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="d3c4c-142">orientation</span><span class="sxs-lookup"><span data-stu-id="d3c4c-142">orientation</span></span>|<span data-ttu-id="d3c4c-143">string</span><span class="sxs-lookup"><span data-stu-id="d3c4c-143">string</span></span>|<span data-ttu-id="d3c4c-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-144">Optional.</span></span> <span data-ttu-id="d3c4c-145">Указывает направление сортировки: по строкам или по столбцам.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="d3c4c-146">Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="d3c4c-147">method</span><span class="sxs-lookup"><span data-stu-id="d3c4c-147">method</span></span>|<span data-ttu-id="d3c4c-148">string</span><span class="sxs-lookup"><span data-stu-id="d3c4c-148">string</span></span>|<span data-ttu-id="d3c4c-149">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-149">Optional.</span></span> <span data-ttu-id="d3c4c-150">Метод сортировки, используемый для китайских символов.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="d3c4c-151">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="d3c4c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3c4c-152">Response</span></span>

<span data-ttu-id="d3c4c-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c4c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d3c4c-155">Example</span></span>
<span data-ttu-id="d3c4c-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3c4c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3c4c-157">Request</span></span>
<span data-ttu-id="d3c4c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d3c4c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3c4c-159">Response</span></span>
<span data-ttu-id="d3c4c-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3c4c-160">Here is an example of the response.</span></span> 
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
