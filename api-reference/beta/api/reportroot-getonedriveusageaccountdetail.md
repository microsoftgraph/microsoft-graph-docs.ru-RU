---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Получите сведения об использовании OneDrive с разбивкой по учетным записям.
localization_priority: Normal
ms.openlocfilehash: 10bf00b66cdb387588acff61c59747de7ae70381
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818608"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="557ec-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="557ec-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

> <span data-ttu-id="557ec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="557ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="557ec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="557ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="557ec-106">Получите сведения об использовании OneDrive с разбивкой по учетным записям.</span><span class="sxs-lookup"><span data-stu-id="557ec-106">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="557ec-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="557ec-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="557ec-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="557ec-108">Permissions</span></span>

<span data-ttu-id="557ec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="557ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="557ec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="557ec-111">Permission type</span></span>                        | <span data-ttu-id="557ec-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="557ec-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="557ec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="557ec-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="557ec-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="557ec-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="557ec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="557ec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="557ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="557ec-116">Not supported.</span></span>                           |
| <span data-ttu-id="557ec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="557ec-117">Application</span></span>                            | <span data-ttu-id="557ec-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="557ec-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="557ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="557ec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="557ec-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="557ec-120">Function parameters</span></span>

<span data-ttu-id="557ec-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="557ec-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="557ec-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="557ec-122">Parameter</span></span> | <span data-ttu-id="557ec-123">Тип</span><span class="sxs-lookup"><span data-stu-id="557ec-123">Type</span></span>   | <span data-ttu-id="557ec-124">Описание</span><span class="sxs-lookup"><span data-stu-id="557ec-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="557ec-125">period</span><span class="sxs-lookup"><span data-stu-id="557ec-125">period</span></span>    | <span data-ttu-id="557ec-126">строка</span><span class="sxs-lookup"><span data-stu-id="557ec-126">string</span></span> | <span data-ttu-id="557ec-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="557ec-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="557ec-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="557ec-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="557ec-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="557ec-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="557ec-130">date</span><span class="sxs-lookup"><span data-stu-id="557ec-130">date</span></span>      | <span data-ttu-id="557ec-131">Date</span><span class="sxs-lookup"><span data-stu-id="557ec-131">Date</span></span>   | <span data-ttu-id="557ec-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="557ec-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="557ec-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="557ec-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="557ec-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="557ec-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="557ec-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="557ec-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="557ec-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="557ec-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="557ec-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="557ec-137">The default output type is text/csv.</span></span> <span data-ttu-id="557ec-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="557ec-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="557ec-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="557ec-139">Request headers</span></span>

| <span data-ttu-id="557ec-140">Имя</span><span class="sxs-lookup"><span data-stu-id="557ec-140">Name</span></span>          | <span data-ttu-id="557ec-141">Описание</span><span class="sxs-lookup"><span data-stu-id="557ec-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="557ec-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="557ec-142">Authorization</span></span> | <span data-ttu-id="557ec-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="557ec-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="557ec-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="557ec-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="557ec-146">CSV</span><span class="sxs-lookup"><span data-stu-id="557ec-146">CSV</span></span>

<span data-ttu-id="557ec-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="557ec-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="557ec-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="557ec-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="557ec-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="557ec-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="557ec-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="557ec-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="557ec-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="557ec-151">Report Refresh Date</span></span>
- <span data-ttu-id="557ec-152">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="557ec-152">Site URL</span></span>
- <span data-ttu-id="557ec-153">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="557ec-153">Owner Display Name</span></span>
- <span data-ttu-id="557ec-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="557ec-154">Is Deleted</span></span>
- <span data-ttu-id="557ec-155">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="557ec-155">Last Activity Date</span></span>
- <span data-ttu-id="557ec-156">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="557ec-156">File Count</span></span>
- <span data-ttu-id="557ec-157">Active File Count (количество активных файлов)</span><span class="sxs-lookup"><span data-stu-id="557ec-157">Active File Count</span></span>
- <span data-ttu-id="557ec-158">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="557ec-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="557ec-159">Storage Allocated (Byte) [выделено (байт)]</span><span class="sxs-lookup"><span data-stu-id="557ec-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="557ec-160">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="557ec-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="557ec-161">JSON</span><span class="sxs-lookup"><span data-stu-id="557ec-161">JSON</span></span>

<span data-ttu-id="557ec-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="557ec-162">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="557ec-163">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="557ec-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="557ec-164">Пример</span><span class="sxs-lookup"><span data-stu-id="557ec-164">Example</span></span>

<span data-ttu-id="557ec-165">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="557ec-165">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="557ec-166">CSV</span><span class="sxs-lookup"><span data-stu-id="557ec-166">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="557ec-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="557ec-167">Request</span></span>

<span data-ttu-id="557ec-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="557ec-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="557ec-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="557ec-169">Response</span></span>

<span data-ttu-id="557ec-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="557ec-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="557ec-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="557ec-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="557ec-172">JSON</span><span class="sxs-lookup"><span data-stu-id="557ec-172">JSON</span></span>

<span data-ttu-id="557ec-173">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="557ec-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="557ec-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="557ec-174">Request</span></span>

<span data-ttu-id="557ec-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="557ec-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="557ec-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="557ec-176">Response</span></span>

<span data-ttu-id="557ec-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="557ec-177">The following is an example of the response.</span></span>

> <span data-ttu-id="557ec-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="557ec-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
