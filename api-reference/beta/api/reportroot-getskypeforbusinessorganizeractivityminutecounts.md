---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 035103416a1d106e49eada0066c4327e47d78730
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265172"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="b64d4-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="b64d4-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b64d4-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="b64d4-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="b64d4-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="b64d4-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="b64d4-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="b64d4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="b64d4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b64d4-108">Permissions</span></span>

<span data-ttu-id="b64d4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b64d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b64d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b64d4-111">Permission type</span></span>                        | <span data-ttu-id="b64d4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b64d4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b64d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b64d4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b64d4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b64d4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b64d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b64d4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b64d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b64d4-116">Not supported.</span></span>                           |
| <span data-ttu-id="b64d4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b64d4-117">Application</span></span>                            | <span data-ttu-id="b64d4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b64d4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b64d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b64d4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b64d4-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b64d4-120">Function parameters</span></span>

<span data-ttu-id="b64d4-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b64d4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b64d4-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="b64d4-122">Parameter</span></span> | <span data-ttu-id="b64d4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b64d4-123">Type</span></span>   | <span data-ttu-id="b64d4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b64d4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b64d4-125">period</span><span class="sxs-lookup"><span data-stu-id="b64d4-125">period</span></span>    | <span data-ttu-id="b64d4-126">string</span><span class="sxs-lookup"><span data-stu-id="b64d4-126">string</span></span> | <span data-ttu-id="b64d4-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b64d4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b64d4-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b64d4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b64d4-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b64d4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b64d4-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b64d4-130">Required.</span></span> |

<span data-ttu-id="b64d4-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b64d4-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b64d4-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="b64d4-132">The default output type is text/csv.</span></span> <span data-ttu-id="b64d4-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b64d4-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b64d4-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b64d4-134">Request headers</span></span>

| <span data-ttu-id="b64d4-135">Имя</span><span class="sxs-lookup"><span data-stu-id="b64d4-135">Name</span></span>          | <span data-ttu-id="b64d4-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b64d4-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b64d4-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b64d4-137">Authorization</span></span> | <span data-ttu-id="b64d4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b64d4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b64d4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b64d4-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b64d4-141">CSV</span><span class="sxs-lookup"><span data-stu-id="b64d4-141">CSV</span></span>

<span data-ttu-id="b64d4-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b64d4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b64d4-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b64d4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b64d4-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b64d4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b64d4-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b64d4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b64d4-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b64d4-146">Report Refresh Date</span></span>
- <span data-ttu-id="b64d4-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="b64d4-147">Report Date</span></span>
- <span data-ttu-id="b64d4-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="b64d4-148">Report Period</span></span>
- <span data-ttu-id="b64d4-149">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="b64d4-149">Audio/Video</span></span>
- <span data-ttu-id="b64d4-150">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b64d4-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="b64d4-151">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b64d4-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="b64d4-152">JSON</span><span class="sxs-lookup"><span data-stu-id="b64d4-152">JSON</span></span>

<span data-ttu-id="b64d4-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитиминутекаунтс](../resources/skypeforbusinessorganizeractivityminutecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b64d4-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b64d4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="b64d4-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b64d4-155">CSV</span><span class="sxs-lookup"><span data-stu-id="b64d4-155">CSV</span></span>

<span data-ttu-id="b64d4-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="b64d4-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b64d4-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b64d4-157">Request</span></span>

<span data-ttu-id="b64d4-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b64d4-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b64d4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b64d4-159">Response</span></span>

<span data-ttu-id="b64d4-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b64d4-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b64d4-161">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="b64d4-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b64d4-162">C#</span><span class="sxs-lookup"><span data-stu-id="b64d4-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b64d4-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="b64d4-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b64d4-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b64d4-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="b64d4-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b64d4-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```

### <a name="json"></a><span data-ttu-id="b64d4-166">JSON</span><span class="sxs-lookup"><span data-stu-id="b64d4-166">JSON</span></span>

<span data-ttu-id="b64d4-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="b64d4-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b64d4-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="b64d4-168">Request</span></span>

<span data-ttu-id="b64d4-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b64d4-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b64d4-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="b64d4-170">Response</span></span>

<span data-ttu-id="b64d4-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b64d4-171">The following is an example of the response.</span></span>

> <span data-ttu-id="b64d4-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b64d4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts)", 
  "value": [
    {
      "audioVideo": 1912, 
      "dialInMicrosoft": 108, 
      "dialOutMicrosoft": 0, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b64d4-174">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b64d4-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b64d4-175">C#</span><span class="sxs-lookup"><span data-stu-id="b64d4-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b64d4-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="b64d4-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b64d4-177">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b64d4-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
