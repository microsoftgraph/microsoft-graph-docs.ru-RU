---
title: 'reportRoot: getEmailActivityUserCounts'
description: Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f1f0c807582cd3f3694779b832dad6d143b44f62
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572922"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="15c82-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="15c82-103">reportRoot: getEmailActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15c82-104">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="15c82-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="15c82-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="15c82-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="15c82-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15c82-106">Permissions</span></span>

<span data-ttu-id="15c82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15c82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15c82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15c82-109">Permission type</span></span>                        | <span data-ttu-id="15c82-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15c82-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="15c82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15c82-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="15c82-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15c82-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="15c82-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15c82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15c82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c82-114">Not supported.</span></span>                           |
| <span data-ttu-id="15c82-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15c82-115">Application</span></span>                            | <span data-ttu-id="15c82-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15c82-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="15c82-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15c82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="15c82-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="15c82-118">Function parameters</span></span>

<span data-ttu-id="15c82-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="15c82-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="15c82-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="15c82-120">Parameter</span></span> | <span data-ttu-id="15c82-121">Тип</span><span class="sxs-lookup"><span data-stu-id="15c82-121">Type</span></span>   | <span data-ttu-id="15c82-122">Описание</span><span class="sxs-lookup"><span data-stu-id="15c82-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="15c82-123">period</span><span class="sxs-lookup"><span data-stu-id="15c82-123">period</span></span>    | <span data-ttu-id="15c82-124">строка</span><span class="sxs-lookup"><span data-stu-id="15c82-124">string</span></span> | <span data-ttu-id="15c82-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="15c82-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="15c82-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="15c82-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="15c82-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="15c82-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="15c82-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15c82-128">Required.</span></span> |

<span data-ttu-id="15c82-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15c82-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="15c82-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="15c82-130">The default output type is text/csv.</span></span> <span data-ttu-id="15c82-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="15c82-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15c82-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15c82-132">Request headers</span></span>

| <span data-ttu-id="15c82-133">Имя</span><span class="sxs-lookup"><span data-stu-id="15c82-133">Name</span></span>          | <span data-ttu-id="15c82-134">Описание</span><span class="sxs-lookup"><span data-stu-id="15c82-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="15c82-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15c82-135">Authorization</span></span> | <span data-ttu-id="15c82-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15c82-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="15c82-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c82-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="15c82-139">CSV</span><span class="sxs-lookup"><span data-stu-id="15c82-139">CSV</span></span>

<span data-ttu-id="15c82-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="15c82-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="15c82-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="15c82-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="15c82-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="15c82-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="15c82-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="15c82-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="15c82-144">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="15c82-144">Report Refresh Date</span></span>
- <span data-ttu-id="15c82-145">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="15c82-145">Send</span></span>
- <span data-ttu-id="15c82-146">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="15c82-146">Receive</span></span>
- <span data-ttu-id="15c82-147">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="15c82-147">Read</span></span>
- <span data-ttu-id="15c82-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="15c82-148">Report Date</span></span>
- <span data-ttu-id="15c82-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="15c82-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="15c82-150">JSON</span><span class="sxs-lookup"><span data-stu-id="15c82-150">JSON</span></span>

<span data-ttu-id="15c82-151">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[emailActivitySummary](../resources/emailactivitysummary.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15c82-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15c82-152">Пример</span><span class="sxs-lookup"><span data-stu-id="15c82-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="15c82-153">CSV</span><span class="sxs-lookup"><span data-stu-id="15c82-153">CSV</span></span>

<span data-ttu-id="15c82-154">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="15c82-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="15c82-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="15c82-155">Request</span></span>

<span data-ttu-id="15c82-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15c82-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="15c82-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c82-157">Response</span></span>

<span data-ttu-id="15c82-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15c82-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="15c82-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="15c82-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="15c82-160">JSON</span><span class="sxs-lookup"><span data-stu-id="15c82-160">JSON</span></span>

<span data-ttu-id="15c82-161">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="15c82-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="15c82-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="15c82-162">Request</span></span>

<span data-ttu-id="15c82-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15c82-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="15c82-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c82-164">Response</span></span>

<span data-ttu-id="15c82-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15c82-165">The following is an example of the response.</span></span>

> <span data-ttu-id="15c82-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15c82-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
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
    "Error: /api-reference/beta/api/reportroot-getemailactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
