---
title: 'reportRoot: getMailboxUsageStorage'
description: Узнайте, сколько места занято в хранилище организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 03533718654d6d4ec083457a64d11836363910b4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331854"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="4d3eb-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="4d3eb-103">reportRoot: getMailboxUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3eb-104">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="4d3eb-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="4d3eb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d3eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d3eb-106">Permissions</span></span>

<span data-ttu-id="4d3eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d3eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d3eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d3eb-109">Permission type</span></span>                        | <span data-ttu-id="4d3eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d3eb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4d3eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d3eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d3eb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d3eb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4d3eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d3eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d3eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-114">Not supported.</span></span>                           |
| <span data-ttu-id="4d3eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d3eb-115">Application</span></span>                            | <span data-ttu-id="4d3eb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d3eb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4d3eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d3eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4d3eb-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4d3eb-118">Function parameters</span></span>

<span data-ttu-id="4d3eb-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4d3eb-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4d3eb-120">Parameter</span></span> | <span data-ttu-id="4d3eb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4d3eb-121">Type</span></span>   | <span data-ttu-id="4d3eb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4d3eb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4d3eb-123">period</span><span class="sxs-lookup"><span data-stu-id="4d3eb-123">period</span></span>    | <span data-ttu-id="4d3eb-124">string</span><span class="sxs-lookup"><span data-stu-id="4d3eb-124">string</span></span> | <span data-ttu-id="4d3eb-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4d3eb-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4d3eb-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4d3eb-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-128">Required.</span></span> |

<span data-ttu-id="4d3eb-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4d3eb-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-130">The default output type is text/csv.</span></span> <span data-ttu-id="4d3eb-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d3eb-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d3eb-132">Request headers</span></span>

| <span data-ttu-id="4d3eb-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4d3eb-133">Name</span></span>          | <span data-ttu-id="4d3eb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4d3eb-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4d3eb-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d3eb-135">Authorization</span></span> | <span data-ttu-id="4d3eb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4d3eb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d3eb-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4d3eb-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4d3eb-139">CSV</span></span>

<span data-ttu-id="4d3eb-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4d3eb-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4d3eb-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4d3eb-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4d3eb-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4d3eb-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4d3eb-144">Report Refresh Date</span></span>
- <span data-ttu-id="4d3eb-145">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="4d3eb-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="4d3eb-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4d3eb-146">Report Date</span></span>
- <span data-ttu-id="4d3eb-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4d3eb-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4d3eb-148">JSON</span><span class="sxs-lookup"><span data-stu-id="4d3eb-148">JSON</span></span>

<span data-ttu-id="4d3eb-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажестораже](../resources/mailboxusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-149">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d3eb-150">Пример</span><span class="sxs-lookup"><span data-stu-id="4d3eb-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4d3eb-151">CSV</span><span class="sxs-lookup"><span data-stu-id="4d3eb-151">CSV</span></span>

<span data-ttu-id="4d3eb-152">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4d3eb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d3eb-153">Request</span></span>

<span data-ttu-id="4d3eb-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4d3eb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d3eb-155">Response</span></span>

<span data-ttu-id="4d3eb-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4d3eb-157">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4d3eb-158">JSON</span><span class="sxs-lookup"><span data-stu-id="4d3eb-158">JSON</span></span>

<span data-ttu-id="4d3eb-159">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4d3eb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d3eb-160">Request</span></span>

<span data-ttu-id="4d3eb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4d3eb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d3eb-162">Response</span></span>

<span data-ttu-id="4d3eb-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-163">The following is an example of the response.</span></span>

> <span data-ttu-id="4d3eb-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d3eb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "storageUsedInBytes": 5159432679270, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
