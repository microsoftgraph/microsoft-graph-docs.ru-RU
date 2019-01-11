---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.openlocfilehash: 6fcf60b248b34c097b59139901e3d0204808034d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881993"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="972ee-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="972ee-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

> <span data-ttu-id="972ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="972ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="972ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="972ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="972ee-106">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="972ee-106">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="972ee-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="972ee-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="972ee-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="972ee-108">Permissions</span></span>

<span data-ttu-id="972ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="972ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="972ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="972ee-111">Permission type</span></span>                        | <span data-ttu-id="972ee-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="972ee-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="972ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="972ee-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="972ee-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="972ee-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="972ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="972ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="972ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="972ee-116">Not supported.</span></span>                           |
| <span data-ttu-id="972ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="972ee-117">Application</span></span>                            | <span data-ttu-id="972ee-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="972ee-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="972ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="972ee-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="972ee-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="972ee-120">Function parameters</span></span>

<span data-ttu-id="972ee-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="972ee-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="972ee-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="972ee-122">Parameter</span></span> | <span data-ttu-id="972ee-123">Тип</span><span class="sxs-lookup"><span data-stu-id="972ee-123">Type</span></span>   | <span data-ttu-id="972ee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="972ee-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="972ee-125">period</span><span class="sxs-lookup"><span data-stu-id="972ee-125">period</span></span>    | <span data-ttu-id="972ee-126">строка</span><span class="sxs-lookup"><span data-stu-id="972ee-126">string</span></span> | <span data-ttu-id="972ee-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="972ee-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="972ee-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="972ee-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="972ee-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="972ee-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="972ee-130">date</span><span class="sxs-lookup"><span data-stu-id="972ee-130">date</span></span>      | <span data-ttu-id="972ee-131">Date</span><span class="sxs-lookup"><span data-stu-id="972ee-131">Date</span></span>   | <span data-ttu-id="972ee-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="972ee-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="972ee-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="972ee-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="972ee-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="972ee-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="972ee-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="972ee-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="972ee-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="972ee-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="972ee-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="972ee-137">The default output type is text/csv.</span></span> <span data-ttu-id="972ee-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="972ee-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="972ee-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="972ee-139">Request headers</span></span>

| <span data-ttu-id="972ee-140">Имя</span><span class="sxs-lookup"><span data-stu-id="972ee-140">Name</span></span>          | <span data-ttu-id="972ee-141">Описание</span><span class="sxs-lookup"><span data-stu-id="972ee-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="972ee-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="972ee-142">Authorization</span></span> | <span data-ttu-id="972ee-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="972ee-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="972ee-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="972ee-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="972ee-146">CSV</span><span class="sxs-lookup"><span data-stu-id="972ee-146">CSV</span></span>

<span data-ttu-id="972ee-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="972ee-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="972ee-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="972ee-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="972ee-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="972ee-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="972ee-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="972ee-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="972ee-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="972ee-151">Report Refresh Date</span></span>
- <span data-ttu-id="972ee-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="972ee-152">User Principal Name</span></span>
- <span data-ttu-id="972ee-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="972ee-153">Last Activity Date</span></span>
- <span data-ttu-id="972ee-154">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="972ee-154">Used Windows</span></span>
- <span data-ttu-id="972ee-155">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="972ee-155">Used Windows Phone</span></span>
- <span data-ttu-id="972ee-156">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="972ee-156">Used Android Phone</span></span>
- <span data-ttu-id="972ee-157">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="972ee-157">Used iPhone</span></span>
- <span data-ttu-id="972ee-158">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="972ee-158">Used iPad</span></span>
- <span data-ttu-id="972ee-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="972ee-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="972ee-160">JSON</span><span class="sxs-lookup"><span data-stu-id="972ee-160">JSON</span></span>

<span data-ttu-id="972ee-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="972ee-161">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="972ee-162">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="972ee-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="972ee-163">Пример</span><span class="sxs-lookup"><span data-stu-id="972ee-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="972ee-164">CSV</span><span class="sxs-lookup"><span data-stu-id="972ee-164">CSV</span></span>

<span data-ttu-id="972ee-165">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="972ee-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="972ee-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="972ee-166">Request</span></span>

<span data-ttu-id="972ee-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="972ee-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="972ee-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="972ee-168">Response</span></span>

<span data-ttu-id="972ee-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="972ee-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="972ee-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="972ee-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="972ee-171">JSON</span><span class="sxs-lookup"><span data-stu-id="972ee-171">JSON</span></span>

<span data-ttu-id="972ee-172">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="972ee-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="972ee-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="972ee-173">Request</span></span>

<span data-ttu-id="972ee-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="972ee-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="972ee-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="972ee-175">Response</span></span>

<span data-ttu-id="972ee-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="972ee-176">The following is an example of the response.</span></span>

> <span data-ttu-id="972ee-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="972ee-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "reportPeriod": "7"
    }
  ]
}
```
