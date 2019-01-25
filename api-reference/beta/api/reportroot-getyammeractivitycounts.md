---
title: 'reportRoot: getYammerActivityCounts'
description: Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0204c0ea634f8793d2f0ab58fdffc8c389443eed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514721"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="36e5b-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="36e5b-103">reportRoot: getYammerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e5b-104">Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="36e5b-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="36e5b-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="36e5b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="36e5b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36e5b-106">Permissions</span></span>

<span data-ttu-id="36e5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36e5b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36e5b-109">Permission type</span></span>                        | <span data-ttu-id="36e5b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36e5b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="36e5b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36e5b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36e5b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e5b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="36e5b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36e5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36e5b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e5b-114">Not supported.</span></span>                           |
| <span data-ttu-id="36e5b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36e5b-115">Application</span></span>                            | <span data-ttu-id="36e5b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e5b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="36e5b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36e5b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="36e5b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="36e5b-118">Function parameters</span></span>

<span data-ttu-id="36e5b-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="36e5b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="36e5b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="36e5b-120">Parameter</span></span> | <span data-ttu-id="36e5b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="36e5b-121">Type</span></span>   | <span data-ttu-id="36e5b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="36e5b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="36e5b-123">period</span><span class="sxs-lookup"><span data-stu-id="36e5b-123">period</span></span>    | <span data-ttu-id="36e5b-124">строка</span><span class="sxs-lookup"><span data-stu-id="36e5b-124">string</span></span> | <span data-ttu-id="36e5b-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="36e5b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="36e5b-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="36e5b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="36e5b-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="36e5b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="36e5b-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36e5b-128">Required.</span></span> |

<span data-ttu-id="36e5b-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="36e5b-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="36e5b-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="36e5b-130">The default output type is text/csv.</span></span> <span data-ttu-id="36e5b-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="36e5b-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36e5b-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36e5b-132">Request headers</span></span>

| <span data-ttu-id="36e5b-133">Имя</span><span class="sxs-lookup"><span data-stu-id="36e5b-133">Name</span></span>          | <span data-ttu-id="36e5b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="36e5b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="36e5b-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36e5b-135">Authorization</span></span> | <span data-ttu-id="36e5b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36e5b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="36e5b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="36e5b-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="36e5b-139">CSV</span><span class="sxs-lookup"><span data-stu-id="36e5b-139">CSV</span></span>

<span data-ttu-id="36e5b-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="36e5b-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="36e5b-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="36e5b-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="36e5b-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="36e5b-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="36e5b-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="36e5b-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="36e5b-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="36e5b-144">Report Refresh Date</span></span>
- <span data-ttu-id="36e5b-145">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="36e5b-145">Liked</span></span>
- <span data-ttu-id="36e5b-146">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="36e5b-146">Posted</span></span>
- <span data-ttu-id="36e5b-147">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="36e5b-147">Read</span></span>
- <span data-ttu-id="36e5b-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="36e5b-148">Report Date</span></span>
- <span data-ttu-id="36e5b-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="36e5b-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="36e5b-150">JSON</span><span class="sxs-lookup"><span data-stu-id="36e5b-150">JSON</span></span>

<span data-ttu-id="36e5b-151">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerActivitySummary](../resources/yammeractivitysummary.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36e5b-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e5b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="36e5b-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="36e5b-153">CSV</span><span class="sxs-lookup"><span data-stu-id="36e5b-153">CSV</span></span>

<span data-ttu-id="36e5b-154">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="36e5b-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="36e5b-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e5b-155">Request</span></span>

<span data-ttu-id="36e5b-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36e5b-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="36e5b-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="36e5b-157">Response</span></span>

<span data-ttu-id="36e5b-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36e5b-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="36e5b-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="36e5b-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="36e5b-160">JSON</span><span class="sxs-lookup"><span data-stu-id="36e5b-160">JSON</span></span>

<span data-ttu-id="36e5b-161">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="36e5b-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="36e5b-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e5b-162">Request</span></span>

<span data-ttu-id="36e5b-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36e5b-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="36e5b-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="36e5b-164">Response</span></span>

<span data-ttu-id="36e5b-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36e5b-165">The following is an example of the response.</span></span>

> <span data-ttu-id="36e5b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36e5b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
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
    "Error: /api-reference/beta/api/reportroot-getyammeractivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
