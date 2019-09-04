---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1dd89f2e239b540e5a2938a8dee82125e5d6460a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722834"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="6078f-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6078f-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6078f-105">Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации.</span><span class="sxs-lookup"><span data-stu-id="6078f-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="6078f-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="6078f-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="6078f-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="6078f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="6078f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6078f-108">Permissions</span></span>

<span data-ttu-id="6078f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6078f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6078f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6078f-111">Permission type</span></span>                        | <span data-ttu-id="6078f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6078f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6078f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6078f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6078f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6078f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6078f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6078f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6078f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6078f-116">Not supported.</span></span>                           |
| <span data-ttu-id="6078f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6078f-117">Application</span></span>                            | <span data-ttu-id="6078f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6078f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6078f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6078f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6078f-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6078f-120">Function parameters</span></span>

<span data-ttu-id="6078f-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6078f-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6078f-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="6078f-122">Parameter</span></span> | <span data-ttu-id="6078f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6078f-123">Type</span></span>   | <span data-ttu-id="6078f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6078f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6078f-125">period</span><span class="sxs-lookup"><span data-stu-id="6078f-125">period</span></span>    | <span data-ttu-id="6078f-126">string</span><span class="sxs-lookup"><span data-stu-id="6078f-126">string</span></span> | <span data-ttu-id="6078f-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6078f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6078f-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6078f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6078f-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6078f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6078f-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6078f-130">Required.</span></span> |

<span data-ttu-id="6078f-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6078f-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6078f-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="6078f-132">The default output type is text/csv.</span></span> <span data-ttu-id="6078f-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6078f-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6078f-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6078f-134">Request headers</span></span>

| <span data-ttu-id="6078f-135">Имя</span><span class="sxs-lookup"><span data-stu-id="6078f-135">Name</span></span>          | <span data-ttu-id="6078f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6078f-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6078f-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6078f-137">Authorization</span></span> | <span data-ttu-id="6078f-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6078f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6078f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6078f-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6078f-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6078f-141">CSV</span></span>

<span data-ttu-id="6078f-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6078f-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6078f-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6078f-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6078f-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6078f-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6078f-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6078f-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6078f-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6078f-146">Report Refresh Date</span></span>
- <span data-ttu-id="6078f-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="6078f-147">Report Date</span></span>
- <span data-ttu-id="6078f-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="6078f-148">Report Period</span></span>
- <span data-ttu-id="6078f-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="6078f-149">IM</span></span>
- <span data-ttu-id="6078f-150">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="6078f-150">Audio/Video</span></span>
- <span data-ttu-id="6078f-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="6078f-151">App Sharing</span></span>
- <span data-ttu-id="6078f-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="6078f-152">Web</span></span>
- <span data-ttu-id="6078f-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="6078f-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="6078f-154">JSON</span><span class="sxs-lookup"><span data-stu-id="6078f-154">JSON</span></span>

<span data-ttu-id="6078f-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспартиЦипантактивитикаунтс](../resources/skypeforbusinessparticipantactivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6078f-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6078f-156">Пример</span><span class="sxs-lookup"><span data-stu-id="6078f-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6078f-157">CSV</span><span class="sxs-lookup"><span data-stu-id="6078f-157">CSV</span></span>

<span data-ttu-id="6078f-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="6078f-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6078f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="6078f-159">Request</span></span>

<span data-ttu-id="6078f-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6078f-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6078f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="6078f-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6078f-162">C#</span><span class="sxs-lookup"><span data-stu-id="6078f-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6078f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6078f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6078f-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6078f-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6078f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6078f-165">Response</span></span>

<span data-ttu-id="6078f-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6078f-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6078f-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6078f-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="6078f-168">JSON</span><span class="sxs-lookup"><span data-stu-id="6078f-168">JSON</span></span>

<span data-ttu-id="6078f-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="6078f-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6078f-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="6078f-170">Request</span></span>

<span data-ttu-id="6078f-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6078f-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6078f-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="6078f-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6078f-173">C#</span><span class="sxs-lookup"><span data-stu-id="6078f-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6078f-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6078f-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6078f-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6078f-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6078f-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="6078f-176">Response</span></span>

<span data-ttu-id="6078f-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6078f-177">The following is an example of the response.</span></span>

> <span data-ttu-id="6078f-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6078f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
      "dialInOut3rdParty": 2, 
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
