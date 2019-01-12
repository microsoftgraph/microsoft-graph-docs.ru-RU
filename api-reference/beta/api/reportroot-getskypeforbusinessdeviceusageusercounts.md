---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: eaf134fdfa528f2e26783c07090a45a7d08831e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978559"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="23f17-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="23f17-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

> <span data-ttu-id="23f17-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23f17-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23f17-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f17-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23f17-107">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="23f17-107">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="23f17-108">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="23f17-108">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="23f17-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="23f17-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="23f17-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23f17-110">Permissions</span></span>

<span data-ttu-id="23f17-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f17-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23f17-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23f17-113">Permission type</span></span>                        | <span data-ttu-id="23f17-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23f17-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23f17-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23f17-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="23f17-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23f17-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23f17-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23f17-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f17-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f17-118">Not supported.</span></span>                           |
| <span data-ttu-id="23f17-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23f17-119">Application</span></span>                            | <span data-ttu-id="23f17-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23f17-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="23f17-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23f17-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="23f17-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="23f17-122">Function parameters</span></span>

<span data-ttu-id="23f17-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="23f17-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="23f17-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="23f17-124">Parameter</span></span> | <span data-ttu-id="23f17-125">Тип</span><span class="sxs-lookup"><span data-stu-id="23f17-125">Type</span></span>   | <span data-ttu-id="23f17-126">Описание</span><span class="sxs-lookup"><span data-stu-id="23f17-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23f17-127">period</span><span class="sxs-lookup"><span data-stu-id="23f17-127">period</span></span>    | <span data-ttu-id="23f17-128">строка</span><span class="sxs-lookup"><span data-stu-id="23f17-128">string</span></span> | <span data-ttu-id="23f17-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23f17-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23f17-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="23f17-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23f17-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="23f17-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="23f17-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23f17-132">Required.</span></span> |

<span data-ttu-id="23f17-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23f17-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="23f17-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="23f17-134">The default output type is text/csv.</span></span> <span data-ttu-id="23f17-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="23f17-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23f17-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23f17-136">Request headers</span></span>

| <span data-ttu-id="23f17-137">Имя</span><span class="sxs-lookup"><span data-stu-id="23f17-137">Name</span></span>          | <span data-ttu-id="23f17-138">Описание</span><span class="sxs-lookup"><span data-stu-id="23f17-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23f17-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23f17-139">Authorization</span></span> | <span data-ttu-id="23f17-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23f17-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23f17-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="23f17-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="23f17-143">CSV</span><span class="sxs-lookup"><span data-stu-id="23f17-143">CSV</span></span>

<span data-ttu-id="23f17-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="23f17-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23f17-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="23f17-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23f17-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="23f17-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23f17-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="23f17-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="23f17-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="23f17-148">Report Refresh Date</span></span>
- <span data-ttu-id="23f17-149">Windows</span><span class="sxs-lookup"><span data-stu-id="23f17-149">Windows</span></span>
- <span data-ttu-id="23f17-150">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="23f17-150">Windows Phone</span></span>
- <span data-ttu-id="23f17-151">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="23f17-151">Android Phone</span></span>
- <span data-ttu-id="23f17-152">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="23f17-152">iPhone</span></span>
- <span data-ttu-id="23f17-153">"iPad";</span><span class="sxs-lookup"><span data-stu-id="23f17-153">iPad</span></span>
- <span data-ttu-id="23f17-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="23f17-154">Report Date</span></span>
- <span data-ttu-id="23f17-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="23f17-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="23f17-156">JSON</span><span class="sxs-lookup"><span data-stu-id="23f17-156">JSON</span></span>

<span data-ttu-id="23f17-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="23f17-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23f17-158">Пример</span><span class="sxs-lookup"><span data-stu-id="23f17-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="23f17-159">CSV</span><span class="sxs-lookup"><span data-stu-id="23f17-159">CSV</span></span>

<span data-ttu-id="23f17-160">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="23f17-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="23f17-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f17-161">Request</span></span>

<span data-ttu-id="23f17-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f17-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="23f17-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="23f17-163">Response</span></span>

<span data-ttu-id="23f17-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="23f17-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="23f17-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="23f17-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="23f17-166">JSON</span><span class="sxs-lookup"><span data-stu-id="23f17-166">JSON</span></span>

<span data-ttu-id="23f17-167">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="23f17-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="23f17-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f17-168">Request</span></span>

<span data-ttu-id="23f17-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f17-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="23f17-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="23f17-170">Response</span></span>

<span data-ttu-id="23f17-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23f17-171">The following is an example of the response.</span></span>

> <span data-ttu-id="23f17-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23f17-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
