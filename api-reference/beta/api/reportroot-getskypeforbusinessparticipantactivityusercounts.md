---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 95220bec57c6c71518b94c130e6b8c8671ef321b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867339"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="738e1-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="738e1-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="738e1-105">Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации</span><span class="sxs-lookup"><span data-stu-id="738e1-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="738e1-106">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу).</span><span class="sxs-lookup"><span data-stu-id="738e1-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="738e1-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия участников конференций Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="738e1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="738e1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="738e1-108">Permissions</span></span>

<span data-ttu-id="738e1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="738e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="738e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="738e1-111">Permission type</span></span>                        | <span data-ttu-id="738e1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="738e1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="738e1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="738e1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="738e1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="738e1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="738e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="738e1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="738e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="738e1-116">Not supported.</span></span>                           |
| <span data-ttu-id="738e1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="738e1-117">Application</span></span>                            | <span data-ttu-id="738e1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="738e1-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="738e1-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="738e1-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="738e1-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="738e1-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="738e1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="738e1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="738e1-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="738e1-122">Function parameters</span></span>

<span data-ttu-id="738e1-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="738e1-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="738e1-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="738e1-124">Parameter</span></span> | <span data-ttu-id="738e1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="738e1-125">Type</span></span>   | <span data-ttu-id="738e1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="738e1-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="738e1-127">period</span><span class="sxs-lookup"><span data-stu-id="738e1-127">period</span></span>    | <span data-ttu-id="738e1-128">string</span><span class="sxs-lookup"><span data-stu-id="738e1-128">string</span></span> | <span data-ttu-id="738e1-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="738e1-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="738e1-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="738e1-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="738e1-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="738e1-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="738e1-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="738e1-132">Required.</span></span> |

<span data-ttu-id="738e1-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="738e1-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="738e1-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="738e1-134">The default output type is text/csv.</span></span> <span data-ttu-id="738e1-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="738e1-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="738e1-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="738e1-136">Request headers</span></span>

| <span data-ttu-id="738e1-137">Имя</span><span class="sxs-lookup"><span data-stu-id="738e1-137">Name</span></span>          | <span data-ttu-id="738e1-138">Описание</span><span class="sxs-lookup"><span data-stu-id="738e1-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="738e1-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="738e1-139">Authorization</span></span> | <span data-ttu-id="738e1-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="738e1-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="738e1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="738e1-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="738e1-143">CSV</span><span class="sxs-lookup"><span data-stu-id="738e1-143">CSV</span></span>

<span data-ttu-id="738e1-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="738e1-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="738e1-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="738e1-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="738e1-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="738e1-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="738e1-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="738e1-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="738e1-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="738e1-148">Report Refresh Date</span></span>
- <span data-ttu-id="738e1-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="738e1-149">Report Date</span></span>
- <span data-ttu-id="738e1-150">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="738e1-150">Report Period</span></span>
- <span data-ttu-id="738e1-151">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="738e1-151">IM</span></span>
- <span data-ttu-id="738e1-152">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="738e1-152">Audio/Video</span></span>
- <span data-ttu-id="738e1-153">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="738e1-153">App Sharing</span></span>
- <span data-ttu-id="738e1-154">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="738e1-154">Web</span></span>
- <span data-ttu-id="738e1-155">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба).</span><span class="sxs-lookup"><span data-stu-id="738e1-155">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="738e1-156">JSON</span><span class="sxs-lookup"><span data-stu-id="738e1-156">JSON</span></span>

<span data-ttu-id="738e1-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспартиЦипантактивитюсеркаунтс](../resources/skypeforbusinessparticipantactivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="738e1-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="738e1-158">Пример</span><span class="sxs-lookup"><span data-stu-id="738e1-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="738e1-159">CSV</span><span class="sxs-lookup"><span data-stu-id="738e1-159">CSV</span></span>

<span data-ttu-id="738e1-160">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="738e1-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="738e1-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="738e1-161">Request</span></span>

<span data-ttu-id="738e1-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="738e1-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="738e1-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="738e1-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="738e1-164">C#</span><span class="sxs-lookup"><span data-stu-id="738e1-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="738e1-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="738e1-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="738e1-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="738e1-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="738e1-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="738e1-167">Response</span></span>

<span data-ttu-id="738e1-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="738e1-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="738e1-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="738e1-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="738e1-170">JSON</span><span class="sxs-lookup"><span data-stu-id="738e1-170">JSON</span></span>

<span data-ttu-id="738e1-171">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="738e1-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="738e1-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="738e1-172">Request</span></span>

<span data-ttu-id="738e1-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="738e1-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="738e1-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="738e1-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="738e1-175">C#</span><span class="sxs-lookup"><span data-stu-id="738e1-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="738e1-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="738e1-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="738e1-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="738e1-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="738e1-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="738e1-178">Response</span></span>

<span data-ttu-id="738e1-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="738e1-179">The following is an example of the response.</span></span>

> <span data-ttu-id="738e1-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="738e1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
