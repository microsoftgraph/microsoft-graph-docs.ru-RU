---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fe785f6a86a885baddf8156df4cd07d038cee1c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991893"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="df9d5-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="df9d5-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df9d5-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="df9d5-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="df9d5-106">(аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="df9d5-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="df9d5-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="df9d5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="df9d5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df9d5-108">Permissions</span></span>

<span data-ttu-id="df9d5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df9d5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df9d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df9d5-111">Permission type</span></span>                        | <span data-ttu-id="df9d5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df9d5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="df9d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df9d5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="df9d5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df9d5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="df9d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df9d5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df9d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df9d5-116">Not supported.</span></span>                           |
| <span data-ttu-id="df9d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df9d5-117">Application</span></span>                            | <span data-ttu-id="df9d5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df9d5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="df9d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df9d5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="df9d5-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="df9d5-120">Function parameters</span></span>

<span data-ttu-id="df9d5-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="df9d5-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="df9d5-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="df9d5-122">Parameter</span></span> | <span data-ttu-id="df9d5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="df9d5-123">Type</span></span>   | <span data-ttu-id="df9d5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="df9d5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="df9d5-125">period</span><span class="sxs-lookup"><span data-stu-id="df9d5-125">period</span></span>    | <span data-ttu-id="df9d5-126">string</span><span class="sxs-lookup"><span data-stu-id="df9d5-126">string</span></span> | <span data-ttu-id="df9d5-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="df9d5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="df9d5-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="df9d5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="df9d5-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="df9d5-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="df9d5-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df9d5-130">Required.</span></span> |

<span data-ttu-id="df9d5-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="df9d5-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="df9d5-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="df9d5-132">The default output type is text/csv.</span></span> <span data-ttu-id="df9d5-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="df9d5-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df9d5-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df9d5-134">Request headers</span></span>

| <span data-ttu-id="df9d5-135">Имя</span><span class="sxs-lookup"><span data-stu-id="df9d5-135">Name</span></span>          | <span data-ttu-id="df9d5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="df9d5-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="df9d5-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df9d5-137">Authorization</span></span> | <span data-ttu-id="df9d5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df9d5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="df9d5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="df9d5-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="df9d5-141">CSV</span><span class="sxs-lookup"><span data-stu-id="df9d5-141">CSV</span></span>

<span data-ttu-id="df9d5-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="df9d5-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="df9d5-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="df9d5-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="df9d5-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="df9d5-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="df9d5-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="df9d5-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="df9d5-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="df9d5-146">Report Refresh Date</span></span>
- <span data-ttu-id="df9d5-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="df9d5-147">Report Date</span></span>
- <span data-ttu-id="df9d5-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="df9d5-148">Report Period</span></span>
- <span data-ttu-id="df9d5-149">Audio/Video (аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="df9d5-149">Audio/Video</span></span>
- <span data-ttu-id="df9d5-150">Dial-in Microsoft (с телефонным подключением через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df9d5-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="df9d5-151">Dial-out Microsoft (с присоединением обратным звонком через Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df9d5-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="df9d5-152">JSON</span><span class="sxs-lookup"><span data-stu-id="df9d5-152">JSON</span></span>

<span data-ttu-id="df9d5-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитиминутекаунтс](../resources/skypeforbusinessorganizeractivityminutecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df9d5-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df9d5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="df9d5-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="df9d5-155">CSV</span><span class="sxs-lookup"><span data-stu-id="df9d5-155">CSV</span></span>

<span data-ttu-id="df9d5-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="df9d5-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="df9d5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="df9d5-157">Request</span></span>

<span data-ttu-id="df9d5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df9d5-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="df9d5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="df9d5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df9d5-160">C#</span><span class="sxs-lookup"><span data-stu-id="df9d5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df9d5-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="df9d5-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df9d5-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="df9d5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="df9d5-163">Java</span><span class="sxs-lookup"><span data-stu-id="df9d5-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityminutecounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df9d5-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="df9d5-164">Response</span></span>

<span data-ttu-id="df9d5-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df9d5-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="df9d5-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="df9d5-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="df9d5-167">JSON</span><span class="sxs-lookup"><span data-stu-id="df9d5-167">JSON</span></span>

<span data-ttu-id="df9d5-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="df9d5-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="df9d5-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="df9d5-169">Request</span></span>

<span data-ttu-id="df9d5-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df9d5-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="df9d5-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="df9d5-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df9d5-172">C#</span><span class="sxs-lookup"><span data-stu-id="df9d5-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df9d5-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="df9d5-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df9d5-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="df9d5-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="df9d5-175">Java</span><span class="sxs-lookup"><span data-stu-id="df9d5-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityminutecounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df9d5-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="df9d5-176">Response</span></span>

<span data-ttu-id="df9d5-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="df9d5-177">The following is an example of the response.</span></span>

> <span data-ttu-id="df9d5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df9d5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
