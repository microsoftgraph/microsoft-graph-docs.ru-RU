---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведения о действиях отдельных пользователей Microsoft Teams.
localization_priority: Normal
ms.openlocfilehash: 7c007acc9988db8dc9e4e7bfdf2440178b1ca445
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815339"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="6880b-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6880b-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

> <span data-ttu-id="6880b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6880b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6880b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6880b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6880b-106">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6880b-106">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="6880b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6880b-107">Permissions</span></span>

<span data-ttu-id="6880b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6880b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6880b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6880b-110">Permission type</span></span>                        | <span data-ttu-id="6880b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6880b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6880b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6880b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6880b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6880b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6880b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6880b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6880b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6880b-115">Not supported.</span></span>                           |
| <span data-ttu-id="6880b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6880b-116">Application</span></span>                            | <span data-ttu-id="6880b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6880b-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6880b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6880b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="6880b-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="6880b-119">Function parameters</span></span>

<span data-ttu-id="6880b-120">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6880b-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6880b-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="6880b-121">Parameter</span></span> | <span data-ttu-id="6880b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6880b-122">Type</span></span>   | <span data-ttu-id="6880b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6880b-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6880b-124">period</span><span class="sxs-lookup"><span data-stu-id="6880b-124">period</span></span>    | <span data-ttu-id="6880b-125">строка</span><span class="sxs-lookup"><span data-stu-id="6880b-125">string</span></span> | <span data-ttu-id="6880b-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6880b-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6880b-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6880b-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6880b-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6880b-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6880b-129">date</span><span class="sxs-lookup"><span data-stu-id="6880b-129">date</span></span>      | <span data-ttu-id="6880b-130">Date</span><span class="sxs-lookup"><span data-stu-id="6880b-130">Date</span></span>   | <span data-ttu-id="6880b-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="6880b-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6880b-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="6880b-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6880b-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="6880b-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6880b-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="6880b-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="6880b-135">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6880b-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6880b-136">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="6880b-136">The default output type is text/csv.</span></span> <span data-ttu-id="6880b-137">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="6880b-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6880b-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6880b-138">Request headers</span></span>

| <span data-ttu-id="6880b-139">Имя</span><span class="sxs-lookup"><span data-stu-id="6880b-139">Name</span></span>          | <span data-ttu-id="6880b-140">Описание</span><span class="sxs-lookup"><span data-stu-id="6880b-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6880b-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6880b-141">Authorization</span></span> | <span data-ttu-id="6880b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6880b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6880b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="6880b-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6880b-145">CSV</span><span class="sxs-lookup"><span data-stu-id="6880b-145">CSV</span></span>

<span data-ttu-id="6880b-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6880b-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6880b-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6880b-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6880b-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6880b-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6880b-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6880b-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6880b-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6880b-150">Report Refresh Date</span></span>
- <span data-ttu-id="6880b-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="6880b-151">User Principal Name</span></span>
- <span data-ttu-id="6880b-152">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="6880b-152">Last Activity Date</span></span>
- <span data-ttu-id="6880b-153">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="6880b-153">Is Deleted</span></span>
- <span data-ttu-id="6880b-154">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="6880b-154">Deleted Date</span></span>
- <span data-ttu-id="6880b-155">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="6880b-155">Assigned Products</span></span>
- <span data-ttu-id="6880b-156">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="6880b-156">Team Chat Message Count</span></span>
- <span data-ttu-id="6880b-157">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="6880b-157">Private Chat Message Count</span></span>
- <span data-ttu-id="6880b-158">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="6880b-158">Call Count</span></span>
- <span data-ttu-id="6880b-159">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="6880b-159">Meeting Count</span></span>
- <span data-ttu-id="6880b-160">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="6880b-160">Has Other Action</span></span>
- <span data-ttu-id="6880b-161">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6880b-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6880b-162">JSON</span><span class="sxs-lookup"><span data-stu-id="6880b-162">JSON</span></span>

<span data-ttu-id="6880b-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6880b-163">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="6880b-164">Размер страницы по умолчанию для этого запроса — 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6880b-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="6880b-165">Пример</span><span class="sxs-lookup"><span data-stu-id="6880b-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6880b-166">CSV</span><span class="sxs-lookup"><span data-stu-id="6880b-166">CSV</span></span>

<span data-ttu-id="6880b-167">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="6880b-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6880b-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6880b-168">Request</span></span>

<span data-ttu-id="6880b-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6880b-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6880b-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="6880b-170">Response</span></span>

<span data-ttu-id="6880b-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6880b-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6880b-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6880b-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="6880b-173">JSON</span><span class="sxs-lookup"><span data-stu-id="6880b-173">JSON</span></span>

<span data-ttu-id="6880b-174">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="6880b-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6880b-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="6880b-175">Request</span></span>

<span data-ttu-id="6880b-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6880b-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6880b-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="6880b-177">Response</span></span>

<span data-ttu-id="6880b-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6880b-178">The following is an example of the response.</span></span>

> <span data-ttu-id="6880b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6880b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
