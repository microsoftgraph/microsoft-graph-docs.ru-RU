---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0c1fa1bf6f42b7fb24d1a4a7db7c50ad4431e8b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545935"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="cb129-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="cb129-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb129-104">Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны.</span><span class="sxs-lookup"><span data-stu-id="cb129-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="cb129-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="cb129-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb129-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb129-106">Permissions</span></span>

<span data-ttu-id="cb129-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb129-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb129-109">Permission type</span></span>                        | <span data-ttu-id="cb129-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb129-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cb129-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb129-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb129-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb129-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cb129-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb129-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb129-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb129-114">Not supported.</span></span>                           |
| <span data-ttu-id="cb129-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb129-115">Application</span></span>                            | <span data-ttu-id="cb129-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb129-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cb129-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb129-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cb129-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cb129-118">Function parameters</span></span>

<span data-ttu-id="cb129-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cb129-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cb129-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="cb129-120">Parameter</span></span> | <span data-ttu-id="cb129-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cb129-121">Type</span></span>   | <span data-ttu-id="cb129-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cb129-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cb129-123">period</span><span class="sxs-lookup"><span data-stu-id="cb129-123">period</span></span>    | <span data-ttu-id="cb129-124">string</span><span class="sxs-lookup"><span data-stu-id="cb129-124">string</span></span> | <span data-ttu-id="cb129-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cb129-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cb129-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="cb129-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cb129-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cb129-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cb129-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb129-128">Required.</span></span> |

<span data-ttu-id="cb129-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cb129-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cb129-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="cb129-130">The default output type is text/csv.</span></span> <span data-ttu-id="cb129-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="cb129-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb129-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb129-132">Request headers</span></span>

| <span data-ttu-id="cb129-133">Имя</span><span class="sxs-lookup"><span data-stu-id="cb129-133">Name</span></span>          | <span data-ttu-id="cb129-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cb129-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cb129-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb129-135">Authorization</span></span> | <span data-ttu-id="cb129-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb129-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cb129-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb129-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cb129-139">CSV</span><span class="sxs-lookup"><span data-stu-id="cb129-139">CSV</span></span>

<span data-ttu-id="cb129-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cb129-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cb129-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cb129-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cb129-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cb129-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cb129-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cb129-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cb129-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cb129-144">Report Refresh Date</span></span>
- <span data-ttu-id="cb129-145">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="cb129-145">Total</span></span>
- <span data-ttu-id="cb129-146">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="cb129-146">Active</span></span>
- <span data-ttu-id="cb129-147">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="cb129-147">Report Date</span></span>
- <span data-ttu-id="cb129-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="cb129-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cb129-149">JSON</span><span class="sxs-lookup"><span data-stu-id="cb129-149">JSON</span></span>

<span data-ttu-id="cb129-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb129-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb129-151">Пример</span><span class="sxs-lookup"><span data-stu-id="cb129-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cb129-152">CSV</span><span class="sxs-lookup"><span data-stu-id="cb129-152">CSV</span></span>

<span data-ttu-id="cb129-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="cb129-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cb129-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb129-154">Request</span></span>

<span data-ttu-id="cb129-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb129-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cb129-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb129-156">Response</span></span>

<span data-ttu-id="cb129-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb129-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cb129-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cb129-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="cb129-159">JSON</span><span class="sxs-lookup"><span data-stu-id="cb129-159">JSON</span></span>

<span data-ttu-id="cb129-160">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="cb129-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cb129-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb129-161">Request</span></span>

<span data-ttu-id="cb129-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb129-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cb129-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb129-163">Response</span></span>

<span data-ttu-id="cb129-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb129-164">The following is an example of the response.</span></span>

> <span data-ttu-id="cb129-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb129-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 26, 
      "active": 5, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
