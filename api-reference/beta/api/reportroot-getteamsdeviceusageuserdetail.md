---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.openlocfilehash: ade8bbcd2ce680bb7103bd0e9dbb09f3d49d1b03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842212"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="58b43-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="58b43-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

> <span data-ttu-id="58b43-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58b43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58b43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58b43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58b43-106">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="58b43-106">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="58b43-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58b43-107">Permissions</span></span>

<span data-ttu-id="58b43-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58b43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58b43-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58b43-110">Permission type</span></span>                        | <span data-ttu-id="58b43-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58b43-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="58b43-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58b43-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="58b43-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58b43-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="58b43-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58b43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58b43-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58b43-115">Not supported.</span></span>                           |
| <span data-ttu-id="58b43-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58b43-116">Application</span></span>                            | <span data-ttu-id="58b43-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58b43-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="58b43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58b43-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="58b43-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="58b43-119">Function parameters</span></span>

<span data-ttu-id="58b43-120">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="58b43-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="58b43-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="58b43-121">Parameter</span></span> | <span data-ttu-id="58b43-122">Тип</span><span class="sxs-lookup"><span data-stu-id="58b43-122">Type</span></span>   | <span data-ttu-id="58b43-123">Описание</span><span class="sxs-lookup"><span data-stu-id="58b43-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="58b43-124">period</span><span class="sxs-lookup"><span data-stu-id="58b43-124">period</span></span>    | <span data-ttu-id="58b43-125">строка</span><span class="sxs-lookup"><span data-stu-id="58b43-125">string</span></span> | <span data-ttu-id="58b43-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="58b43-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="58b43-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="58b43-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="58b43-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="58b43-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="58b43-129">date</span><span class="sxs-lookup"><span data-stu-id="58b43-129">date</span></span>      | <span data-ttu-id="58b43-130">Date</span><span class="sxs-lookup"><span data-stu-id="58b43-130">Date</span></span>   | <span data-ttu-id="58b43-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="58b43-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="58b43-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="58b43-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="58b43-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="58b43-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="58b43-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="58b43-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="58b43-135">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58b43-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="58b43-136">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="58b43-136">The default output type is text/csv.</span></span> <span data-ttu-id="58b43-137">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="58b43-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58b43-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58b43-138">Request headers</span></span>

| <span data-ttu-id="58b43-139">Имя</span><span class="sxs-lookup"><span data-stu-id="58b43-139">Name</span></span>          | <span data-ttu-id="58b43-140">Описание</span><span class="sxs-lookup"><span data-stu-id="58b43-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="58b43-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58b43-141">Authorization</span></span> | <span data-ttu-id="58b43-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58b43-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="58b43-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="58b43-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="58b43-145">CSV</span><span class="sxs-lookup"><span data-stu-id="58b43-145">CSV</span></span>

<span data-ttu-id="58b43-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="58b43-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="58b43-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="58b43-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="58b43-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="58b43-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="58b43-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="58b43-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="58b43-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="58b43-150">Report Refresh Date</span></span>
- <span data-ttu-id="58b43-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="58b43-151">User Principal Name</span></span>
- <span data-ttu-id="58b43-152">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="58b43-152">Last Activity Date</span></span>
- <span data-ttu-id="58b43-153">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="58b43-153">Is Deleted</span></span>
- <span data-ttu-id="58b43-154">Deleted Date (дата удаления);</span><span class="sxs-lookup"><span data-stu-id="58b43-154">Deleted Date</span></span>
- <span data-ttu-id="58b43-155">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="58b43-155">Used Web</span></span>
- <span data-ttu-id="58b43-156">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="58b43-156">Used Windows Phone</span></span>
- <span data-ttu-id="58b43-157">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="58b43-157">Used iOS</span></span>
- <span data-ttu-id="58b43-158">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="58b43-158">Used Mac</span></span>
- <span data-ttu-id="58b43-159">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="58b43-159">Used Android Phone</span></span>
- <span data-ttu-id="58b43-160">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="58b43-160">Used Windows</span></span>
- <span data-ttu-id="58b43-161">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="58b43-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="58b43-162">JSON</span><span class="sxs-lookup"><span data-stu-id="58b43-162">JSON</span></span>

<span data-ttu-id="58b43-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="58b43-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="58b43-164">Размер страницы по умолчанию для этого запроса — 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="58b43-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="58b43-165">Пример</span><span class="sxs-lookup"><span data-stu-id="58b43-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="58b43-166">CSV</span><span class="sxs-lookup"><span data-stu-id="58b43-166">CSV</span></span>

<span data-ttu-id="58b43-167">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="58b43-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="58b43-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="58b43-168">Request</span></span>

<span data-ttu-id="58b43-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58b43-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="58b43-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="58b43-170">Response</span></span>

<span data-ttu-id="58b43-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58b43-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="58b43-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="58b43-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="58b43-173">JSON</span><span class="sxs-lookup"><span data-stu-id="58b43-173">JSON</span></span>

<span data-ttu-id="58b43-174">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="58b43-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="58b43-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="58b43-175">Request</span></span>

<span data-ttu-id="58b43-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58b43-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="58b43-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="58b43-177">Response</span></span>

<span data-ttu-id="58b43-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58b43-178">The following is an example of the response.</span></span>

> <span data-ttu-id="58b43-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58b43-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
