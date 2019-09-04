---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 109a0ee1894756b5284956fa1e9151a126723709
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724932"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="cf43f-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cf43f-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf43f-105">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="cf43f-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="cf43f-106">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="cf43f-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf43f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf43f-107">Permissions</span></span>

<span data-ttu-id="cf43f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf43f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf43f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf43f-110">Permission type</span></span>                        | <span data-ttu-id="cf43f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf43f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cf43f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf43f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf43f-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf43f-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cf43f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf43f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf43f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf43f-115">Not supported.</span></span>                           |
| <span data-ttu-id="cf43f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf43f-116">Application</span></span>                            | <span data-ttu-id="cf43f-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf43f-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cf43f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf43f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="cf43f-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cf43f-119">Function parameters</span></span>

<span data-ttu-id="cf43f-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cf43f-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cf43f-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="cf43f-121">Parameter</span></span> | <span data-ttu-id="cf43f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="cf43f-122">Type</span></span>   | <span data-ttu-id="cf43f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cf43f-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cf43f-124">period</span><span class="sxs-lookup"><span data-stu-id="cf43f-124">period</span></span>    | <span data-ttu-id="cf43f-125">string</span><span class="sxs-lookup"><span data-stu-id="cf43f-125">string</span></span> | <span data-ttu-id="cf43f-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cf43f-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cf43f-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="cf43f-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cf43f-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cf43f-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cf43f-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf43f-129">Required.</span></span> |

<span data-ttu-id="cf43f-130">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cf43f-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cf43f-131">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="cf43f-131">The default output type is text/csv.</span></span> <span data-ttu-id="cf43f-132">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="cf43f-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf43f-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf43f-133">Request headers</span></span>

| <span data-ttu-id="cf43f-134">Имя</span><span class="sxs-lookup"><span data-stu-id="cf43f-134">Name</span></span>          | <span data-ttu-id="cf43f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="cf43f-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cf43f-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf43f-136">Authorization</span></span> | <span data-ttu-id="cf43f-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf43f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cf43f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf43f-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cf43f-140">CSV</span><span class="sxs-lookup"><span data-stu-id="cf43f-140">CSV</span></span>

<span data-ttu-id="cf43f-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cf43f-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cf43f-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cf43f-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cf43f-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cf43f-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cf43f-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cf43f-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cf43f-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cf43f-145">Report Refresh Date</span></span>
- <span data-ttu-id="cf43f-146">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="cf43f-146">Report Date</span></span>
- <span data-ttu-id="cf43f-147">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="cf43f-147">Team Chat Messages</span></span>
- <span data-ttu-id="cf43f-148">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="cf43f-148">Private Chat Messages</span></span>
- <span data-ttu-id="cf43f-149">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="cf43f-149">Calls</span></span>
- <span data-ttu-id="cf43f-150">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="cf43f-150">Meetings</span></span>
- <span data-ttu-id="cf43f-151">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="cf43f-151">Other Actions</span></span>
- <span data-ttu-id="cf43f-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="cf43f-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cf43f-153">JSON</span><span class="sxs-lookup"><span data-stu-id="cf43f-153">JSON</span></span>

<span data-ttu-id="cf43f-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсусерактивитюсеркаунтс](../resources/teamsuseractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf43f-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf43f-155">Пример</span><span class="sxs-lookup"><span data-stu-id="cf43f-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cf43f-156">CSV</span><span class="sxs-lookup"><span data-stu-id="cf43f-156">CSV</span></span>

<span data-ttu-id="cf43f-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="cf43f-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cf43f-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf43f-158">Request</span></span>

<span data-ttu-id="cf43f-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf43f-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cf43f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf43f-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf43f-161">C#</span><span class="sxs-lookup"><span data-stu-id="cf43f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf43f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf43f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf43f-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cf43f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf43f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf43f-164">Response</span></span>

<span data-ttu-id="cf43f-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf43f-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cf43f-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cf43f-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="cf43f-167">JSON</span><span class="sxs-lookup"><span data-stu-id="cf43f-167">JSON</span></span>

<span data-ttu-id="cf43f-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="cf43f-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cf43f-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf43f-169">Request</span></span>

<span data-ttu-id="cf43f-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf43f-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cf43f-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf43f-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf43f-172">C#</span><span class="sxs-lookup"><span data-stu-id="cf43f-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf43f-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf43f-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf43f-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cf43f-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf43f-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf43f-175">Response</span></span>

<span data-ttu-id="cf43f-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf43f-176">The following is an example of the response.</span></span>

> <span data-ttu-id="cf43f-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf43f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
