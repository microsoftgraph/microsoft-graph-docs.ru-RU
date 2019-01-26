---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведения о действиях отдельных пользователей Microsoft Teams.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7ca084fbae4ca7714a207364bdf0e9f525a39ff4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576418"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="93cc1-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="93cc1-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93cc1-104">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="93cc1-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="93cc1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93cc1-105">Permissions</span></span>

<span data-ttu-id="93cc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93cc1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93cc1-108">Permission type</span></span>                        | <span data-ttu-id="93cc1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93cc1-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="93cc1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93cc1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="93cc1-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93cc1-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="93cc1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93cc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93cc1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93cc1-113">Not supported.</span></span>                           |
| <span data-ttu-id="93cc1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93cc1-114">Application</span></span>                            | <span data-ttu-id="93cc1-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93cc1-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="93cc1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93cc1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="93cc1-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="93cc1-117">Function parameters</span></span>

<span data-ttu-id="93cc1-118">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="93cc1-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="93cc1-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="93cc1-119">Parameter</span></span> | <span data-ttu-id="93cc1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="93cc1-120">Type</span></span>   | <span data-ttu-id="93cc1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="93cc1-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="93cc1-122">period</span><span class="sxs-lookup"><span data-stu-id="93cc1-122">period</span></span>    | <span data-ttu-id="93cc1-123">строка</span><span class="sxs-lookup"><span data-stu-id="93cc1-123">string</span></span> | <span data-ttu-id="93cc1-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="93cc1-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="93cc1-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="93cc1-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="93cc1-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="93cc1-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="93cc1-127">date</span><span class="sxs-lookup"><span data-stu-id="93cc1-127">date</span></span>      | <span data-ttu-id="93cc1-128">Date</span><span class="sxs-lookup"><span data-stu-id="93cc1-128">Date</span></span>   | <span data-ttu-id="93cc1-129">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="93cc1-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="93cc1-130">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="93cc1-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="93cc1-131">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="93cc1-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="93cc1-132">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="93cc1-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="93cc1-133">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="93cc1-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="93cc1-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="93cc1-134">The default output type is text/csv.</span></span> <span data-ttu-id="93cc1-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="93cc1-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93cc1-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93cc1-136">Request headers</span></span>

| <span data-ttu-id="93cc1-137">Имя</span><span class="sxs-lookup"><span data-stu-id="93cc1-137">Name</span></span>          | <span data-ttu-id="93cc1-138">Описание</span><span class="sxs-lookup"><span data-stu-id="93cc1-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="93cc1-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93cc1-139">Authorization</span></span> | <span data-ttu-id="93cc1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93cc1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="93cc1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="93cc1-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="93cc1-143">CSV</span><span class="sxs-lookup"><span data-stu-id="93cc1-143">CSV</span></span>

<span data-ttu-id="93cc1-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="93cc1-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="93cc1-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="93cc1-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="93cc1-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="93cc1-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="93cc1-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="93cc1-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="93cc1-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="93cc1-148">Report Refresh Date</span></span>
- <span data-ttu-id="93cc1-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="93cc1-149">User Principal Name</span></span>
- <span data-ttu-id="93cc1-150">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="93cc1-150">Last Activity Date</span></span>
- <span data-ttu-id="93cc1-151">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="93cc1-151">Is Deleted</span></span>
- <span data-ttu-id="93cc1-152">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="93cc1-152">Deleted Date</span></span>
- <span data-ttu-id="93cc1-153">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="93cc1-153">Assigned Products</span></span>
- <span data-ttu-id="93cc1-154">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="93cc1-154">Team Chat Message Count</span></span>
- <span data-ttu-id="93cc1-155">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="93cc1-155">Private Chat Message Count</span></span>
- <span data-ttu-id="93cc1-156">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="93cc1-156">Call Count</span></span>
- <span data-ttu-id="93cc1-157">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="93cc1-157">Meeting Count</span></span>
- <span data-ttu-id="93cc1-158">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="93cc1-158">Has Other Action</span></span>
- <span data-ttu-id="93cc1-159">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="93cc1-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="93cc1-160">JSON</span><span class="sxs-lookup"><span data-stu-id="93cc1-160">JSON</span></span>

<span data-ttu-id="93cc1-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93cc1-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="93cc1-162">Размер страницы по умолчанию для этого запроса — 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="93cc1-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="93cc1-163">Пример</span><span class="sxs-lookup"><span data-stu-id="93cc1-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="93cc1-164">CSV</span><span class="sxs-lookup"><span data-stu-id="93cc1-164">CSV</span></span>

<span data-ttu-id="93cc1-165">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="93cc1-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="93cc1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="93cc1-166">Request</span></span>

<span data-ttu-id="93cc1-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93cc1-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="93cc1-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="93cc1-168">Response</span></span>

<span data-ttu-id="93cc1-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93cc1-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="93cc1-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="93cc1-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="93cc1-171">JSON</span><span class="sxs-lookup"><span data-stu-id="93cc1-171">JSON</span></span>

<span data-ttu-id="93cc1-172">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="93cc1-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="93cc1-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="93cc1-173">Request</span></span>

<span data-ttu-id="93cc1-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93cc1-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="93cc1-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="93cc1-175">Response</span></span>

<span data-ttu-id="93cc1-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93cc1-176">The following is an example of the response.</span></span>

> <span data-ttu-id="93cc1-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93cc1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
