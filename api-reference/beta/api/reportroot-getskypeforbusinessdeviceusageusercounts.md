---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 379446dc0eb317c30ee1339a46331fdfd1c0f9e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332149"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="4f167-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="4f167-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f167-105">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4f167-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="4f167-106">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="4f167-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="4f167-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="4f167-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f167-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f167-108">Permissions</span></span>

<span data-ttu-id="4f167-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f167-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f167-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f167-111">Permission type</span></span>                        | <span data-ttu-id="4f167-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f167-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4f167-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f167-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f167-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f167-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4f167-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f167-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f167-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f167-116">Not supported.</span></span>                           |
| <span data-ttu-id="4f167-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f167-117">Application</span></span>                            | <span data-ttu-id="4f167-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f167-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4f167-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f167-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4f167-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4f167-120">Function parameters</span></span>

<span data-ttu-id="4f167-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4f167-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4f167-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f167-122">Parameter</span></span> | <span data-ttu-id="4f167-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4f167-123">Type</span></span>   | <span data-ttu-id="4f167-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4f167-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4f167-125">period</span><span class="sxs-lookup"><span data-stu-id="4f167-125">period</span></span>    | <span data-ttu-id="4f167-126">string</span><span class="sxs-lookup"><span data-stu-id="4f167-126">string</span></span> | <span data-ttu-id="4f167-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4f167-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4f167-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4f167-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4f167-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4f167-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4f167-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f167-130">Required.</span></span> |

<span data-ttu-id="4f167-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4f167-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4f167-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4f167-132">The default output type is text/csv.</span></span> <span data-ttu-id="4f167-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4f167-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f167-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f167-134">Request headers</span></span>

| <span data-ttu-id="4f167-135">Имя</span><span class="sxs-lookup"><span data-stu-id="4f167-135">Name</span></span>          | <span data-ttu-id="4f167-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4f167-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4f167-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f167-137">Authorization</span></span> | <span data-ttu-id="4f167-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f167-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4f167-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f167-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4f167-141">CSV</span><span class="sxs-lookup"><span data-stu-id="4f167-141">CSV</span></span>

<span data-ttu-id="4f167-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4f167-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4f167-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4f167-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4f167-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4f167-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4f167-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4f167-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4f167-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4f167-146">Report Refresh Date</span></span>
- <span data-ttu-id="4f167-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="4f167-147">Windows</span></span>
- <span data-ttu-id="4f167-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="4f167-148">Windows Phone</span></span>
- <span data-ttu-id="4f167-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="4f167-149">Android Phone</span></span>
- <span data-ttu-id="4f167-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="4f167-150">iPhone</span></span>
- <span data-ttu-id="4f167-151">iPad</span><span class="sxs-lookup"><span data-stu-id="4f167-151">iPad</span></span>
- <span data-ttu-id="4f167-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4f167-152">Report Date</span></span>
- <span data-ttu-id="4f167-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4f167-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4f167-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4f167-154">JSON</span></span>

<span data-ttu-id="4f167-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессдевицеусажеусеркаунтс](../resources/skypeforbusinessdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f167-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f167-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4f167-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4f167-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4f167-157">CSV</span></span>

<span data-ttu-id="4f167-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4f167-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4f167-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f167-159">Request</span></span>

<span data-ttu-id="4f167-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f167-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4f167-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f167-161">Response</span></span>

<span data-ttu-id="4f167-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f167-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4f167-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4f167-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4f167-164">JSON</span><span class="sxs-lookup"><span data-stu-id="4f167-164">JSON</span></span>

<span data-ttu-id="4f167-165">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4f167-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4f167-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f167-166">Request</span></span>

<span data-ttu-id="4f167-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f167-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4f167-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f167-168">Response</span></span>

<span data-ttu-id="4f167-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f167-169">The following is an example of the response.</span></span>

> <span data-ttu-id="4f167-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f167-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
