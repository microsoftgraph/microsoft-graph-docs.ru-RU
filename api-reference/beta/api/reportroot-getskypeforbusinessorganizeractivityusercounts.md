---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 94af6ef213cc0f32eb86c0e21b53ad0917dda6a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987980"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="753f8-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="753f8-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="753f8-105">Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="753f8-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="753f8-106">Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="753f8-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="753f8-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="753f8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="753f8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="753f8-108">Permissions</span></span>

<span data-ttu-id="753f8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="753f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="753f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="753f8-111">Permission type</span></span>                        | <span data-ttu-id="753f8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="753f8-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="753f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="753f8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="753f8-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="753f8-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="753f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="753f8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="753f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="753f8-116">Not supported.</span></span>                           |
| <span data-ttu-id="753f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="753f8-117">Application</span></span>                            | <span data-ttu-id="753f8-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="753f8-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="753f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="753f8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="753f8-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="753f8-120">Function parameters</span></span>

<span data-ttu-id="753f8-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="753f8-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="753f8-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="753f8-122">Parameter</span></span> | <span data-ttu-id="753f8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="753f8-123">Type</span></span>   | <span data-ttu-id="753f8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="753f8-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="753f8-125">period</span><span class="sxs-lookup"><span data-stu-id="753f8-125">period</span></span>    | <span data-ttu-id="753f8-126">string</span><span class="sxs-lookup"><span data-stu-id="753f8-126">string</span></span> | <span data-ttu-id="753f8-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="753f8-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="753f8-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="753f8-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="753f8-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="753f8-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="753f8-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="753f8-130">Required.</span></span> |

<span data-ttu-id="753f8-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="753f8-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="753f8-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="753f8-132">The default output type is text/csv.</span></span> <span data-ttu-id="753f8-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="753f8-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="753f8-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="753f8-134">Request headers</span></span>

| <span data-ttu-id="753f8-135">Имя</span><span class="sxs-lookup"><span data-stu-id="753f8-135">Name</span></span>          | <span data-ttu-id="753f8-136">Описание</span><span class="sxs-lookup"><span data-stu-id="753f8-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="753f8-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="753f8-137">Authorization</span></span> | <span data-ttu-id="753f8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="753f8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="753f8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="753f8-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="753f8-141">CSV</span><span class="sxs-lookup"><span data-stu-id="753f8-141">CSV</span></span>

<span data-ttu-id="753f8-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="753f8-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="753f8-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="753f8-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="753f8-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="753f8-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="753f8-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="753f8-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="753f8-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="753f8-146">Report Refresh Date</span></span>
- <span data-ttu-id="753f8-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="753f8-147">Report Date</span></span>
- <span data-ttu-id="753f8-148">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="753f8-148">Report Period</span></span>
- <span data-ttu-id="753f8-149">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="753f8-149">IM</span></span>
- <span data-ttu-id="753f8-150">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="753f8-150">Audio/Video</span></span>
- <span data-ttu-id="753f8-151">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="753f8-151">App Sharing</span></span>
- <span data-ttu-id="753f8-152">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="753f8-152">Web</span></span>
- <span data-ttu-id="753f8-153">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="753f8-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="753f8-154">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="753f8-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="753f8-155">JSON</span><span class="sxs-lookup"><span data-stu-id="753f8-155">JSON</span></span>

<span data-ttu-id="753f8-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитюсеркаунтс](../resources/skypeforbusinessorganizeractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="753f8-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="753f8-157">Пример</span><span class="sxs-lookup"><span data-stu-id="753f8-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="753f8-158">CSV</span><span class="sxs-lookup"><span data-stu-id="753f8-158">CSV</span></span>

<span data-ttu-id="753f8-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="753f8-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="753f8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="753f8-160">Request</span></span>

<span data-ttu-id="753f8-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="753f8-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="753f8-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="753f8-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="753f8-163">C#</span><span class="sxs-lookup"><span data-stu-id="753f8-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="753f8-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="753f8-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="753f8-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="753f8-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="753f8-166">Java</span><span class="sxs-lookup"><span data-stu-id="753f8-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="753f8-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="753f8-167">Response</span></span>

<span data-ttu-id="753f8-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="753f8-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="753f8-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="753f8-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="753f8-170">JSON</span><span class="sxs-lookup"><span data-stu-id="753f8-170">JSON</span></span>

<span data-ttu-id="753f8-171">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="753f8-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="753f8-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="753f8-172">Request</span></span>

<span data-ttu-id="753f8-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="753f8-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="753f8-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="753f8-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="753f8-175">C#</span><span class="sxs-lookup"><span data-stu-id="753f8-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="753f8-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="753f8-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="753f8-177">Цель — C</span><span class="sxs-lookup"><span data-stu-id="753f8-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="753f8-178">Java</span><span class="sxs-lookup"><span data-stu-id="753f8-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="753f8-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="753f8-179">Response</span></span>

<span data-ttu-id="753f8-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="753f8-180">The following is an example of the response.</span></span>

> <span data-ttu-id="753f8-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="753f8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityUserCounts)", 
  "value": [
    {
      "im": 37, 
      "audioVideo": 42, 
      "appSharing": 35, 
      "web": 3, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 36, 
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
