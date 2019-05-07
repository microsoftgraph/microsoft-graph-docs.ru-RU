---
title: 'reportRoot: getOffice365ActivationCounts'
description: Получите количество активаций Office 365 на компьютерах и мобильных устройствах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 080a5bf3694d5134338b4eb321eb38eaf00785bc
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639455"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="597ee-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="597ee-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="597ee-104">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="597ee-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="597ee-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="597ee-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="597ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="597ee-106">Permissions</span></span>

<span data-ttu-id="597ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="597ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="597ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="597ee-109">Permission type</span></span>                        | <span data-ttu-id="597ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="597ee-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="597ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="597ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="597ee-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="597ee-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="597ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="597ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="597ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="597ee-114">Not supported.</span></span>                           |
| <span data-ttu-id="597ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="597ee-115">Application</span></span>                            | <span data-ttu-id="597ee-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="597ee-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="597ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="597ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="597ee-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="597ee-118">Query parameters</span></span>

<span data-ttu-id="597ee-119">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="597ee-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="597ee-120">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="597ee-120">The default output type is text/csv.</span></span> <span data-ttu-id="597ee-121">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="597ee-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="597ee-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="597ee-122">Request headers</span></span>

| <span data-ttu-id="597ee-123">Имя</span><span class="sxs-lookup"><span data-stu-id="597ee-123">Name</span></span>          | <span data-ttu-id="597ee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="597ee-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="597ee-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="597ee-125">Authorization</span></span> | <span data-ttu-id="597ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="597ee-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="597ee-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="597ee-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="597ee-129">CSV</span><span class="sxs-lookup"><span data-stu-id="597ee-129">CSV</span></span>

<span data-ttu-id="597ee-130">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="597ee-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="597ee-131">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="597ee-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="597ee-132">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="597ee-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="597ee-133">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="597ee-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="597ee-134">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="597ee-134">Report Refresh Date</span></span>
- <span data-ttu-id="597ee-135">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="597ee-135">Product Type</span></span>
- <span data-ttu-id="597ee-136">Windows</span><span class="sxs-lookup"><span data-stu-id="597ee-136">Windows</span></span>
- <span data-ttu-id="597ee-137">Mac</span><span class="sxs-lookup"><span data-stu-id="597ee-137">Mac</span></span>
- <span data-ttu-id="597ee-138">Android</span><span class="sxs-lookup"><span data-stu-id="597ee-138">Android</span></span>
- <span data-ttu-id="597ee-139">iOS</span><span class="sxs-lookup"><span data-stu-id="597ee-139">iOS</span></span>
- <span data-ttu-id="597ee-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="597ee-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="597ee-141">JSON</span><span class="sxs-lookup"><span data-stu-id="597ee-141">JSON</span></span>

<span data-ttu-id="597ee-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActivationCounts](../resources/office365activationcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="597ee-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="597ee-143">Пример</span><span class="sxs-lookup"><span data-stu-id="597ee-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="597ee-144">CSV</span><span class="sxs-lookup"><span data-stu-id="597ee-144">CSV</span></span>

<span data-ttu-id="597ee-145">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="597ee-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="597ee-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="597ee-146">Request</span></span>

<span data-ttu-id="597ee-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="597ee-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="597ee-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="597ee-148">Response</span></span>

<span data-ttu-id="597ee-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="597ee-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="597ee-150">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="597ee-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="597ee-151">Языках</span><span class="sxs-lookup"><span data-stu-id="597ee-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="597ee-152">Язык</span><span class="sxs-lookup"><span data-stu-id="597ee-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="597ee-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="597ee-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="597ee-154">JSON</span><span class="sxs-lookup"><span data-stu-id="597ee-154">JSON</span></span>

<span data-ttu-id="597ee-155">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="597ee-155">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="597ee-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="597ee-156">Request</span></span>

<span data-ttu-id="597ee-157">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="597ee-157">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="597ee-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="597ee-158">Response</span></span>

<span data-ttu-id="597ee-159">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="597ee-159">The following example shows the response.</span></span>

> <span data-ttu-id="597ee-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="597ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="597ee-162">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="597ee-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="597ee-163">Языках</span><span class="sxs-lookup"><span data-stu-id="597ee-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="597ee-164">Язык</span><span class="sxs-lookup"><span data-stu-id="597ee-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationcounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
