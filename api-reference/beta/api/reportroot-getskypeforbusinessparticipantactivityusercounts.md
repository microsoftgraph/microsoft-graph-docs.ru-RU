---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a209b8d4e5aecd8cb23bcb987191d53fd1040a32
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639168"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="1981b-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1981b-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1981b-105">Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="1981b-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="1981b-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="1981b-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="1981b-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="1981b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="1981b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1981b-108">Permissions</span></span>

<span data-ttu-id="1981b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1981b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1981b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1981b-111">Permission type</span></span>                        | <span data-ttu-id="1981b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1981b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1981b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1981b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1981b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1981b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1981b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1981b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1981b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1981b-116">Not supported.</span></span>                           |
| <span data-ttu-id="1981b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1981b-117">Application</span></span>                            | <span data-ttu-id="1981b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1981b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1981b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1981b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1981b-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1981b-120">Function parameters</span></span>

<span data-ttu-id="1981b-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1981b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1981b-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="1981b-122">Parameter</span></span> | <span data-ttu-id="1981b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1981b-123">Type</span></span>   | <span data-ttu-id="1981b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1981b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1981b-125">period</span><span class="sxs-lookup"><span data-stu-id="1981b-125">period</span></span>    | <span data-ttu-id="1981b-126">string</span><span class="sxs-lookup"><span data-stu-id="1981b-126">string</span></span> | <span data-ttu-id="1981b-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1981b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1981b-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1981b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1981b-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1981b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1981b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1981b-130">Required.</span></span> |

<span data-ttu-id="1981b-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1981b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1981b-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="1981b-132">The default output type is text/csv.</span></span> <span data-ttu-id="1981b-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1981b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1981b-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1981b-134">Request headers</span></span>

| <span data-ttu-id="1981b-135">Имя</span><span class="sxs-lookup"><span data-stu-id="1981b-135">Name</span></span>          | <span data-ttu-id="1981b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1981b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1981b-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1981b-137">Authorization</span></span> | <span data-ttu-id="1981b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1981b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1981b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1981b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1981b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1981b-141">CSV</span></span>

<span data-ttu-id="1981b-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1981b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1981b-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1981b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1981b-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1981b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1981b-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1981b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1981b-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1981b-146">Report Refresh Date</span></span>
- <span data-ttu-id="1981b-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="1981b-147">Report Date</span></span>
- <span data-ttu-id="1981b-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="1981b-148">Report Period</span></span>
- <span data-ttu-id="1981b-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="1981b-149">IM</span></span>
- <span data-ttu-id="1981b-150">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="1981b-150">Audio/Video</span></span>
- <span data-ttu-id="1981b-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="1981b-151">App Sharing</span></span>
- <span data-ttu-id="1981b-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="1981b-152">Web</span></span>
- <span data-ttu-id="1981b-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="1981b-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="1981b-154">JSON</span><span class="sxs-lookup"><span data-stu-id="1981b-154">JSON</span></span>

<span data-ttu-id="1981b-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспартиЦипантактивитюсеркаунтс](../resources/skypeforbusinessparticipantactivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1981b-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1981b-156">Пример</span><span class="sxs-lookup"><span data-stu-id="1981b-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1981b-157">CSV</span><span class="sxs-lookup"><span data-stu-id="1981b-157">CSV</span></span>

<span data-ttu-id="1981b-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="1981b-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1981b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="1981b-159">Request</span></span>

<span data-ttu-id="1981b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1981b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1981b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="1981b-161">Response</span></span>

<span data-ttu-id="1981b-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1981b-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1981b-163">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1981b-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1981b-164">Языках</span><span class="sxs-lookup"><span data-stu-id="1981b-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1981b-165">Язык</span><span class="sxs-lookup"><span data-stu-id="1981b-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="1981b-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1981b-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1981b-167">JSON</span><span class="sxs-lookup"><span data-stu-id="1981b-167">JSON</span></span>

<span data-ttu-id="1981b-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="1981b-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1981b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="1981b-169">Request</span></span>

<span data-ttu-id="1981b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1981b-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1981b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1981b-171">Response</span></span>

<span data-ttu-id="1981b-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1981b-172">The following is an example of the response.</span></span>

> <span data-ttu-id="1981b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1981b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1981b-175">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1981b-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1981b-176">Языках</span><span class="sxs-lookup"><span data-stu-id="1981b-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1981b-177">Язык</span><span class="sxs-lookup"><span data-stu-id="1981b-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
