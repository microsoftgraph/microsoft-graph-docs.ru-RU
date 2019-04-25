---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 76b489a4ceb1fb721ec7ebb4d8892e6e11fc53d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538144"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="88b0b-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="88b0b-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88b0b-105">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="88b0b-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="88b0b-106">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="88b0b-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="88b0b-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="88b0b-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="88b0b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88b0b-108">Permissions</span></span>

<span data-ttu-id="88b0b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88b0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88b0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88b0b-111">Permission type</span></span>                        | <span data-ttu-id="88b0b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88b0b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="88b0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88b0b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="88b0b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88b0b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="88b0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88b0b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88b0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88b0b-116">Not supported.</span></span>                           |
| <span data-ttu-id="88b0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88b0b-117">Application</span></span>                            | <span data-ttu-id="88b0b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88b0b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="88b0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88b0b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="88b0b-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="88b0b-120">Function parameters</span></span>

<span data-ttu-id="88b0b-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="88b0b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="88b0b-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="88b0b-122">Parameter</span></span> | <span data-ttu-id="88b0b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="88b0b-123">Type</span></span>   | <span data-ttu-id="88b0b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="88b0b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="88b0b-125">period</span><span class="sxs-lookup"><span data-stu-id="88b0b-125">period</span></span>    | <span data-ttu-id="88b0b-126">string</span><span class="sxs-lookup"><span data-stu-id="88b0b-126">string</span></span> | <span data-ttu-id="88b0b-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="88b0b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="88b0b-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="88b0b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="88b0b-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="88b0b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="88b0b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88b0b-130">Required.</span></span> |

<span data-ttu-id="88b0b-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="88b0b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="88b0b-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="88b0b-132">The default output type is text/csv.</span></span> <span data-ttu-id="88b0b-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="88b0b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88b0b-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88b0b-134">Request headers</span></span>

| <span data-ttu-id="88b0b-135">Имя</span><span class="sxs-lookup"><span data-stu-id="88b0b-135">Name</span></span>          | <span data-ttu-id="88b0b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="88b0b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="88b0b-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88b0b-137">Authorization</span></span> | <span data-ttu-id="88b0b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88b0b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="88b0b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="88b0b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="88b0b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="88b0b-141">CSV</span></span>

<span data-ttu-id="88b0b-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="88b0b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="88b0b-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="88b0b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="88b0b-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="88b0b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="88b0b-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="88b0b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="88b0b-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="88b0b-146">Report Refresh Date</span></span>
- <span data-ttu-id="88b0b-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="88b0b-147">Site Type</span></span>
- <span data-ttu-id="88b0b-148">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="88b0b-148">Total</span></span>
- <span data-ttu-id="88b0b-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="88b0b-149">Active</span></span>
- <span data-ttu-id="88b0b-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="88b0b-150">Report Date</span></span>
- <span data-ttu-id="88b0b-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="88b0b-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="88b0b-152">JSON</span><span class="sxs-lookup"><span data-stu-id="88b0b-152">JSON</span></span>

<span data-ttu-id="88b0b-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажеаккаунткаунтс](../resources/onedriveusageaccountcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88b0b-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88b0b-154">Пример</span><span class="sxs-lookup"><span data-stu-id="88b0b-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="88b0b-155">CSV</span><span class="sxs-lookup"><span data-stu-id="88b0b-155">CSV</span></span>

<span data-ttu-id="88b0b-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="88b0b-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="88b0b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="88b0b-157">Request</span></span>

<span data-ttu-id="88b0b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88b0b-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="88b0b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="88b0b-159">Response</span></span>

<span data-ttu-id="88b0b-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88b0b-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="88b0b-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="88b0b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="88b0b-162">JSON</span><span class="sxs-lookup"><span data-stu-id="88b0b-162">JSON</span></span>

<span data-ttu-id="88b0b-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="88b0b-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="88b0b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="88b0b-164">Request</span></span>

<span data-ttu-id="88b0b-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88b0b-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="88b0b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="88b0b-166">Response</span></span>

<span data-ttu-id="88b0b-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88b0b-167">The following is an example of the response.</span></span>

> <span data-ttu-id="88b0b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88b0b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
