---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5536fc6bc7ef1ee97f5480d4d99778daf889a134
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454124"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="12fef-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="12fef-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="12fef-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12fef-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12fef-106">Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных и организованных конференций</span><span class="sxs-lookup"><span data-stu-id="12fef-106">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="12fef-107">Типы сеансов конференц-связи включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="12fef-107">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="12fef-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="12fef-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="12fef-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12fef-109">Permissions</span></span>

<span data-ttu-id="12fef-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12fef-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fef-112">Permission type</span></span>                        | <span data-ttu-id="12fef-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fef-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="12fef-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fef-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="12fef-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="12fef-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="12fef-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fef-117">Not supported.</span></span>                           |
| <span data-ttu-id="12fef-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fef-118">Application</span></span>                            | <span data-ttu-id="12fef-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="12fef-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="12fef-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="12fef-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="12fef-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="12fef-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="12fef-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fef-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="12fef-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="12fef-123">Function parameters</span></span>

<span data-ttu-id="12fef-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="12fef-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="12fef-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="12fef-125">Parameter</span></span> | <span data-ttu-id="12fef-126">Тип</span><span class="sxs-lookup"><span data-stu-id="12fef-126">Type</span></span>   | <span data-ttu-id="12fef-127">Описание</span><span class="sxs-lookup"><span data-stu-id="12fef-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="12fef-128">period</span><span class="sxs-lookup"><span data-stu-id="12fef-128">period</span></span>    | <span data-ttu-id="12fef-129">string</span><span class="sxs-lookup"><span data-stu-id="12fef-129">string</span></span> | <span data-ttu-id="12fef-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="12fef-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="12fef-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="12fef-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="12fef-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="12fef-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="12fef-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fef-133">Required.</span></span> |

<span data-ttu-id="12fef-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="12fef-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="12fef-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="12fef-135">The default output type is text/csv.</span></span> <span data-ttu-id="12fef-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="12fef-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12fef-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12fef-137">Request headers</span></span>

| <span data-ttu-id="12fef-138">Имя</span><span class="sxs-lookup"><span data-stu-id="12fef-138">Name</span></span>          | <span data-ttu-id="12fef-139">Описание</span><span class="sxs-lookup"><span data-stu-id="12fef-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="12fef-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12fef-140">Authorization</span></span> | <span data-ttu-id="12fef-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fef-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="12fef-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fef-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="12fef-144">CSV</span><span class="sxs-lookup"><span data-stu-id="12fef-144">CSV</span></span>

<span data-ttu-id="12fef-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="12fef-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="12fef-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="12fef-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="12fef-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="12fef-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="12fef-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="12fef-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="12fef-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="12fef-149">Report Refresh Date</span></span>
- <span data-ttu-id="12fef-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="12fef-150">Report Date</span></span>
- <span data-ttu-id="12fef-151">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="12fef-151">Report Period</span></span>
- <span data-ttu-id="12fef-152">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="12fef-152">IM</span></span>
- <span data-ttu-id="12fef-153">"Audio/Video" (Аудио и видео);</span><span class="sxs-lookup"><span data-stu-id="12fef-153">Audio/Video</span></span>
- <span data-ttu-id="12fef-154">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="12fef-154">App Sharing</span></span>
- <span data-ttu-id="12fef-155">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="12fef-155">Web</span></span>
- <span data-ttu-id="12fef-156">"Dial-in/out 3rd Party" (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба);</span><span class="sxs-lookup"><span data-stu-id="12fef-156">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="12fef-157">"Dial-in/out Microsoft" (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="12fef-157">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="12fef-158">JSON</span><span class="sxs-lookup"><span data-stu-id="12fef-158">JSON</span></span>

<span data-ttu-id="12fef-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессорганизерактивитюсеркаунтс](../resources/skypeforbusinessorganizeractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12fef-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fef-160">Пример</span><span class="sxs-lookup"><span data-stu-id="12fef-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="12fef-161">CSV</span><span class="sxs-lookup"><span data-stu-id="12fef-161">CSV</span></span>

<span data-ttu-id="12fef-162">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="12fef-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="12fef-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fef-163">Request</span></span>

<span data-ttu-id="12fef-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fef-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="12fef-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="12fef-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="12fef-166">C#</span><span class="sxs-lookup"><span data-stu-id="12fef-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12fef-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12fef-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12fef-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12fef-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="12fef-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fef-169">Response</span></span>

<span data-ttu-id="12fef-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12fef-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="12fef-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="12fef-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="12fef-172">JSON</span><span class="sxs-lookup"><span data-stu-id="12fef-172">JSON</span></span>

<span data-ttu-id="12fef-173">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="12fef-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="12fef-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fef-174">Request</span></span>

<span data-ttu-id="12fef-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fef-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="12fef-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="12fef-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="12fef-177">C#</span><span class="sxs-lookup"><span data-stu-id="12fef-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12fef-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12fef-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12fef-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12fef-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="12fef-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fef-180">Response</span></span>

<span data-ttu-id="12fef-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12fef-181">The following is an example of the response.</span></span>

> <span data-ttu-id="12fef-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12fef-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
