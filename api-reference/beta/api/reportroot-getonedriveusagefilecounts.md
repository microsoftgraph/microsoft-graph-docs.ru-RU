---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ecbacda01f470c4101bd9c13499c1a33980cd876
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331873"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="04038-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="04038-104">reportRoot: getOneDriveUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04038-105">Получение общего количества файлов на всех сайтах и количества активных файлов.</span><span class="sxs-lookup"><span data-stu-id="04038-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="04038-106">Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="04038-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="04038-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="04038-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="04038-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04038-108">Permissions</span></span>

<span data-ttu-id="04038-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04038-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04038-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04038-111">Permission type</span></span>                        | <span data-ttu-id="04038-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04038-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="04038-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04038-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="04038-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04038-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="04038-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04038-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04038-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04038-116">Not supported.</span></span>                           |
| <span data-ttu-id="04038-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04038-117">Application</span></span>                            | <span data-ttu-id="04038-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04038-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="04038-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04038-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="04038-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="04038-120">Function parameters</span></span>

<span data-ttu-id="04038-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="04038-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="04038-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="04038-122">Parameter</span></span> | <span data-ttu-id="04038-123">Тип</span><span class="sxs-lookup"><span data-stu-id="04038-123">Type</span></span>   | <span data-ttu-id="04038-124">Описание</span><span class="sxs-lookup"><span data-stu-id="04038-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="04038-125">period</span><span class="sxs-lookup"><span data-stu-id="04038-125">period</span></span>    | <span data-ttu-id="04038-126">string</span><span class="sxs-lookup"><span data-stu-id="04038-126">string</span></span> | <span data-ttu-id="04038-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="04038-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="04038-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="04038-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="04038-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="04038-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="04038-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04038-130">Required.</span></span> |

<span data-ttu-id="04038-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="04038-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="04038-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="04038-132">The default output type is text/csv.</span></span> <span data-ttu-id="04038-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="04038-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04038-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04038-134">Request headers</span></span>

| <span data-ttu-id="04038-135">Имя</span><span class="sxs-lookup"><span data-stu-id="04038-135">Name</span></span>          | <span data-ttu-id="04038-136">Описание</span><span class="sxs-lookup"><span data-stu-id="04038-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="04038-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04038-137">Authorization</span></span> | <span data-ttu-id="04038-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04038-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="04038-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="04038-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="04038-141">CSV</span><span class="sxs-lookup"><span data-stu-id="04038-141">CSV</span></span>

<span data-ttu-id="04038-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="04038-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="04038-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="04038-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="04038-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="04038-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="04038-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="04038-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="04038-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="04038-146">Report Refresh Date</span></span>
- <span data-ttu-id="04038-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="04038-147">Site Type</span></span>
- <span data-ttu-id="04038-148">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="04038-148">Total</span></span>
- <span data-ttu-id="04038-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="04038-149">Active</span></span>
- <span data-ttu-id="04038-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="04038-150">Report Date</span></span>
- <span data-ttu-id="04038-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="04038-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="04038-152">JSON</span><span class="sxs-lookup"><span data-stu-id="04038-152">JSON</span></span>

<span data-ttu-id="04038-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажефилекаунтс](../resources/onedriveusagefilecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04038-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04038-154">Пример</span><span class="sxs-lookup"><span data-stu-id="04038-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="04038-155">CSV</span><span class="sxs-lookup"><span data-stu-id="04038-155">CSV</span></span>

<span data-ttu-id="04038-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="04038-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="04038-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="04038-157">Request</span></span>

<span data-ttu-id="04038-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04038-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="04038-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="04038-159">Response</span></span>

<span data-ttu-id="04038-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04038-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="04038-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="04038-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="04038-162">JSON</span><span class="sxs-lookup"><span data-stu-id="04038-162">JSON</span></span>

<span data-ttu-id="04038-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="04038-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="04038-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="04038-164">Request</span></span>

<span data-ttu-id="04038-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04038-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="04038-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="04038-166">Response</span></span>

<span data-ttu-id="04038-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04038-167">The following is an example of the response.</span></span>

> <span data-ttu-id="04038-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04038-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 297960, 
      "active": 4679, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
