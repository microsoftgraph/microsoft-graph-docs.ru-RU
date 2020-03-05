---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5aec1d1def6af4099f7d28f80e1d0bd787716733
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454131"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="5bbe9-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="5bbe9-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="5bbe9-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5bbe9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bbe9-106">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="5bbe9-106">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="5bbe9-107">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="5bbe9-107">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="5bbe9-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="5bbe9-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="5bbe9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bbe9-109">Permissions</span></span>

<span data-ttu-id="5bbe9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bbe9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bbe9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bbe9-112">Permission type</span></span>                        | <span data-ttu-id="5bbe9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bbe9-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5bbe9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bbe9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bbe9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bbe9-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5bbe9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bbe9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bbe9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-117">Not supported.</span></span>                           |
| <span data-ttu-id="5bbe9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bbe9-118">Application</span></span>                            | <span data-ttu-id="5bbe9-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bbe9-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="5bbe9-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5bbe9-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5bbe9-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5bbe9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bbe9-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5bbe9-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5bbe9-123">Function parameters</span></span>

<span data-ttu-id="5bbe9-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5bbe9-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="5bbe9-125">Parameter</span></span> | <span data-ttu-id="5bbe9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5bbe9-126">Type</span></span>   | <span data-ttu-id="5bbe9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5bbe9-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5bbe9-128">period</span><span class="sxs-lookup"><span data-stu-id="5bbe9-128">period</span></span>    | <span data-ttu-id="5bbe9-129">string</span><span class="sxs-lookup"><span data-stu-id="5bbe9-129">string</span></span> | <span data-ttu-id="5bbe9-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5bbe9-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5bbe9-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5bbe9-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-133">Required.</span></span> |

<span data-ttu-id="5bbe9-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5bbe9-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-135">The default output type is text/csv.</span></span> <span data-ttu-id="5bbe9-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bbe9-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bbe9-137">Request headers</span></span>

| <span data-ttu-id="5bbe9-138">Имя</span><span class="sxs-lookup"><span data-stu-id="5bbe9-138">Name</span></span>          | <span data-ttu-id="5bbe9-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5bbe9-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5bbe9-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bbe9-140">Authorization</span></span> | <span data-ttu-id="5bbe9-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5bbe9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbe9-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5bbe9-144">CSV</span><span class="sxs-lookup"><span data-stu-id="5bbe9-144">CSV</span></span>

<span data-ttu-id="5bbe9-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5bbe9-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5bbe9-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5bbe9-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5bbe9-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5bbe9-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5bbe9-149">Report Refresh Date</span></span>
- <span data-ttu-id="5bbe9-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="5bbe9-150">Report Date</span></span>
- <span data-ttu-id="5bbe9-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="5bbe9-151">Report Period</span></span>
- <span data-ttu-id="5bbe9-152">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="5bbe9-152">Audio</span></span>
- <span data-ttu-id="5bbe9-153">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="5bbe9-153">Video</span></span>

### <a name="json"></a><span data-ttu-id="5bbe9-154">JSON</span><span class="sxs-lookup"><span data-stu-id="5bbe9-154">JSON</span></span>

<span data-ttu-id="5bbe9-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспиртопирактивитиминутекаунтс](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bbe9-156">Пример</span><span class="sxs-lookup"><span data-stu-id="5bbe9-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5bbe9-157">CSV</span><span class="sxs-lookup"><span data-stu-id="5bbe9-157">CSV</span></span>

<span data-ttu-id="5bbe9-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5bbe9-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbe9-159">Request</span></span>

<span data-ttu-id="5bbe9-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bbe9-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bbe9-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="5bbe9-162">C#</span><span class="sxs-lookup"><span data-stu-id="5bbe9-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bbe9-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bbe9-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bbe9-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bbe9-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bbe9-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbe9-165">Response</span></span>

<span data-ttu-id="5bbe9-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5bbe9-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5bbe9-168">JSON</span><span class="sxs-lookup"><span data-stu-id="5bbe9-168">JSON</span></span>

<span data-ttu-id="5bbe9-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5bbe9-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbe9-170">Request</span></span>

<span data-ttu-id="5bbe9-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bbe9-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bbe9-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="5bbe9-173">C#</span><span class="sxs-lookup"><span data-stu-id="5bbe9-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bbe9-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bbe9-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bbe9-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bbe9-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bbe9-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbe9-176">Response</span></span>

<span data-ttu-id="5bbe9-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-177">The following is an example of the response.</span></span>

> <span data-ttu-id="5bbe9-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bbe9-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
