---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b8e52b5a5256e307f721c575bebc7932daf800f3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575823"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="31638-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="31638-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31638-104">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="31638-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="31638-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="31638-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="31638-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31638-106">Permissions</span></span>

<span data-ttu-id="31638-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31638-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31638-109">Permission type</span></span>                        | <span data-ttu-id="31638-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31638-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="31638-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31638-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31638-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31638-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="31638-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31638-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31638-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31638-114">Not supported.</span></span>                           |
| <span data-ttu-id="31638-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31638-115">Application</span></span>                            | <span data-ttu-id="31638-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31638-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="31638-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31638-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="31638-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="31638-118">Function parameters</span></span>

<span data-ttu-id="31638-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="31638-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="31638-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="31638-120">Parameter</span></span> | <span data-ttu-id="31638-121">Тип</span><span class="sxs-lookup"><span data-stu-id="31638-121">Type</span></span>   | <span data-ttu-id="31638-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31638-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="31638-123">period</span><span class="sxs-lookup"><span data-stu-id="31638-123">period</span></span>    | <span data-ttu-id="31638-124">строка</span><span class="sxs-lookup"><span data-stu-id="31638-124">string</span></span> | <span data-ttu-id="31638-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="31638-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="31638-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="31638-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="31638-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="31638-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="31638-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31638-128">Required.</span></span> |

<span data-ttu-id="31638-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31638-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="31638-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="31638-130">The default output type is text/csv.</span></span> <span data-ttu-id="31638-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="31638-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31638-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31638-132">Request headers</span></span>

| <span data-ttu-id="31638-133">Имя</span><span class="sxs-lookup"><span data-stu-id="31638-133">Name</span></span>          | <span data-ttu-id="31638-134">Описание</span><span class="sxs-lookup"><span data-stu-id="31638-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="31638-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31638-135">Authorization</span></span> | <span data-ttu-id="31638-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31638-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="31638-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="31638-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="31638-139">CSV</span><span class="sxs-lookup"><span data-stu-id="31638-139">CSV</span></span>

<span data-ttu-id="31638-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="31638-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="31638-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="31638-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="31638-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="31638-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="31638-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="31638-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="31638-144">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="31638-144">Report Refresh Date</span></span>
- <span data-ttu-id="31638-145">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="31638-145">Outlook 2016</span></span>
- <span data-ttu-id="31638-146">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="31638-146">Outlook 2013</span></span>
- <span data-ttu-id="31638-147">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="31638-147">Outlook 2010</span></span>
- <span data-ttu-id="31638-148">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="31638-148">Outlook 2007</span></span>
- <span data-ttu-id="31638-149">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="31638-149">Undetermined</span></span>
- <span data-ttu-id="31638-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="31638-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="31638-151">JSON</span><span class="sxs-lookup"><span data-stu-id="31638-151">JSON</span></span>

<span data-ttu-id="31638-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="31638-152">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31638-153">Пример</span><span class="sxs-lookup"><span data-stu-id="31638-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="31638-154">CSV</span><span class="sxs-lookup"><span data-stu-id="31638-154">CSV</span></span>

<span data-ttu-id="31638-155">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="31638-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="31638-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="31638-156">Request</span></span>

<span data-ttu-id="31638-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31638-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="31638-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="31638-158">Response</span></span>

<span data-ttu-id="31638-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31638-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="31638-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="31638-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="31638-161">JSON</span><span class="sxs-lookup"><span data-stu-id="31638-161">JSON</span></span>

<span data-ttu-id="31638-162">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="31638-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="31638-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="31638-163">Request</span></span>

<span data-ttu-id="31638-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31638-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="31638-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="31638-165">Response</span></span>

<span data-ttu-id="31638-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31638-166">The following is an example of the response.</span></span>

> <span data-ttu-id="31638-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31638-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailappusageversionsusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
