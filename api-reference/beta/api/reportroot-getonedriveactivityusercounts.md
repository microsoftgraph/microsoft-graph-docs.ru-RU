---
title: 'reportRoot: getOneDriveActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей OneDrive.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4798a640c415cc9aecdf360826da2093cecb7195
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528363"
---
# <a name="reportroot-getonedriveactivityusercounts"></a><span data-ttu-id="01137-103">reportRoot: getOneDriveActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="01137-103">reportRoot: getOneDriveActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01137-104">Отслеживайте, как меняется количество активных пользователей OneDrive.</span><span class="sxs-lookup"><span data-stu-id="01137-104">Get the trend in the number of active OneDrive users.</span></span>

> <span data-ttu-id="01137-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="01137-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="01137-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01137-106">Permissions</span></span>

<span data-ttu-id="01137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01137-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01137-109">Permission type</span></span>                        | <span data-ttu-id="01137-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01137-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="01137-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01137-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01137-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01137-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="01137-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01137-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01137-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01137-114">Not supported.</span></span>                           |
| <span data-ttu-id="01137-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01137-115">Application</span></span>                            | <span data-ttu-id="01137-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01137-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="01137-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01137-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="01137-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="01137-118">Function parameters</span></span>

<span data-ttu-id="01137-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="01137-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="01137-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="01137-120">Parameter</span></span> | <span data-ttu-id="01137-121">Тип</span><span class="sxs-lookup"><span data-stu-id="01137-121">Type</span></span>   | <span data-ttu-id="01137-122">Описание</span><span class="sxs-lookup"><span data-stu-id="01137-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="01137-123">period</span><span class="sxs-lookup"><span data-stu-id="01137-123">period</span></span>    | <span data-ttu-id="01137-124">строка</span><span class="sxs-lookup"><span data-stu-id="01137-124">string</span></span> | <span data-ttu-id="01137-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="01137-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="01137-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="01137-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="01137-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="01137-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="01137-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01137-128">Required.</span></span> |

<span data-ttu-id="01137-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01137-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="01137-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="01137-130">The default output type is text/csv.</span></span> <span data-ttu-id="01137-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="01137-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01137-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01137-132">Request headers</span></span>

| <span data-ttu-id="01137-133">Имя</span><span class="sxs-lookup"><span data-stu-id="01137-133">Name</span></span>          | <span data-ttu-id="01137-134">Описание</span><span class="sxs-lookup"><span data-stu-id="01137-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="01137-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01137-135">Authorization</span></span> | <span data-ttu-id="01137-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01137-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="01137-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="01137-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="01137-139">CSV</span><span class="sxs-lookup"><span data-stu-id="01137-139">CSV</span></span>

<span data-ttu-id="01137-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="01137-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="01137-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="01137-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="01137-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="01137-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="01137-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="01137-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="01137-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="01137-144">Report Refresh Date</span></span>
- <span data-ttu-id="01137-145">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="01137-145">Viewed Or Edited</span></span>
- <span data-ttu-id="01137-146">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="01137-146">Synced</span></span>
- <span data-ttu-id="01137-147">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="01137-147">Shared Internally</span></span>
- <span data-ttu-id="01137-148">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="01137-148">Shared Externally</span></span>
- <span data-ttu-id="01137-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="01137-149">Report Date</span></span>
- <span data-ttu-id="01137-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="01137-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="01137-151">JSON</span><span class="sxs-lookup"><span data-stu-id="01137-151">JSON</span></span>

<span data-ttu-id="01137-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[siteActivitySummary](../resources/siteactivitysummary.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01137-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01137-153">Пример</span><span class="sxs-lookup"><span data-stu-id="01137-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="01137-154">CSV</span><span class="sxs-lookup"><span data-stu-id="01137-154">CSV</span></span>

<span data-ttu-id="01137-155">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="01137-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="01137-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="01137-156">Request</span></span>

<span data-ttu-id="01137-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01137-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="01137-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="01137-158">Response</span></span>

<span data-ttu-id="01137-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01137-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="01137-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="01137-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="01137-161">JSON</span><span class="sxs-lookup"><span data-stu-id="01137-161">JSON</span></span>

<span data-ttu-id="01137-162">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="01137-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="01137-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="01137-163">Request</span></span>

<span data-ttu-id="01137-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01137-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="01137-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="01137-165">Response</span></span>

<span data-ttu-id="01137-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01137-166">The following is an example of the response.</span></span>

> <span data-ttu-id="01137-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01137-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 93, 
      "synced": 26, 
      "sharedInternally": 6, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
