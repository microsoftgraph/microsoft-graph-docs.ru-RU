---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 15ed192eab2641dd91354726812ae4d4f528c71a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336512"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="83cc8-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="83cc8-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83cc8-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="83cc8-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="83cc8-106">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="83cc8-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="83cc8-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="83cc8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="83cc8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83cc8-108">Permissions</span></span>

<span data-ttu-id="83cc8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83cc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83cc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83cc8-111">Permission type</span></span>                        | <span data-ttu-id="83cc8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83cc8-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="83cc8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83cc8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="83cc8-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83cc8-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="83cc8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83cc8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83cc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83cc8-116">Not supported.</span></span>                           |
| <span data-ttu-id="83cc8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83cc8-117">Application</span></span>                            | <span data-ttu-id="83cc8-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83cc8-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="83cc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83cc8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="83cc8-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="83cc8-120">Function parameters</span></span>

<span data-ttu-id="83cc8-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="83cc8-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="83cc8-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="83cc8-122">Parameter</span></span> | <span data-ttu-id="83cc8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="83cc8-123">Type</span></span>   | <span data-ttu-id="83cc8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="83cc8-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="83cc8-125">period</span><span class="sxs-lookup"><span data-stu-id="83cc8-125">period</span></span>    | <span data-ttu-id="83cc8-126">string</span><span class="sxs-lookup"><span data-stu-id="83cc8-126">string</span></span> | <span data-ttu-id="83cc8-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="83cc8-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="83cc8-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="83cc8-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="83cc8-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="83cc8-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="83cc8-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83cc8-130">Required.</span></span> |

<span data-ttu-id="83cc8-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="83cc8-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="83cc8-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="83cc8-132">The default output type is text/csv.</span></span> <span data-ttu-id="83cc8-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="83cc8-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83cc8-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83cc8-134">Request headers</span></span>

| <span data-ttu-id="83cc8-135">Имя</span><span class="sxs-lookup"><span data-stu-id="83cc8-135">Name</span></span>          | <span data-ttu-id="83cc8-136">Описание</span><span class="sxs-lookup"><span data-stu-id="83cc8-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="83cc8-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83cc8-137">Authorization</span></span> | <span data-ttu-id="83cc8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83cc8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="83cc8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="83cc8-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="83cc8-141">CSV</span><span class="sxs-lookup"><span data-stu-id="83cc8-141">CSV</span></span>

<span data-ttu-id="83cc8-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="83cc8-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="83cc8-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="83cc8-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="83cc8-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="83cc8-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="83cc8-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="83cc8-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="83cc8-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="83cc8-146">Report Refresh Date</span></span>
- <span data-ttu-id="83cc8-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="83cc8-147">Report Date</span></span>
- <span data-ttu-id="83cc8-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="83cc8-148">Report Period</span></span>
- <span data-ttu-id="83cc8-149">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="83cc8-149">Audio</span></span>
- <span data-ttu-id="83cc8-150">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="83cc8-150">Video</span></span>

### <a name="json"></a><span data-ttu-id="83cc8-151">JSON</span><span class="sxs-lookup"><span data-stu-id="83cc8-151">JSON</span></span>

<span data-ttu-id="83cc8-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспиртопирактивитиминутекаунтс](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83cc8-152">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83cc8-153">Пример</span><span class="sxs-lookup"><span data-stu-id="83cc8-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="83cc8-154">CSV</span><span class="sxs-lookup"><span data-stu-id="83cc8-154">CSV</span></span>

<span data-ttu-id="83cc8-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="83cc8-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="83cc8-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="83cc8-156">Request</span></span>

<span data-ttu-id="83cc8-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83cc8-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="83cc8-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="83cc8-158">Response</span></span>

<span data-ttu-id="83cc8-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83cc8-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="83cc8-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="83cc8-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="83cc8-161">JSON</span><span class="sxs-lookup"><span data-stu-id="83cc8-161">JSON</span></span>

<span data-ttu-id="83cc8-162">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="83cc8-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="83cc8-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="83cc8-163">Request</span></span>

<span data-ttu-id="83cc8-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83cc8-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="83cc8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="83cc8-165">Response</span></span>

<span data-ttu-id="83cc8-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83cc8-166">The following is an example of the response.</span></span>

> <span data-ttu-id="83cc8-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83cc8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
