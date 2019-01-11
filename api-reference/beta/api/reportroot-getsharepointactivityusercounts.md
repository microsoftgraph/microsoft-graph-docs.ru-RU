---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.
localization_priority: Normal
ms.openlocfilehash: 356f079a1d0836b6cd824a30d6882ed12f0155fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842205"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="0230c-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0230c-104">reportRoot: getSharePointActivityUserCounts</span></span>

> <span data-ttu-id="0230c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0230c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0230c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0230c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0230c-107">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="0230c-107">Get the trend in the number of active users.</span></span> <span data-ttu-id="0230c-108">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="0230c-108">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="0230c-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="0230c-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="0230c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0230c-110">Permissions</span></span>

<span data-ttu-id="0230c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0230c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0230c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0230c-113">Permission type</span></span>                        | <span data-ttu-id="0230c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0230c-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0230c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0230c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="0230c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0230c-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0230c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0230c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0230c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0230c-118">Not supported.</span></span>                           |
| <span data-ttu-id="0230c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0230c-119">Application</span></span>                            | <span data-ttu-id="0230c-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0230c-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0230c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0230c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0230c-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="0230c-122">Function parameters</span></span>

<span data-ttu-id="0230c-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0230c-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0230c-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="0230c-124">Parameter</span></span> | <span data-ttu-id="0230c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0230c-125">Type</span></span>   | <span data-ttu-id="0230c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0230c-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0230c-127">period</span><span class="sxs-lookup"><span data-stu-id="0230c-127">period</span></span>    | <span data-ttu-id="0230c-128">строка</span><span class="sxs-lookup"><span data-stu-id="0230c-128">string</span></span> | <span data-ttu-id="0230c-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0230c-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0230c-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0230c-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0230c-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0230c-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0230c-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0230c-132">Required.</span></span> |

<span data-ttu-id="0230c-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0230c-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0230c-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="0230c-134">The default output type is text/csv.</span></span> <span data-ttu-id="0230c-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="0230c-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0230c-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0230c-136">Request headers</span></span>

| <span data-ttu-id="0230c-137">Имя</span><span class="sxs-lookup"><span data-stu-id="0230c-137">Name</span></span>          | <span data-ttu-id="0230c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0230c-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0230c-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0230c-139">Authorization</span></span> | <span data-ttu-id="0230c-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0230c-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0230c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="0230c-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0230c-143">CSV</span><span class="sxs-lookup"><span data-stu-id="0230c-143">CSV</span></span>

<span data-ttu-id="0230c-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0230c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0230c-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0230c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0230c-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0230c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0230c-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0230c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0230c-148">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="0230c-148">Report Refresh Date</span></span>
- <span data-ttu-id="0230c-149">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="0230c-149">Visited Page</span></span>
- <span data-ttu-id="0230c-150">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="0230c-150">Viewed Or Edited</span></span>
- <span data-ttu-id="0230c-151">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="0230c-151">Synced</span></span>
- <span data-ttu-id="0230c-152">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="0230c-152">Shared Internally</span></span>
- <span data-ttu-id="0230c-153">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="0230c-153">Shared Externally</span></span>
- <span data-ttu-id="0230c-154">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="0230c-154">Report Date</span></span>
- <span data-ttu-id="0230c-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="0230c-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0230c-156">JSON</span><span class="sxs-lookup"><span data-stu-id="0230c-156">JSON</span></span>

<span data-ttu-id="0230c-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0230c-157">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0230c-158">Пример</span><span class="sxs-lookup"><span data-stu-id="0230c-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0230c-159">CSV</span><span class="sxs-lookup"><span data-stu-id="0230c-159">CSV</span></span>

<span data-ttu-id="0230c-160">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="0230c-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0230c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="0230c-161">Request</span></span>

<span data-ttu-id="0230c-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0230c-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0230c-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="0230c-163">Response</span></span>

<span data-ttu-id="0230c-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0230c-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0230c-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0230c-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="0230c-166">JSON</span><span class="sxs-lookup"><span data-stu-id="0230c-166">JSON</span></span>

<span data-ttu-id="0230c-167">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="0230c-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0230c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="0230c-168">Request</span></span>

<span data-ttu-id="0230c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0230c-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0230c-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="0230c-170">Response</span></span>

<span data-ttu-id="0230c-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0230c-171">The following is an example of the response.</span></span>

> <span data-ttu-id="0230c-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0230c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
