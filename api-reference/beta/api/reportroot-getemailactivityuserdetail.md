---
title: 'reportRoot: getEmailActivityUserDetail'
description: Узнайте, какие действия пользователи выполняли с электронной почтой.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 7cb3545b5bf0571e8b7ce45347dfd9931b3095ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921915"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="72348-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="72348-103">reportRoot: getEmailActivityUserDetail</span></span>

> <span data-ttu-id="72348-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72348-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72348-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72348-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72348-106">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="72348-106">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="72348-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="72348-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="72348-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72348-108">Permissions</span></span>

<span data-ttu-id="72348-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72348-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72348-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72348-111">Permission type</span></span>                        | <span data-ttu-id="72348-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72348-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="72348-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72348-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="72348-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72348-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="72348-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72348-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72348-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72348-116">Not supported.</span></span>                           |
| <span data-ttu-id="72348-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72348-117">Application</span></span>                            | <span data-ttu-id="72348-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72348-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="72348-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72348-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="72348-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="72348-120">Function parameters</span></span>

<span data-ttu-id="72348-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="72348-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="72348-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="72348-122">Parameter</span></span> | <span data-ttu-id="72348-123">Тип</span><span class="sxs-lookup"><span data-stu-id="72348-123">Type</span></span>   | <span data-ttu-id="72348-124">Описание</span><span class="sxs-lookup"><span data-stu-id="72348-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="72348-125">period</span><span class="sxs-lookup"><span data-stu-id="72348-125">period</span></span>    | <span data-ttu-id="72348-126">строка</span><span class="sxs-lookup"><span data-stu-id="72348-126">string</span></span> | <span data-ttu-id="72348-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="72348-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="72348-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="72348-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="72348-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="72348-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="72348-130">date</span><span class="sxs-lookup"><span data-stu-id="72348-130">date</span></span>      | <span data-ttu-id="72348-131">Date</span><span class="sxs-lookup"><span data-stu-id="72348-131">Date</span></span>   | <span data-ttu-id="72348-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="72348-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="72348-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="72348-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="72348-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="72348-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="72348-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="72348-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="72348-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72348-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="72348-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="72348-137">The default output type is text/csv.</span></span> <span data-ttu-id="72348-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="72348-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72348-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72348-139">Request headers</span></span>

| <span data-ttu-id="72348-140">Имя</span><span class="sxs-lookup"><span data-stu-id="72348-140">Name</span></span>          | <span data-ttu-id="72348-141">Описание</span><span class="sxs-lookup"><span data-stu-id="72348-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="72348-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72348-142">Authorization</span></span> | <span data-ttu-id="72348-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72348-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="72348-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="72348-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="72348-146">CSV</span><span class="sxs-lookup"><span data-stu-id="72348-146">CSV</span></span>

<span data-ttu-id="72348-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="72348-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="72348-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="72348-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="72348-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="72348-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="72348-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="72348-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="72348-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="72348-151">Report Refresh Date</span></span>
- <span data-ttu-id="72348-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="72348-152">User Principal Name</span></span>
- <span data-ttu-id="72348-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="72348-153">Display Name</span></span>
- <span data-ttu-id="72348-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="72348-154">Is Deleted</span></span>
- <span data-ttu-id="72348-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="72348-155">Deleted Date</span></span>
- <span data-ttu-id="72348-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="72348-156">Last Activity Date</span></span>
- <span data-ttu-id="72348-157">Send Count (количество отправленных писем)</span><span class="sxs-lookup"><span data-stu-id="72348-157">Send Count</span></span>
- <span data-ttu-id="72348-158">Receive Count (количество полученных писем)</span><span class="sxs-lookup"><span data-stu-id="72348-158">Receive Count</span></span>
- <span data-ttu-id="72348-159">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="72348-159">Read Count</span></span>
- <span data-ttu-id="72348-160">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="72348-160">Assigned Products</span></span>
- <span data-ttu-id="72348-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="72348-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="72348-162">JSON</span><span class="sxs-lookup"><span data-stu-id="72348-162">JSON</span></span>

<span data-ttu-id="72348-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="72348-163">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="72348-164">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="72348-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="72348-165">Пример</span><span class="sxs-lookup"><span data-stu-id="72348-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="72348-166">CSV</span><span class="sxs-lookup"><span data-stu-id="72348-166">CSV</span></span>

<span data-ttu-id="72348-167">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="72348-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="72348-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="72348-168">Request</span></span>

<span data-ttu-id="72348-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72348-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="72348-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="72348-170">Response</span></span>

<span data-ttu-id="72348-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72348-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="72348-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="72348-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="72348-173">JSON</span><span class="sxs-lookup"><span data-stu-id="72348-173">JSON</span></span>

<span data-ttu-id="72348-174">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="72348-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="72348-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="72348-175">Request</span></span>

<span data-ttu-id="72348-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72348-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="72348-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="72348-177">Response</span></span>

<span data-ttu-id="72348-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72348-178">The following is an example of the response.</span></span>

> <span data-ttu-id="72348-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72348-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
