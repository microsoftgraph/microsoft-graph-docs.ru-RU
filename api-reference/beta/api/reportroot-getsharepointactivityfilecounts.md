---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 647b58f55e10c85d2c54c34324d5e21362f6176e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955368"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="ad9a2-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="ad9a2-103">reportRoot: getSharePointActivityFileCounts</span></span>

> <span data-ttu-id="ad9a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad9a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad9a2-106">Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-106">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="ad9a2-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="ad9a2-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad9a2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad9a2-108">Permissions</span></span>

<span data-ttu-id="ad9a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad9a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad9a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad9a2-111">Permission type</span></span>                        | <span data-ttu-id="ad9a2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad9a2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad9a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad9a2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad9a2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad9a2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad9a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad9a2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad9a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-116">Not supported.</span></span>                           |
| <span data-ttu-id="ad9a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad9a2-117">Application</span></span>                            | <span data-ttu-id="ad9a2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad9a2-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ad9a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad9a2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ad9a2-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="ad9a2-120">Function parameters</span></span>

<span data-ttu-id="ad9a2-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ad9a2-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="ad9a2-122">Parameter</span></span> | <span data-ttu-id="ad9a2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ad9a2-123">Type</span></span>   | <span data-ttu-id="ad9a2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ad9a2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad9a2-125">period</span><span class="sxs-lookup"><span data-stu-id="ad9a2-125">period</span></span>    | <span data-ttu-id="ad9a2-126">строка</span><span class="sxs-lookup"><span data-stu-id="ad9a2-126">string</span></span> | <span data-ttu-id="ad9a2-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad9a2-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad9a2-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ad9a2-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-130">Required.</span></span> |

<span data-ttu-id="ad9a2-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ad9a2-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-132">The default output type is text/csv.</span></span> <span data-ttu-id="ad9a2-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad9a2-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad9a2-134">Request headers</span></span>

| <span data-ttu-id="ad9a2-135">Имя</span><span class="sxs-lookup"><span data-stu-id="ad9a2-135">Name</span></span>          | <span data-ttu-id="ad9a2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ad9a2-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ad9a2-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad9a2-137">Authorization</span></span> | <span data-ttu-id="ad9a2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ad9a2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad9a2-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ad9a2-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ad9a2-141">CSV</span></span>

<span data-ttu-id="ad9a2-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad9a2-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad9a2-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad9a2-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ad9a2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad9a2-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ad9a2-146">Report Refresh Date</span></span>
- <span data-ttu-id="ad9a2-147">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="ad9a2-147">Viewed Or Edited</span></span>
- <span data-ttu-id="ad9a2-148">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="ad9a2-148">Synced</span></span>
- <span data-ttu-id="ad9a2-149">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="ad9a2-149">Shared Internally</span></span>
- <span data-ttu-id="ad9a2-150">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="ad9a2-150">Shared Externally</span></span>
- <span data-ttu-id="ad9a2-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="ad9a2-151">Report Date</span></span>
- <span data-ttu-id="ad9a2-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ad9a2-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ad9a2-153">JSON</span><span class="sxs-lookup"><span data-stu-id="ad9a2-153">JSON</span></span>

<span data-ttu-id="ad9a2-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[siteActivitySummary](../resources/siteactivitysummary.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-154">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad9a2-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ad9a2-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ad9a2-156">CSV</span><span class="sxs-lookup"><span data-stu-id="ad9a2-156">CSV</span></span>

<span data-ttu-id="ad9a2-157">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ad9a2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad9a2-158">Request</span></span>

<span data-ttu-id="ad9a2-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ad9a2-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad9a2-160">Response</span></span>

<span data-ttu-id="ad9a2-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ad9a2-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ad9a2-163">JSON</span><span class="sxs-lookup"><span data-stu-id="ad9a2-163">JSON</span></span>

<span data-ttu-id="ad9a2-164">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ad9a2-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad9a2-165">Request</span></span>

<span data-ttu-id="ad9a2-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ad9a2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad9a2-167">Response</span></span>

<span data-ttu-id="ad9a2-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-168">The following is an example of the response.</span></span>

> <span data-ttu-id="ad9a2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad9a2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
