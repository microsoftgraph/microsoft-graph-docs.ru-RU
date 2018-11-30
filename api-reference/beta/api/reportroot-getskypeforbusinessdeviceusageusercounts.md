---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
ms.openlocfilehash: 21f8746a94860834ad6fdb2465a672f264fee145
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074824"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="88820-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="88820-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

> <span data-ttu-id="88820-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88820-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88820-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88820-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88820-107">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="88820-107">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="88820-108">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="88820-108">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="88820-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="88820-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="88820-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88820-110">Permissions</span></span>

<span data-ttu-id="88820-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88820-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88820-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88820-113">Permission type</span></span>                        | <span data-ttu-id="88820-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88820-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="88820-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88820-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="88820-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88820-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="88820-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88820-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88820-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88820-118">Not supported.</span></span>                           |
| <span data-ttu-id="88820-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88820-119">Application</span></span>                            | <span data-ttu-id="88820-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88820-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="88820-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88820-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="88820-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="88820-122">Function parameters</span></span>

<span data-ttu-id="88820-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="88820-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="88820-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="88820-124">Parameter</span></span> | <span data-ttu-id="88820-125">Тип</span><span class="sxs-lookup"><span data-stu-id="88820-125">Type</span></span>   | <span data-ttu-id="88820-126">Описание</span><span class="sxs-lookup"><span data-stu-id="88820-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="88820-127">period</span><span class="sxs-lookup"><span data-stu-id="88820-127">period</span></span>    | <span data-ttu-id="88820-128">строка</span><span class="sxs-lookup"><span data-stu-id="88820-128">string</span></span> | <span data-ttu-id="88820-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="88820-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="88820-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="88820-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="88820-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="88820-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="88820-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88820-132">Required.</span></span> |

<span data-ttu-id="88820-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="88820-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="88820-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="88820-134">The default output type is text/csv.</span></span> <span data-ttu-id="88820-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="88820-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88820-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88820-136">Request headers</span></span>

| <span data-ttu-id="88820-137">Имя</span><span class="sxs-lookup"><span data-stu-id="88820-137">Name</span></span>          | <span data-ttu-id="88820-138">Описание</span><span class="sxs-lookup"><span data-stu-id="88820-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="88820-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88820-139">Authorization</span></span> | <span data-ttu-id="88820-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88820-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="88820-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="88820-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="88820-143">CSV</span><span class="sxs-lookup"><span data-stu-id="88820-143">CSV</span></span>

<span data-ttu-id="88820-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="88820-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="88820-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="88820-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="88820-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="88820-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="88820-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="88820-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="88820-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="88820-148">Report Refresh Date</span></span>
- <span data-ttu-id="88820-149">Windows</span><span class="sxs-lookup"><span data-stu-id="88820-149">Windows</span></span>
- <span data-ttu-id="88820-150">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="88820-150">Windows Phone</span></span>
- <span data-ttu-id="88820-151">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="88820-151">Android Phone</span></span>
- <span data-ttu-id="88820-152">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="88820-152">iPhone</span></span>
- <span data-ttu-id="88820-153">"iPad";</span><span class="sxs-lookup"><span data-stu-id="88820-153">iPad</span></span>
- <span data-ttu-id="88820-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="88820-154">Report Date</span></span>
- <span data-ttu-id="88820-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="88820-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="88820-156">JSON</span><span class="sxs-lookup"><span data-stu-id="88820-156">JSON</span></span>

<span data-ttu-id="88820-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="88820-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88820-158">Пример</span><span class="sxs-lookup"><span data-stu-id="88820-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="88820-159">CSV</span><span class="sxs-lookup"><span data-stu-id="88820-159">CSV</span></span>

<span data-ttu-id="88820-160">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="88820-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="88820-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="88820-161">Request</span></span>

<span data-ttu-id="88820-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88820-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="88820-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="88820-163">Response</span></span>

<span data-ttu-id="88820-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="88820-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="88820-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="88820-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="88820-166">JSON</span><span class="sxs-lookup"><span data-stu-id="88820-166">JSON</span></span>

<span data-ttu-id="88820-167">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="88820-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="88820-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="88820-168">Request</span></span>

<span data-ttu-id="88820-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88820-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="88820-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="88820-170">Response</span></span>

<span data-ttu-id="88820-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88820-171">The following is an example of the response.</span></span>

> <span data-ttu-id="88820-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88820-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
