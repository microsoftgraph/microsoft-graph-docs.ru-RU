---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 60910677e83a8139db1b94be523ef2332f49942d
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639399"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="da674-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="da674-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da674-104">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="da674-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="da674-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="da674-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="da674-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da674-106">Permissions</span></span>

<span data-ttu-id="da674-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da674-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da674-109">Permission type</span></span>                        | <span data-ttu-id="da674-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da674-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="da674-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da674-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da674-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da674-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="da674-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da674-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da674-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da674-114">Not supported.</span></span>                           |
| <span data-ttu-id="da674-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da674-115">Application</span></span>                            | <span data-ttu-id="da674-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da674-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="da674-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da674-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="da674-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="da674-118">Function parameters</span></span>

<span data-ttu-id="da674-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="da674-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="da674-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="da674-120">Parameter</span></span> | <span data-ttu-id="da674-121">Тип</span><span class="sxs-lookup"><span data-stu-id="da674-121">Type</span></span>   | <span data-ttu-id="da674-122">Описание</span><span class="sxs-lookup"><span data-stu-id="da674-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="da674-123">period</span><span class="sxs-lookup"><span data-stu-id="da674-123">period</span></span>    | <span data-ttu-id="da674-124">string</span><span class="sxs-lookup"><span data-stu-id="da674-124">string</span></span> | <span data-ttu-id="da674-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="da674-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="da674-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="da674-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="da674-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="da674-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="da674-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da674-128">Required.</span></span> |

<span data-ttu-id="da674-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="da674-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="da674-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="da674-130">The default output type is text/csv.</span></span> <span data-ttu-id="da674-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="da674-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da674-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da674-132">Request headers</span></span>

| <span data-ttu-id="da674-133">Имя</span><span class="sxs-lookup"><span data-stu-id="da674-133">Name</span></span>          | <span data-ttu-id="da674-134">Описание</span><span class="sxs-lookup"><span data-stu-id="da674-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="da674-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da674-135">Authorization</span></span> | <span data-ttu-id="da674-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da674-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="da674-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da674-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="da674-139">CSV</span><span class="sxs-lookup"><span data-stu-id="da674-139">CSV</span></span>

<span data-ttu-id="da674-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="da674-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="da674-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="da674-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="da674-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="da674-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="da674-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="da674-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="da674-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="da674-144">Report Refresh Date</span></span>
- <span data-ttu-id="da674-145">Mailbox Storage Used (Byte) [занято почтовыми ящиками (байт)]</span><span class="sxs-lookup"><span data-stu-id="da674-145">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="da674-146">Site Storage Used (Byte) [занято сайтами (байт)]</span><span class="sxs-lookup"><span data-stu-id="da674-146">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="da674-147">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="da674-147">Report Date</span></span>
- <span data-ttu-id="da674-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="da674-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="da674-149">JSON</span><span class="sxs-lookup"><span data-stu-id="da674-149">JSON</span></span>

<span data-ttu-id="da674-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da674-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da674-151">Пример</span><span class="sxs-lookup"><span data-stu-id="da674-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="da674-152">CSV</span><span class="sxs-lookup"><span data-stu-id="da674-152">CSV</span></span>

<span data-ttu-id="da674-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="da674-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="da674-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="da674-154">Request</span></span>

<span data-ttu-id="da674-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da674-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="da674-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="da674-156">Response</span></span>

<span data-ttu-id="da674-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da674-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="da674-158">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="da674-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da674-159">Языках</span><span class="sxs-lookup"><span data-stu-id="da674-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da674-160">Язык</span><span class="sxs-lookup"><span data-stu-id="da674-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="da674-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="da674-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="da674-162">JSON</span><span class="sxs-lookup"><span data-stu-id="da674-162">JSON</span></span>

<span data-ttu-id="da674-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="da674-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="da674-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="da674-164">Request</span></span>

<span data-ttu-id="da674-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da674-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="da674-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="da674-166">Response</span></span>

<span data-ttu-id="da674-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da674-167">The following is an example of the response.</span></span>

> <span data-ttu-id="da674-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da674-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailboxStorageUsedInBytes": 523143237898, 
      "siteStorageUsedInBytes": 31124384, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="da674-170">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="da674-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da674-171">Языках</span><span class="sxs-lookup"><span data-stu-id="da674-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da674-172">Язык</span><span class="sxs-lookup"><span data-stu-id="da674-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitystorage_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
