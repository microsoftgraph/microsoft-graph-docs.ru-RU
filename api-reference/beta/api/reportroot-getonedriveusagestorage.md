---
title: 'reportRoot: getOneDriveUsageStorage'
description: Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 04ee3c303b086e82f322f3bc0778d1d4533ff5e7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933101"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="f6c13-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="f6c13-103">reportRoot: getOneDriveUsageStorage</span></span>

> <span data-ttu-id="f6c13-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f6c13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6c13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c13-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6c13-106">Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f6c13-106">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="f6c13-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="f6c13-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c13-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c13-108">Permissions</span></span>

<span data-ttu-id="f6c13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6c13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6c13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c13-111">Permission type</span></span>                        | <span data-ttu-id="f6c13-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6c13-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f6c13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6c13-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6c13-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6c13-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f6c13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6c13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c13-116">Not supported.</span></span>                           |
| <span data-ttu-id="f6c13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6c13-117">Application</span></span>                            | <span data-ttu-id="f6c13-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6c13-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f6c13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6c13-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f6c13-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="f6c13-120">Function parameters</span></span>

<span data-ttu-id="f6c13-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f6c13-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f6c13-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="f6c13-122">Parameter</span></span> | <span data-ttu-id="f6c13-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f6c13-123">Type</span></span>   | <span data-ttu-id="f6c13-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c13-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f6c13-125">period</span><span class="sxs-lookup"><span data-stu-id="f6c13-125">period</span></span>    | <span data-ttu-id="f6c13-126">строка</span><span class="sxs-lookup"><span data-stu-id="f6c13-126">string</span></span> | <span data-ttu-id="f6c13-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f6c13-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f6c13-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f6c13-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f6c13-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f6c13-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f6c13-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c13-130">Required.</span></span> |

<span data-ttu-id="f6c13-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6c13-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f6c13-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="f6c13-132">The default output type is text/csv.</span></span> <span data-ttu-id="f6c13-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="f6c13-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6c13-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6c13-134">Request headers</span></span>

| <span data-ttu-id="f6c13-135">Имя</span><span class="sxs-lookup"><span data-stu-id="f6c13-135">Name</span></span>          | <span data-ttu-id="f6c13-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c13-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f6c13-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6c13-137">Authorization</span></span> | <span data-ttu-id="f6c13-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c13-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f6c13-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6c13-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f6c13-141">CSV</span><span class="sxs-lookup"><span data-stu-id="f6c13-141">CSV</span></span>

<span data-ttu-id="f6c13-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f6c13-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f6c13-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c13-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f6c13-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f6c13-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f6c13-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f6c13-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f6c13-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f6c13-146">Report Refresh Date</span></span>
- <span data-ttu-id="f6c13-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="f6c13-147">Site Type</span></span>
- <span data-ttu-id="f6c13-148">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="f6c13-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="f6c13-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="f6c13-149">Report Date</span></span>
- <span data-ttu-id="f6c13-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="f6c13-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f6c13-151">JSON</span><span class="sxs-lookup"><span data-stu-id="f6c13-151">JSON</span></span>

<span data-ttu-id="f6c13-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[siteUsageStorage](../resources/siteusagestorage.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f6c13-152">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c13-153">Пример</span><span class="sxs-lookup"><span data-stu-id="f6c13-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f6c13-154">CSV</span><span class="sxs-lookup"><span data-stu-id="f6c13-154">CSV</span></span>

<span data-ttu-id="f6c13-155">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="f6c13-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f6c13-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6c13-156">Request</span></span>

<span data-ttu-id="f6c13-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6c13-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f6c13-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6c13-158">Response</span></span>

<span data-ttu-id="f6c13-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f6c13-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f6c13-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f6c13-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f6c13-161">JSON</span><span class="sxs-lookup"><span data-stu-id="f6c13-161">JSON</span></span>

<span data-ttu-id="f6c13-162">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="f6c13-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f6c13-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6c13-163">Request</span></span>

<span data-ttu-id="f6c13-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6c13-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f6c13-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6c13-165">Response</span></span>

<span data-ttu-id="f6c13-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c13-166">The following is an example of the response.</span></span>

> <span data-ttu-id="f6c13-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6c13-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 132654293197, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
