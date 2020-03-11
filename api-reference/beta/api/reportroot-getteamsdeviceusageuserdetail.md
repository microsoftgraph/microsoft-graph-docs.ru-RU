---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 922cd27b869501d5c5d94c8cd0419e19310b62ba
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590387"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="7d21b-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7d21b-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="7d21b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d21b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d21b-105">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="7d21b-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d21b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d21b-106">Permissions</span></span>

<span data-ttu-id="7d21b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d21b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d21b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d21b-109">Permission type</span></span>                        | <span data-ttu-id="7d21b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d21b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7d21b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d21b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d21b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d21b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7d21b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d21b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d21b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d21b-114">Not supported.</span></span>                           |
| <span data-ttu-id="7d21b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d21b-115">Application</span></span>                            | <span data-ttu-id="7d21b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d21b-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="7d21b-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7d21b-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7d21b-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7d21b-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7d21b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d21b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="7d21b-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="7d21b-120">Function parameters</span></span>

<span data-ttu-id="7d21b-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7d21b-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7d21b-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="7d21b-122">Parameter</span></span> | <span data-ttu-id="7d21b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7d21b-123">Type</span></span>   | <span data-ttu-id="7d21b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7d21b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7d21b-125">period</span><span class="sxs-lookup"><span data-stu-id="7d21b-125">period</span></span>    | <span data-ttu-id="7d21b-126">string</span><span class="sxs-lookup"><span data-stu-id="7d21b-126">string</span></span> | <span data-ttu-id="7d21b-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7d21b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7d21b-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7d21b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7d21b-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7d21b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7d21b-130">date</span><span class="sxs-lookup"><span data-stu-id="7d21b-130">date</span></span>      | <span data-ttu-id="7d21b-131">Date</span><span class="sxs-lookup"><span data-stu-id="7d21b-131">Date</span></span>   | <span data-ttu-id="7d21b-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="7d21b-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7d21b-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="7d21b-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7d21b-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="7d21b-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7d21b-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="7d21b-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7d21b-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d21b-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7d21b-137">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="7d21b-137">The default output type is text/csv.</span></span> <span data-ttu-id="7d21b-138">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="7d21b-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d21b-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d21b-139">Request headers</span></span>

| <span data-ttu-id="7d21b-140">Имя</span><span class="sxs-lookup"><span data-stu-id="7d21b-140">Name</span></span>          | <span data-ttu-id="7d21b-141">Описание</span><span class="sxs-lookup"><span data-stu-id="7d21b-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7d21b-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d21b-142">Authorization</span></span> | <span data-ttu-id="7d21b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d21b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7d21b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d21b-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7d21b-146">CSV</span><span class="sxs-lookup"><span data-stu-id="7d21b-146">CSV</span></span>

<span data-ttu-id="7d21b-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7d21b-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7d21b-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7d21b-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7d21b-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7d21b-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7d21b-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7d21b-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7d21b-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7d21b-151">Report Refresh Date</span></span>
- <span data-ttu-id="7d21b-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="7d21b-152">User Principal Name</span></span>
- <span data-ttu-id="7d21b-153">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="7d21b-153">Last Activity Date</span></span>
- <span data-ttu-id="7d21b-154">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="7d21b-154">Is Deleted</span></span>
- <span data-ttu-id="7d21b-155">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="7d21b-155">Deleted Date</span></span>
- <span data-ttu-id="7d21b-156">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="7d21b-156">Used Web</span></span>
- <span data-ttu-id="7d21b-157">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="7d21b-157">Used Windows Phone</span></span>
- <span data-ttu-id="7d21b-158">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="7d21b-158">Used iOS</span></span>
- <span data-ttu-id="7d21b-159">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="7d21b-159">Used Mac</span></span>
- <span data-ttu-id="7d21b-160">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="7d21b-160">Used Android Phone</span></span>
- <span data-ttu-id="7d21b-161">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="7d21b-161">Used Windows</span></span>
- <span data-ttu-id="7d21b-162">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="7d21b-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7d21b-163">JSON</span><span class="sxs-lookup"><span data-stu-id="7d21b-163">JSON</span></span>

<span data-ttu-id="7d21b-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажеусердетаил](../resources/teamsdeviceusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d21b-164">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7d21b-165">Размер страницы по умолчанию для этого запроса составляет 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="7d21b-165">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="7d21b-166">Пример</span><span class="sxs-lookup"><span data-stu-id="7d21b-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7d21b-167">CSV</span><span class="sxs-lookup"><span data-stu-id="7d21b-167">CSV</span></span>

<span data-ttu-id="7d21b-168">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="7d21b-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7d21b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d21b-169">Request</span></span>

<span data-ttu-id="7d21b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d21b-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7d21b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d21b-171">Response</span></span>

<span data-ttu-id="7d21b-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7d21b-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7d21b-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7d21b-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7d21b-174">JSON</span><span class="sxs-lookup"><span data-stu-id="7d21b-174">JSON</span></span>

<span data-ttu-id="7d21b-175">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="7d21b-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7d21b-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d21b-176">Request</span></span>

<span data-ttu-id="7d21b-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d21b-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7d21b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d21b-178">Response</span></span>

<span data-ttu-id="7d21b-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7d21b-179">The following is an example of the response.</span></span>

> <span data-ttu-id="7d21b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d21b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
