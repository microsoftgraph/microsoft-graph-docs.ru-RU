---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ceff341f4f75690263267fcc8924db19e0a19a16
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053526"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="edff5-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="edff5-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="edff5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edff5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edff5-105">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="edff5-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="edff5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edff5-106">Permissions</span></span>

<span data-ttu-id="edff5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="edff5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edff5-109">Permission type</span></span>                        | <span data-ttu-id="edff5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edff5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="edff5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edff5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="edff5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="edff5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="edff5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edff5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edff5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edff5-114">Not supported.</span></span>                           |
| <span data-ttu-id="edff5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edff5-115">Application</span></span>                            | <span data-ttu-id="edff5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="edff5-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="edff5-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="edff5-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="edff5-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="edff5-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="edff5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edff5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="edff5-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="edff5-120">Function parameters</span></span>

<span data-ttu-id="edff5-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="edff5-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="edff5-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="edff5-122">Parameter</span></span> | <span data-ttu-id="edff5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="edff5-123">Type</span></span>   | <span data-ttu-id="edff5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="edff5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="edff5-125">period</span><span class="sxs-lookup"><span data-stu-id="edff5-125">period</span></span>    | <span data-ttu-id="edff5-126">string</span><span class="sxs-lookup"><span data-stu-id="edff5-126">string</span></span> | <span data-ttu-id="edff5-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="edff5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="edff5-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="edff5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="edff5-129">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="edff5-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="edff5-130">date</span><span class="sxs-lookup"><span data-stu-id="edff5-130">date</span></span>      | <span data-ttu-id="edff5-131">Date</span><span class="sxs-lookup"><span data-stu-id="edff5-131">Date</span></span>   | <span data-ttu-id="edff5-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="edff5-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="edff5-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="edff5-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="edff5-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="edff5-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="edff5-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="edff5-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="edff5-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="edff5-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="edff5-137">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="edff5-137">The default output type is text/csv.</span></span> <span data-ttu-id="edff5-138">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="edff5-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="edff5-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edff5-139">Request headers</span></span>

| <span data-ttu-id="edff5-140">Имя</span><span class="sxs-lookup"><span data-stu-id="edff5-140">Name</span></span>          | <span data-ttu-id="edff5-141">Описание</span><span class="sxs-lookup"><span data-stu-id="edff5-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="edff5-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edff5-142">Authorization</span></span> | <span data-ttu-id="edff5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edff5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="edff5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="edff5-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="edff5-146">CSV</span><span class="sxs-lookup"><span data-stu-id="edff5-146">CSV</span></span>

<span data-ttu-id="edff5-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="edff5-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="edff5-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="edff5-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="edff5-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="edff5-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="edff5-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="edff5-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="edff5-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="edff5-151">Report Refresh Date</span></span>
- <span data-ttu-id="edff5-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="edff5-152">User Principal Name</span></span>
- <span data-ttu-id="edff5-153">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="edff5-153">Last Activity Date</span></span>
- <span data-ttu-id="edff5-154">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="edff5-154">Is Deleted</span></span>
- <span data-ttu-id="edff5-155">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="edff5-155">Deleted Date</span></span>
- <span data-ttu-id="edff5-156">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="edff5-156">Used Web</span></span>
- <span data-ttu-id="edff5-157">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="edff5-157">Used Windows Phone</span></span>
- <span data-ttu-id="edff5-158">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="edff5-158">Used iOS</span></span>
- <span data-ttu-id="edff5-159">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="edff5-159">Used Mac</span></span>
- <span data-ttu-id="edff5-160">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="edff5-160">Used Android Phone</span></span>
- <span data-ttu-id="edff5-161">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="edff5-161">Used Windows</span></span>
- <span data-ttu-id="edff5-162">Используемая ОС Chrome</span><span class="sxs-lookup"><span data-stu-id="edff5-162">Used Chrome OS</span></span>
- <span data-ttu-id="edff5-163">Использованный Linux</span><span class="sxs-lookup"><span data-stu-id="edff5-163">Used Linux</span></span>
- <span data-ttu-id="edff5-164">Лицензировано</span><span class="sxs-lookup"><span data-stu-id="edff5-164">Is Licensed</span></span>
- <span data-ttu-id="edff5-165">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="edff5-165">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="edff5-166">JSON</span><span class="sxs-lookup"><span data-stu-id="edff5-166">JSON</span></span>

<span data-ttu-id="edff5-167">В случае успешной работы этот метод возвращает код ответа и `200 OK` **[объект teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="edff5-167">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="edff5-168">Размер страницы по умолчанию для этого запроса — 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="edff5-168">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="edff5-169">Пример</span><span class="sxs-lookup"><span data-stu-id="edff5-169">Example</span></span>

### <a name="csv"></a><span data-ttu-id="edff5-170">CSV</span><span class="sxs-lookup"><span data-stu-id="edff5-170">CSV</span></span>

<span data-ttu-id="edff5-171">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="edff5-171">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="edff5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="edff5-172">Request</span></span>

<span data-ttu-id="edff5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edff5-173">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="edff5-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="edff5-174">Response</span></span>

<span data-ttu-id="edff5-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edff5-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="edff5-176">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="edff5-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Used Chrome OS,Used Linux,Is Licensed,Report Period
```

### <a name="json"></a><span data-ttu-id="edff5-177">JSON</span><span class="sxs-lookup"><span data-stu-id="edff5-177">JSON</span></span>

<span data-ttu-id="edff5-178">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="edff5-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="edff5-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="edff5-179">Request</span></span>

<span data-ttu-id="edff5-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edff5-180">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="edff5-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="edff5-181">Response</span></span>

<span data-ttu-id="edff5-182">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="edff5-182">The following is an example of the response.</span></span>

> <span data-ttu-id="edff5-183">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="edff5-183">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "isLicensed": true, 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
      "usedChromeOS": false, 
      "usedLinux": false, 
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


