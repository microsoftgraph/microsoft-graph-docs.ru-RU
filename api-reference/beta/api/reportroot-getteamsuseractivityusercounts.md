---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 60e20a603f663bd20fcd94cc08535bb93f9cfa60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983115"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="c550a-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c550a-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c550a-105">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="c550a-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="c550a-106">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="c550a-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="c550a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c550a-107">Permissions</span></span>

<span data-ttu-id="c550a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c550a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c550a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c550a-110">Permission type</span></span>                        | <span data-ttu-id="c550a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c550a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c550a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c550a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c550a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c550a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c550a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c550a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c550a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c550a-115">Not supported.</span></span>                           |
| <span data-ttu-id="c550a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c550a-116">Application</span></span>                            | <span data-ttu-id="c550a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c550a-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c550a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c550a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="c550a-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c550a-119">Function parameters</span></span>

<span data-ttu-id="c550a-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c550a-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c550a-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="c550a-121">Parameter</span></span> | <span data-ttu-id="c550a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c550a-122">Type</span></span>   | <span data-ttu-id="c550a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c550a-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c550a-124">period</span><span class="sxs-lookup"><span data-stu-id="c550a-124">period</span></span>    | <span data-ttu-id="c550a-125">string</span><span class="sxs-lookup"><span data-stu-id="c550a-125">string</span></span> | <span data-ttu-id="c550a-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c550a-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c550a-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c550a-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c550a-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c550a-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c550a-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c550a-129">Required.</span></span> |

<span data-ttu-id="c550a-130">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c550a-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c550a-131">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c550a-131">The default output type is text/csv.</span></span> <span data-ttu-id="c550a-132">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c550a-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c550a-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c550a-133">Request headers</span></span>

| <span data-ttu-id="c550a-134">Имя</span><span class="sxs-lookup"><span data-stu-id="c550a-134">Name</span></span>          | <span data-ttu-id="c550a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c550a-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c550a-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c550a-136">Authorization</span></span> | <span data-ttu-id="c550a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c550a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c550a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c550a-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c550a-140">CSV</span><span class="sxs-lookup"><span data-stu-id="c550a-140">CSV</span></span>

<span data-ttu-id="c550a-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c550a-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c550a-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c550a-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c550a-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c550a-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c550a-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c550a-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c550a-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c550a-145">Report Refresh Date</span></span>
- <span data-ttu-id="c550a-146">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c550a-146">Report Date</span></span>
- <span data-ttu-id="c550a-147">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="c550a-147">Team Chat Messages</span></span>
- <span data-ttu-id="c550a-148">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="c550a-148">Private Chat Messages</span></span>
- <span data-ttu-id="c550a-149">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="c550a-149">Calls</span></span>
- <span data-ttu-id="c550a-150">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="c550a-150">Meetings</span></span>
- <span data-ttu-id="c550a-151">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="c550a-151">Other Actions</span></span>
- <span data-ttu-id="c550a-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c550a-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c550a-153">JSON</span><span class="sxs-lookup"><span data-stu-id="c550a-153">JSON</span></span>

<span data-ttu-id="c550a-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсусерактивитюсеркаунтс](../resources/teamsuseractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c550a-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c550a-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c550a-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c550a-156">CSV</span><span class="sxs-lookup"><span data-stu-id="c550a-156">CSV</span></span>

<span data-ttu-id="c550a-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c550a-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c550a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c550a-158">Request</span></span>

<span data-ttu-id="c550a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c550a-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c550a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c550a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c550a-161">C#</span><span class="sxs-lookup"><span data-stu-id="c550a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c550a-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="c550a-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c550a-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c550a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c550a-164">Java</span><span class="sxs-lookup"><span data-stu-id="c550a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c550a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c550a-165">Response</span></span>

<span data-ttu-id="c550a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c550a-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c550a-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c550a-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a><span data-ttu-id="c550a-168">JSON</span><span class="sxs-lookup"><span data-stu-id="c550a-168">JSON</span></span>

<span data-ttu-id="c550a-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c550a-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c550a-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c550a-170">Request</span></span>

<span data-ttu-id="c550a-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c550a-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c550a-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c550a-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c550a-173">C#</span><span class="sxs-lookup"><span data-stu-id="c550a-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c550a-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="c550a-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c550a-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c550a-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c550a-176">Java</span><span class="sxs-lookup"><span data-stu-id="c550a-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c550a-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c550a-177">Response</span></span>

<span data-ttu-id="c550a-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c550a-178">The following is an example of the response.</span></span>

> <span data-ttu-id="c550a-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c550a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
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
