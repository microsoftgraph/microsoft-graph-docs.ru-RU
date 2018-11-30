---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Получение сведений об использовании сайтов SharePoint.
ms.openlocfilehash: 58c51bfcc14f3478a53c45f66f64ce7dc547ea6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079558"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="56423-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="56423-103">reportRoot: getSharePointSiteUsageDetail</span></span>

> <span data-ttu-id="56423-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56423-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56423-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56423-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56423-106">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="56423-106">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="56423-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="56423-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="56423-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56423-108">Permissions</span></span>

<span data-ttu-id="56423-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56423-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56423-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56423-111">Permission type</span></span>                        | <span data-ttu-id="56423-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56423-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="56423-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56423-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="56423-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="56423-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="56423-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56423-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56423-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56423-116">Not supported.</span></span>                           |
| <span data-ttu-id="56423-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56423-117">Application</span></span>                            | <span data-ttu-id="56423-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="56423-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="56423-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56423-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="56423-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="56423-120">Function parameters</span></span>

<span data-ttu-id="56423-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="56423-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="56423-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="56423-122">Parameter</span></span> | <span data-ttu-id="56423-123">Тип</span><span class="sxs-lookup"><span data-stu-id="56423-123">Type</span></span>   | <span data-ttu-id="56423-124">Описание</span><span class="sxs-lookup"><span data-stu-id="56423-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="56423-125">period</span><span class="sxs-lookup"><span data-stu-id="56423-125">period</span></span>    | <span data-ttu-id="56423-126">строка</span><span class="sxs-lookup"><span data-stu-id="56423-126">string</span></span> | <span data-ttu-id="56423-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="56423-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="56423-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="56423-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="56423-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="56423-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="56423-130">date</span><span class="sxs-lookup"><span data-stu-id="56423-130">date</span></span>      | <span data-ttu-id="56423-131">Date</span><span class="sxs-lookup"><span data-stu-id="56423-131">Date</span></span>   | <span data-ttu-id="56423-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="56423-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="56423-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="56423-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="56423-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="56423-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="56423-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="56423-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="56423-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56423-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="56423-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="56423-137">The default output type is text/csv.</span></span> <span data-ttu-id="56423-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="56423-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56423-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56423-139">Request headers</span></span>

| <span data-ttu-id="56423-140">Имя</span><span class="sxs-lookup"><span data-stu-id="56423-140">Name</span></span>          | <span data-ttu-id="56423-141">Описание</span><span class="sxs-lookup"><span data-stu-id="56423-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="56423-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56423-142">Authorization</span></span> | <span data-ttu-id="56423-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56423-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="56423-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="56423-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="56423-146">CSV</span><span class="sxs-lookup"><span data-stu-id="56423-146">CSV</span></span>

<span data-ttu-id="56423-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="56423-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="56423-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="56423-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="56423-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="56423-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="56423-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="56423-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="56423-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="56423-151">Report Refresh Date</span></span>
- <span data-ttu-id="56423-152">Идентификатор сайта</span><span class="sxs-lookup"><span data-stu-id="56423-152">Site Id</span></span>
- <span data-ttu-id="56423-153">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="56423-153">Site URL</span></span>
- <span data-ttu-id="56423-154">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="56423-154">Owner Display Name</span></span>
- <span data-ttu-id="56423-155">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="56423-155">Is Deleted</span></span>
- <span data-ttu-id="56423-156">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="56423-156">Last Activity Date</span></span>
- <span data-ttu-id="56423-157">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="56423-157">File Count</span></span>
- <span data-ttu-id="56423-158">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="56423-158">Active File Count</span></span>
- <span data-ttu-id="56423-159">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="56423-159">Page View Count</span></span>
- <span data-ttu-id="56423-160">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="56423-160">Visited Page Count</span></span>
- <span data-ttu-id="56423-161">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="56423-161">Storage Used (Byte)</span></span>
- <span data-ttu-id="56423-162">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="56423-162">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="56423-163">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="56423-163">Root Web Template</span></span>
- <span data-ttu-id="56423-164">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="56423-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="56423-165">JSON</span><span class="sxs-lookup"><span data-stu-id="56423-165">JSON</span></span>

<span data-ttu-id="56423-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56423-166">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="56423-167">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="56423-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="56423-168">Пример</span><span class="sxs-lookup"><span data-stu-id="56423-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="56423-169">CSV</span><span class="sxs-lookup"><span data-stu-id="56423-169">CSV</span></span>

<span data-ttu-id="56423-170">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="56423-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="56423-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="56423-171">Request</span></span>

<span data-ttu-id="56423-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56423-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="56423-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="56423-173">Response</span></span>

<span data-ttu-id="56423-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56423-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="56423-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="56423-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```

### <a name="json"></a><span data-ttu-id="56423-176">JSON</span><span class="sxs-lookup"><span data-stu-id="56423-176">JSON</span></span>

<span data-ttu-id="56423-177">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="56423-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="56423-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="56423-178">Request</span></span>

<span data-ttu-id="56423-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56423-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="56423-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="56423-180">Response</span></span>

<span data-ttu-id="56423-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56423-181">The following is an example of the response.</span></span>

> <span data-ttu-id="56423-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56423-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
      "reportPeriod": "7"
    }
  ]
}
```
