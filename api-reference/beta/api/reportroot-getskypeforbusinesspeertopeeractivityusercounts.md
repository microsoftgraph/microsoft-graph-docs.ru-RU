---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7c27e454f5a74c186a30d5f3b495fb83a9cd52a0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269120"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="6317d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6317d-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6317d-105">Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="6317d-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="6317d-106">Такие типы включают обмен мгновенными сообщениями, предоставление общего доступа к приложениям, аудио, видео, а также передачу файлов в одноранговых сеансах.</span><span class="sxs-lookup"><span data-stu-id="6317d-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="6317d-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в одноранговых сеансах Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="6317d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="6317d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6317d-108">Permissions</span></span>

<span data-ttu-id="6317d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6317d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6317d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6317d-111">Permission type</span></span>                        | <span data-ttu-id="6317d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6317d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6317d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6317d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6317d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6317d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6317d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6317d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6317d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6317d-116">Not supported.</span></span>                           |
| <span data-ttu-id="6317d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6317d-117">Application</span></span>                            | <span data-ttu-id="6317d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6317d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6317d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6317d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6317d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6317d-120">Function parameters</span></span>

<span data-ttu-id="6317d-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6317d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6317d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="6317d-122">Parameter</span></span> | <span data-ttu-id="6317d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6317d-123">Type</span></span>   | <span data-ttu-id="6317d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6317d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6317d-125">period</span><span class="sxs-lookup"><span data-stu-id="6317d-125">period</span></span>    | <span data-ttu-id="6317d-126">string</span><span class="sxs-lookup"><span data-stu-id="6317d-126">string</span></span> | <span data-ttu-id="6317d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6317d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6317d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6317d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6317d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6317d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6317d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6317d-130">Required.</span></span> |

<span data-ttu-id="6317d-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6317d-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6317d-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="6317d-132">The default output type is text/csv.</span></span> <span data-ttu-id="6317d-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6317d-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6317d-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6317d-134">Request headers</span></span>

| <span data-ttu-id="6317d-135">Имя</span><span class="sxs-lookup"><span data-stu-id="6317d-135">Name</span></span>          | <span data-ttu-id="6317d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6317d-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6317d-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6317d-137">Authorization</span></span> | <span data-ttu-id="6317d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6317d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6317d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6317d-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6317d-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6317d-141">CSV</span></span>

<span data-ttu-id="6317d-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6317d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6317d-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6317d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6317d-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6317d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6317d-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6317d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6317d-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6317d-146">Report Refresh Date</span></span>
- <span data-ttu-id="6317d-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="6317d-147">Report Date</span></span>
- <span data-ttu-id="6317d-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="6317d-148">Report Period</span></span>
- <span data-ttu-id="6317d-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="6317d-149">IM</span></span>
- <span data-ttu-id="6317d-150">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="6317d-150">Audio</span></span>
- <span data-ttu-id="6317d-151">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="6317d-151">Video</span></span>
- <span data-ttu-id="6317d-152">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="6317d-152">App Sharing</span></span>
- <span data-ttu-id="6317d-153">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="6317d-153">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="6317d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="6317d-154">JSON</span></span>

<span data-ttu-id="6317d-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспиртопирактивитюсеркаунтс](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6317d-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6317d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="6317d-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6317d-157">CSV</span><span class="sxs-lookup"><span data-stu-id="6317d-157">CSV</span></span>

<span data-ttu-id="6317d-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="6317d-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6317d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="6317d-159">Request</span></span>

<span data-ttu-id="6317d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6317d-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6317d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6317d-161">Response</span></span>

<span data-ttu-id="6317d-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6317d-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6317d-163">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="6317d-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6317d-164">C#</span><span class="sxs-lookup"><span data-stu-id="6317d-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6317d-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="6317d-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6317d-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6317d-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6317d-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6317d-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="6317d-168">JSON</span><span class="sxs-lookup"><span data-stu-id="6317d-168">JSON</span></span>

<span data-ttu-id="6317d-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="6317d-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6317d-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="6317d-170">Request</span></span>

<span data-ttu-id="6317d-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6317d-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6317d-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="6317d-172">Response</span></span>

<span data-ttu-id="6317d-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6317d-173">The following is an example of the response.</span></span>

> <span data-ttu-id="6317d-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6317d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts)", 
  "value": [
    {
      "im": 379, 
      "audio": 42, 
      "video": 2, 
      "appSharing": 34, 
      "fileTransfer": 36, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6317d-176">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6317d-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6317d-177">C#</span><span class="sxs-lookup"><span data-stu-id="6317d-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6317d-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="6317d-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6317d-179">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6317d-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivityusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
