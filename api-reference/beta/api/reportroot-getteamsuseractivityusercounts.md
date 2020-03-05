---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3184bdaa59f5203f3d3f3630ed8477de55c91d44
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454027"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="4536d-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="4536d-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="4536d-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4536d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4536d-106">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="4536d-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="4536d-107">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="4536d-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="4536d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4536d-108">Permissions</span></span>

<span data-ttu-id="4536d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4536d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4536d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4536d-111">Permission type</span></span>                        | <span data-ttu-id="4536d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4536d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4536d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4536d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4536d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4536d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4536d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4536d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4536d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4536d-116">Not supported.</span></span>                           |
| <span data-ttu-id="4536d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4536d-117">Application</span></span>                            | <span data-ttu-id="4536d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4536d-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="4536d-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4536d-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4536d-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4536d-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4536d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4536d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="4536d-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4536d-122">Function parameters</span></span>

<span data-ttu-id="4536d-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4536d-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4536d-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="4536d-124">Parameter</span></span> | <span data-ttu-id="4536d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4536d-125">Type</span></span>   | <span data-ttu-id="4536d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4536d-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4536d-127">period</span><span class="sxs-lookup"><span data-stu-id="4536d-127">period</span></span>    | <span data-ttu-id="4536d-128">string</span><span class="sxs-lookup"><span data-stu-id="4536d-128">string</span></span> | <span data-ttu-id="4536d-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4536d-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4536d-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4536d-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4536d-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4536d-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4536d-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4536d-132">Required.</span></span> |

<span data-ttu-id="4536d-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4536d-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4536d-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4536d-134">The default output type is text/csv.</span></span> <span data-ttu-id="4536d-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4536d-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4536d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4536d-136">Request headers</span></span>

| <span data-ttu-id="4536d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="4536d-137">Name</span></span>          | <span data-ttu-id="4536d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4536d-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4536d-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4536d-139">Authorization</span></span> | <span data-ttu-id="4536d-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4536d-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4536d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4536d-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4536d-143">CSV</span><span class="sxs-lookup"><span data-stu-id="4536d-143">CSV</span></span>

<span data-ttu-id="4536d-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4536d-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4536d-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4536d-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4536d-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4536d-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4536d-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4536d-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4536d-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4536d-148">Report Refresh Date</span></span>
- <span data-ttu-id="4536d-149">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4536d-149">Report Date</span></span>
- <span data-ttu-id="4536d-150">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="4536d-150">Team Chat Messages</span></span>
- <span data-ttu-id="4536d-151">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="4536d-151">Private Chat Messages</span></span>
- <span data-ttu-id="4536d-152">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="4536d-152">Calls</span></span>
- <span data-ttu-id="4536d-153">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="4536d-153">Meetings</span></span>
- <span data-ttu-id="4536d-154">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="4536d-154">Other Actions</span></span>
- <span data-ttu-id="4536d-155">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4536d-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4536d-156">JSON</span><span class="sxs-lookup"><span data-stu-id="4536d-156">JSON</span></span>

<span data-ttu-id="4536d-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсусерактивитюсеркаунтс](../resources/teamsuseractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4536d-157">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4536d-158">Пример</span><span class="sxs-lookup"><span data-stu-id="4536d-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4536d-159">CSV</span><span class="sxs-lookup"><span data-stu-id="4536d-159">CSV</span></span>

<span data-ttu-id="4536d-160">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4536d-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4536d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4536d-161">Request</span></span>

<span data-ttu-id="4536d-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4536d-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4536d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="4536d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="4536d-164">C#</span><span class="sxs-lookup"><span data-stu-id="4536d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4536d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4536d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4536d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4536d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4536d-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4536d-167">Response</span></span>

<span data-ttu-id="4536d-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4536d-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4536d-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4536d-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4536d-170">JSON</span><span class="sxs-lookup"><span data-stu-id="4536d-170">JSON</span></span>

<span data-ttu-id="4536d-171">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4536d-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4536d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4536d-172">Request</span></span>

<span data-ttu-id="4536d-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4536d-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4536d-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="4536d-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="4536d-175">C#</span><span class="sxs-lookup"><span data-stu-id="4536d-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4536d-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4536d-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4536d-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4536d-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4536d-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="4536d-178">Response</span></span>

<span data-ttu-id="4536d-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4536d-179">The following is an example of the response.</span></span>

> <span data-ttu-id="4536d-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4536d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
