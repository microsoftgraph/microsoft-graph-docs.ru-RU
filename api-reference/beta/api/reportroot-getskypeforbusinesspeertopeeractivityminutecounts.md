---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c5aa11b4f80c2c6bfd635f77ac99c2bf96c27b59
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867346"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="ccc96-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="ccc96-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccc96-105">Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов</span><span class="sxs-lookup"><span data-stu-id="ccc96-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="ccc96-106">(аудио и видео).</span><span class="sxs-lookup"><span data-stu-id="ccc96-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="ccc96-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="ccc96-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc96-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc96-108">Permissions</span></span>

<span data-ttu-id="ccc96-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccc96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccc96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc96-111">Permission type</span></span>                        | <span data-ttu-id="ccc96-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccc96-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ccc96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccc96-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccc96-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccc96-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ccc96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccc96-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccc96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccc96-116">Not supported.</span></span>                           |
| <span data-ttu-id="ccc96-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccc96-117">Application</span></span>                            | <span data-ttu-id="ccc96-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccc96-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="ccc96-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ccc96-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ccc96-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ccc96-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ccc96-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccc96-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ccc96-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ccc96-122">Function parameters</span></span>

<span data-ttu-id="ccc96-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ccc96-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ccc96-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="ccc96-124">Parameter</span></span> | <span data-ttu-id="ccc96-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ccc96-125">Type</span></span>   | <span data-ttu-id="ccc96-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc96-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ccc96-127">period</span><span class="sxs-lookup"><span data-stu-id="ccc96-127">period</span></span>    | <span data-ttu-id="ccc96-128">string</span><span class="sxs-lookup"><span data-stu-id="ccc96-128">string</span></span> | <span data-ttu-id="ccc96-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ccc96-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ccc96-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ccc96-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ccc96-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ccc96-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ccc96-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccc96-132">Required.</span></span> |

<span data-ttu-id="ccc96-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ccc96-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ccc96-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ccc96-134">The default output type is text/csv.</span></span> <span data-ttu-id="ccc96-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ccc96-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccc96-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccc96-136">Request headers</span></span>

| <span data-ttu-id="ccc96-137">Имя</span><span class="sxs-lookup"><span data-stu-id="ccc96-137">Name</span></span>          | <span data-ttu-id="ccc96-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc96-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ccc96-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccc96-139">Authorization</span></span> | <span data-ttu-id="ccc96-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccc96-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ccc96-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc96-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ccc96-143">CSV</span><span class="sxs-lookup"><span data-stu-id="ccc96-143">CSV</span></span>

<span data-ttu-id="ccc96-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ccc96-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ccc96-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ccc96-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ccc96-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ccc96-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ccc96-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ccc96-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ccc96-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ccc96-148">Report Refresh Date</span></span>
- <span data-ttu-id="ccc96-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="ccc96-149">Report Date</span></span>
- <span data-ttu-id="ccc96-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="ccc96-150">Report Period</span></span>
- <span data-ttu-id="ccc96-151">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="ccc96-151">Audio</span></span>
- <span data-ttu-id="ccc96-152">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="ccc96-152">Video</span></span>

### <a name="json"></a><span data-ttu-id="ccc96-153">JSON</span><span class="sxs-lookup"><span data-stu-id="ccc96-153">JSON</span></span>

<span data-ttu-id="ccc96-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспиртопирактивитиминутекаунтс](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccc96-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccc96-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ccc96-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ccc96-156">CSV</span><span class="sxs-lookup"><span data-stu-id="ccc96-156">CSV</span></span>

<span data-ttu-id="ccc96-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ccc96-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ccc96-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc96-158">Request</span></span>

<span data-ttu-id="ccc96-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccc96-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ccc96-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc96-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccc96-161">C#</span><span class="sxs-lookup"><span data-stu-id="ccc96-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccc96-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc96-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccc96-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc96-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccc96-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc96-164">Response</span></span>

<span data-ttu-id="ccc96-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccc96-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ccc96-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ccc96-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ccc96-167">JSON</span><span class="sxs-lookup"><span data-stu-id="ccc96-167">JSON</span></span>

<span data-ttu-id="ccc96-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ccc96-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ccc96-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc96-169">Request</span></span>

<span data-ttu-id="ccc96-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccc96-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ccc96-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc96-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccc96-172">C#</span><span class="sxs-lookup"><span data-stu-id="ccc96-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccc96-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc96-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccc96-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc96-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccc96-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc96-175">Response</span></span>

<span data-ttu-id="ccc96-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccc96-176">The following is an example of the response.</span></span>

> <span data-ttu-id="ccc96-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccc96-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
