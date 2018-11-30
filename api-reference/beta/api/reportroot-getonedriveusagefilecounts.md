---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
ms.openlocfilehash: 5b67166cb6019154e6238b7307f622fed361350a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080409"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="3fc86-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="3fc86-104">reportRoot: getOneDriveUsageFileCounts</span></span>

> <span data-ttu-id="3fc86-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3fc86-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fc86-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fc86-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3fc86-107">Получение общего количества файлов на всех сайтах и количества активных файлов.</span><span class="sxs-lookup"><span data-stu-id="3fc86-107">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="3fc86-108">Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="3fc86-108">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="3fc86-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="3fc86-109">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="3fc86-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fc86-110">Permissions</span></span>

<span data-ttu-id="3fc86-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fc86-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fc86-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fc86-113">Permission type</span></span>                        | <span data-ttu-id="3fc86-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fc86-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3fc86-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fc86-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="3fc86-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fc86-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3fc86-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fc86-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fc86-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fc86-118">Not supported.</span></span>                           |
| <span data-ttu-id="3fc86-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fc86-119">Application</span></span>                            | <span data-ttu-id="3fc86-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fc86-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3fc86-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fc86-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3fc86-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="3fc86-122">Function parameters</span></span>

<span data-ttu-id="3fc86-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3fc86-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3fc86-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="3fc86-124">Parameter</span></span> | <span data-ttu-id="3fc86-125">Тип</span><span class="sxs-lookup"><span data-stu-id="3fc86-125">Type</span></span>   | <span data-ttu-id="3fc86-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc86-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3fc86-127">period</span><span class="sxs-lookup"><span data-stu-id="3fc86-127">period</span></span>    | <span data-ttu-id="3fc86-128">строка</span><span class="sxs-lookup"><span data-stu-id="3fc86-128">string</span></span> | <span data-ttu-id="3fc86-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3fc86-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3fc86-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3fc86-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3fc86-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3fc86-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3fc86-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fc86-132">Required.</span></span> |

<span data-ttu-id="3fc86-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3fc86-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3fc86-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="3fc86-134">The default output type is text/csv.</span></span> <span data-ttu-id="3fc86-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="3fc86-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fc86-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fc86-136">Request headers</span></span>

| <span data-ttu-id="3fc86-137">Имя</span><span class="sxs-lookup"><span data-stu-id="3fc86-137">Name</span></span>          | <span data-ttu-id="3fc86-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc86-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3fc86-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fc86-139">Authorization</span></span> | <span data-ttu-id="3fc86-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fc86-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3fc86-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fc86-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3fc86-143">CSV</span><span class="sxs-lookup"><span data-stu-id="3fc86-143">CSV</span></span>

<span data-ttu-id="3fc86-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3fc86-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3fc86-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3fc86-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3fc86-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3fc86-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3fc86-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3fc86-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3fc86-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3fc86-148">Report Refresh Date</span></span>
- <span data-ttu-id="3fc86-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="3fc86-149">Site Type</span></span>
- <span data-ttu-id="3fc86-150">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="3fc86-150">Total</span></span>
- <span data-ttu-id="3fc86-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="3fc86-151">Active</span></span>
- <span data-ttu-id="3fc86-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3fc86-152">Report Date</span></span>
- <span data-ttu-id="3fc86-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3fc86-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3fc86-154">JSON</span><span class="sxs-lookup"><span data-stu-id="3fc86-154">JSON</span></span>

<span data-ttu-id="3fc86-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3fc86-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fc86-156">Пример</span><span class="sxs-lookup"><span data-stu-id="3fc86-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3fc86-157">CSV</span><span class="sxs-lookup"><span data-stu-id="3fc86-157">CSV</span></span>

<span data-ttu-id="3fc86-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="3fc86-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3fc86-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fc86-159">Request</span></span>

<span data-ttu-id="3fc86-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fc86-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3fc86-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fc86-161">Response</span></span>

<span data-ttu-id="3fc86-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3fc86-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3fc86-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3fc86-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3fc86-164">JSON</span><span class="sxs-lookup"><span data-stu-id="3fc86-164">JSON</span></span>

<span data-ttu-id="3fc86-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3fc86-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3fc86-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fc86-166">Request</span></span>

<span data-ttu-id="3fc86-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fc86-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3fc86-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fc86-168">Response</span></span>

<span data-ttu-id="3fc86-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3fc86-169">The following is an example of the response.</span></span>

> <span data-ttu-id="3fc86-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fc86-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 297960, 
      "active": 4679, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
