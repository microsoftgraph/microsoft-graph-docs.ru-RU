---
title: 'RangeSort: apply'
description: Выполнение операции сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7979033ce520f0d29172a910f4935c428bee383f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538268"
---
# <a name="rangesort-apply"></a><span data-ttu-id="2c7de-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="2c7de-103">RangeSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c7de-104">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="2c7de-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c7de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c7de-105">Permissions</span></span>
<span data-ttu-id="2c7de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c7de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c7de-108">Permission type</span></span>      | <span data-ttu-id="2c7de-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c7de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c7de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c7de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c7de-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c7de-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c7de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c7de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c7de-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c7de-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c7de-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c7de-114">Application</span></span> | <span data-ttu-id="2c7de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c7de-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c7de-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c7de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="2c7de-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c7de-117">Request headers</span></span>
| <span data-ttu-id="2c7de-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2c7de-118">Name</span></span>       | <span data-ttu-id="2c7de-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2c7de-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c7de-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c7de-120">Authorization</span></span>  | <span data-ttu-id="2c7de-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c7de-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2c7de-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2c7de-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c7de-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c7de-126">Request body</span></span>
<span data-ttu-id="2c7de-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2c7de-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c7de-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c7de-128">Parameter</span></span>    | <span data-ttu-id="2c7de-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2c7de-129">Type</span></span>   |<span data-ttu-id="2c7de-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2c7de-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c7de-131">fields</span><span class="sxs-lookup"><span data-stu-id="2c7de-131">fields</span></span>|<span data-ttu-id="2c7de-132">SortField</span><span class="sxs-lookup"><span data-stu-id="2c7de-132">SortField</span></span>|<span data-ttu-id="2c7de-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="2c7de-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="2c7de-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="2c7de-134">matchCase</span></span>|<span data-ttu-id="2c7de-135">логический</span><span class="sxs-lookup"><span data-stu-id="2c7de-135">boolean</span></span>|<span data-ttu-id="2c7de-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="2c7de-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="2c7de-138">hasHeaders</span></span>|<span data-ttu-id="2c7de-139">boolean</span><span class="sxs-lookup"><span data-stu-id="2c7de-139">boolean</span></span>|<span data-ttu-id="2c7de-p105">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="2c7de-142">orientation</span><span class="sxs-lookup"><span data-stu-id="2c7de-142">orientation</span></span>|<span data-ttu-id="2c7de-143">string</span><span class="sxs-lookup"><span data-stu-id="2c7de-143">string</span></span>|<span data-ttu-id="2c7de-p106">Необязательный параметр. Указывает направление сортировки: по строкам или по столбцам.  Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="2c7de-147">метод</span><span class="sxs-lookup"><span data-stu-id="2c7de-147">method</span></span>|<span data-ttu-id="2c7de-148">string</span><span class="sxs-lookup"><span data-stu-id="2c7de-148">string</span></span>|<span data-ttu-id="2c7de-p107">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="2c7de-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c7de-152">Response</span></span>

<span data-ttu-id="2c7de-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2c7de-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c7de-155">Пример</span><span class="sxs-lookup"><span data-stu-id="2c7de-155">Example</span></span>
<span data-ttu-id="2c7de-156">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2c7de-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2c7de-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c7de-157">Request</span></span>
<span data-ttu-id="2c7de-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c7de-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="2c7de-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c7de-159">Response</span></span>
<span data-ttu-id="2c7de-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c7de-160">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
