---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 757a7d6fe8b6fca0ee980a0ef93852fe1ab6d433
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265396"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="6c44b-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="6c44b-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c44b-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="6c44b-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="6c44b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="6c44b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c44b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c44b-106">Permissions</span></span>

<span data-ttu-id="6c44b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c44b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c44b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c44b-109">Permission type</span></span>                        | <span data-ttu-id="6c44b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c44b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6c44b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c44b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c44b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c44b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6c44b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c44b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c44b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c44b-114">Not supported.</span></span>                           |
| <span data-ttu-id="6c44b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c44b-115">Application</span></span>                            | <span data-ttu-id="6c44b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c44b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6c44b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c44b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="6c44b-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="6c44b-118">Query parameters</span></span>

<span data-ttu-id="6c44b-119">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6c44b-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6c44b-120">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="6c44b-120">The default output type is text/csv.</span></span> <span data-ttu-id="6c44b-121">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6c44b-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c44b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c44b-122">Request headers</span></span>

| <span data-ttu-id="6c44b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6c44b-123">Name</span></span>          | <span data-ttu-id="6c44b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6c44b-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6c44b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c44b-125">Authorization</span></span> | <span data-ttu-id="6c44b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c44b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6c44b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c44b-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6c44b-129">CSV</span><span class="sxs-lookup"><span data-stu-id="6c44b-129">CSV</span></span>

<span data-ttu-id="6c44b-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6c44b-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6c44b-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6c44b-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6c44b-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6c44b-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6c44b-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6c44b-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6c44b-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6c44b-134">Report Refresh Date</span></span>
- <span data-ttu-id="6c44b-135">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="6c44b-135">Product Type</span></span>
- <span data-ttu-id="6c44b-136">Windows</span><span class="sxs-lookup"><span data-stu-id="6c44b-136">Windows</span></span>
- <span data-ttu-id="6c44b-137">Mac</span><span class="sxs-lookup"><span data-stu-id="6c44b-137">Mac</span></span>
- <span data-ttu-id="6c44b-138">Android</span><span class="sxs-lookup"><span data-stu-id="6c44b-138">Android</span></span>
- <span data-ttu-id="6c44b-139">iOS</span><span class="sxs-lookup"><span data-stu-id="6c44b-139">iOS</span></span>
- <span data-ttu-id="6c44b-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="6c44b-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="6c44b-141">JSON</span><span class="sxs-lookup"><span data-stu-id="6c44b-141">JSON</span></span>

<span data-ttu-id="6c44b-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationCounts](../resources/office365activationcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c44b-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c44b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6c44b-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6c44b-144">CSV</span><span class="sxs-lookup"><span data-stu-id="6c44b-144">CSV</span></span>

<span data-ttu-id="6c44b-145">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="6c44b-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6c44b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c44b-146">Request</span></span>

<span data-ttu-id="6c44b-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c44b-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6c44b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c44b-148">Response</span></span>

<span data-ttu-id="6c44b-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c44b-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c44b-150">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="6c44b-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c44b-151">C#</span><span class="sxs-lookup"><span data-stu-id="6c44b-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c44b-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c44b-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6c44b-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6c44b-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6c44b-154">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6c44b-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="6c44b-155">JSON</span><span class="sxs-lookup"><span data-stu-id="6c44b-155">JSON</span></span>

<span data-ttu-id="6c44b-156">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="6c44b-156">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6c44b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c44b-157">Request</span></span>

<span data-ttu-id="6c44b-158">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c44b-158">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6c44b-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c44b-159">Response</span></span>

<span data-ttu-id="6c44b-160">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c44b-160">The following example shows the response.</span></span>

> <span data-ttu-id="6c44b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c44b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c44b-163">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6c44b-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c44b-164">C#</span><span class="sxs-lookup"><span data-stu-id="6c44b-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c44b-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c44b-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6c44b-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6c44b-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
