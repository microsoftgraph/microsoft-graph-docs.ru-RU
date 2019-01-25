---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0e24a66905afa0ccb20c30fb4414e621cb4a1683
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522282"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="36914-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="36914-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36914-104">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="36914-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="36914-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36914-105">Permissions</span></span>

<span data-ttu-id="36914-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36914-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36914-108">Permission type</span></span>                        | <span data-ttu-id="36914-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36914-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="36914-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36914-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="36914-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36914-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="36914-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36914-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36914-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36914-113">Not supported.</span></span>                           |
| <span data-ttu-id="36914-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36914-114">Application</span></span>                            | <span data-ttu-id="36914-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36914-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="36914-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36914-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="36914-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="36914-117">Function parameters</span></span>

<span data-ttu-id="36914-118">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="36914-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="36914-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="36914-119">Parameter</span></span> | <span data-ttu-id="36914-120">Тип</span><span class="sxs-lookup"><span data-stu-id="36914-120">Type</span></span>   | <span data-ttu-id="36914-121">Описание</span><span class="sxs-lookup"><span data-stu-id="36914-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="36914-122">period</span><span class="sxs-lookup"><span data-stu-id="36914-122">period</span></span>    | <span data-ttu-id="36914-123">строка</span><span class="sxs-lookup"><span data-stu-id="36914-123">string</span></span> | <span data-ttu-id="36914-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="36914-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="36914-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="36914-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="36914-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="36914-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="36914-127">date</span><span class="sxs-lookup"><span data-stu-id="36914-127">date</span></span>      | <span data-ttu-id="36914-128">Date</span><span class="sxs-lookup"><span data-stu-id="36914-128">Date</span></span>   | <span data-ttu-id="36914-129">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="36914-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="36914-130">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="36914-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="36914-131">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="36914-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="36914-132">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="36914-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="36914-133">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="36914-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="36914-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="36914-134">The default output type is text/csv.</span></span> <span data-ttu-id="36914-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="36914-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36914-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36914-136">Request headers</span></span>

| <span data-ttu-id="36914-137">Имя</span><span class="sxs-lookup"><span data-stu-id="36914-137">Name</span></span>          | <span data-ttu-id="36914-138">Описание</span><span class="sxs-lookup"><span data-stu-id="36914-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="36914-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36914-139">Authorization</span></span> | <span data-ttu-id="36914-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36914-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="36914-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="36914-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="36914-143">CSV</span><span class="sxs-lookup"><span data-stu-id="36914-143">CSV</span></span>

<span data-ttu-id="36914-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="36914-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="36914-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="36914-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="36914-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="36914-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="36914-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="36914-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="36914-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="36914-148">Report Refresh Date</span></span>
- <span data-ttu-id="36914-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="36914-149">User Principal Name</span></span>
- <span data-ttu-id="36914-150">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="36914-150">Last Activity Date</span></span>
- <span data-ttu-id="36914-151">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="36914-151">Is Deleted</span></span>
- <span data-ttu-id="36914-152">Deleted Date (дата удаления);</span><span class="sxs-lookup"><span data-stu-id="36914-152">Deleted Date</span></span>
- <span data-ttu-id="36914-153">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="36914-153">Used Web</span></span>
- <span data-ttu-id="36914-154">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="36914-154">Used Windows Phone</span></span>
- <span data-ttu-id="36914-155">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="36914-155">Used iOS</span></span>
- <span data-ttu-id="36914-156">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="36914-156">Used Mac</span></span>
- <span data-ttu-id="36914-157">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="36914-157">Used Android Phone</span></span>
- <span data-ttu-id="36914-158">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="36914-158">Used Windows</span></span>
- <span data-ttu-id="36914-159">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="36914-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="36914-160">JSON</span><span class="sxs-lookup"><span data-stu-id="36914-160">JSON</span></span>

<span data-ttu-id="36914-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36914-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="36914-162">Размер страницы по умолчанию для этого запроса — 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="36914-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="36914-163">Пример</span><span class="sxs-lookup"><span data-stu-id="36914-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="36914-164">CSV</span><span class="sxs-lookup"><span data-stu-id="36914-164">CSV</span></span>

<span data-ttu-id="36914-165">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="36914-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="36914-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="36914-166">Request</span></span>

<span data-ttu-id="36914-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36914-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="36914-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="36914-168">Response</span></span>

<span data-ttu-id="36914-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36914-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="36914-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="36914-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="36914-171">JSON</span><span class="sxs-lookup"><span data-stu-id="36914-171">JSON</span></span>

<span data-ttu-id="36914-172">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="36914-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="36914-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="36914-173">Request</span></span>

<span data-ttu-id="36914-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36914-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="36914-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="36914-175">Response</span></span>

<span data-ttu-id="36914-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36914-176">The following is an example of the response.</span></span>

> <span data-ttu-id="36914-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36914-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
