---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a260121c66a8aff080a39d0f581c20a4fc240cad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454082"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="09e33-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="09e33-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="09e33-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09e33-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e33-106">Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов</span><span class="sxs-lookup"><span data-stu-id="09e33-106">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="09e33-107">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).</span><span class="sxs-lookup"><span data-stu-id="09e33-107">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="09e33-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="09e33-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="09e33-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09e33-109">Permissions</span></span>

<span data-ttu-id="09e33-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09e33-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09e33-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09e33-112">Permission type</span></span>                        | <span data-ttu-id="09e33-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09e33-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="09e33-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09e33-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="09e33-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e33-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="09e33-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09e33-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09e33-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09e33-117">Not supported.</span></span>                           |
| <span data-ttu-id="09e33-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09e33-118">Application</span></span>                            | <span data-ttu-id="09e33-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e33-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="09e33-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09e33-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="09e33-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="09e33-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="09e33-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09e33-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="09e33-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="09e33-123">Function parameters</span></span>

<span data-ttu-id="09e33-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="09e33-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="09e33-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="09e33-125">Parameter</span></span> | <span data-ttu-id="09e33-126">Тип</span><span class="sxs-lookup"><span data-stu-id="09e33-126">Type</span></span>   | <span data-ttu-id="09e33-127">Описание</span><span class="sxs-lookup"><span data-stu-id="09e33-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="09e33-128">period</span><span class="sxs-lookup"><span data-stu-id="09e33-128">period</span></span>    | <span data-ttu-id="09e33-129">string</span><span class="sxs-lookup"><span data-stu-id="09e33-129">string</span></span> | <span data-ttu-id="09e33-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="09e33-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="09e33-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="09e33-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="09e33-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="09e33-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="09e33-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09e33-133">Required.</span></span> |

<span data-ttu-id="09e33-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="09e33-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="09e33-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="09e33-135">The default output type is text/csv.</span></span> <span data-ttu-id="09e33-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="09e33-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09e33-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09e33-137">Request headers</span></span>

| <span data-ttu-id="09e33-138">Имя</span><span class="sxs-lookup"><span data-stu-id="09e33-138">Name</span></span>          | <span data-ttu-id="09e33-139">Описание</span><span class="sxs-lookup"><span data-stu-id="09e33-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="09e33-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09e33-140">Authorization</span></span> | <span data-ttu-id="09e33-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09e33-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="09e33-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="09e33-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="09e33-144">CSV</span><span class="sxs-lookup"><span data-stu-id="09e33-144">CSV</span></span>

<span data-ttu-id="09e33-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="09e33-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="09e33-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="09e33-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="09e33-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="09e33-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="09e33-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="09e33-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="09e33-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="09e33-149">Report Refresh Date</span></span>
- <span data-ttu-id="09e33-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="09e33-150">Report Date</span></span>
- <span data-ttu-id="09e33-151">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="09e33-151">Report Period</span></span>
- <span data-ttu-id="09e33-152">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="09e33-152">IM</span></span>
- <span data-ttu-id="09e33-153">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="09e33-153">Audio</span></span>
- <span data-ttu-id="09e33-154">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="09e33-154">Video</span></span>
- <span data-ttu-id="09e33-155">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="09e33-155">App Sharing</span></span>
- <span data-ttu-id="09e33-156">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="09e33-156">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="09e33-157">JSON</span><span class="sxs-lookup"><span data-stu-id="09e33-157">JSON</span></span>

<span data-ttu-id="09e33-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинесспиртопирактивитикаунтс](../resources/skypeforbusinesspeertopeeractivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09e33-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e33-159">Пример</span><span class="sxs-lookup"><span data-stu-id="09e33-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="09e33-160">CSV</span><span class="sxs-lookup"><span data-stu-id="09e33-160">CSV</span></span>

<span data-ttu-id="09e33-161">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="09e33-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="09e33-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="09e33-162">Request</span></span>

<span data-ttu-id="09e33-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09e33-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="09e33-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="09e33-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="09e33-165">C#</span><span class="sxs-lookup"><span data-stu-id="09e33-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09e33-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09e33-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09e33-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09e33-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="09e33-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="09e33-168">Response</span></span>

<span data-ttu-id="09e33-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09e33-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="09e33-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="09e33-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="09e33-171">JSON</span><span class="sxs-lookup"><span data-stu-id="09e33-171">JSON</span></span>

<span data-ttu-id="09e33-172">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="09e33-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="09e33-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="09e33-173">Request</span></span>

<span data-ttu-id="09e33-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09e33-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="09e33-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="09e33-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="09e33-176">C#</span><span class="sxs-lookup"><span data-stu-id="09e33-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09e33-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09e33-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09e33-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09e33-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="09e33-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="09e33-179">Response</span></span>

<span data-ttu-id="09e33-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09e33-180">The following is an example of the response.</span></span>

> <span data-ttu-id="09e33-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09e33-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
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
