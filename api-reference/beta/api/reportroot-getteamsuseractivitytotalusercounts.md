---
title: 'reportRoot: getTeamsUserActivityTotalUserCounts'
description: Получите число пользователей, Microsoft Teams лицензированных или не лицензированных пользователей по типу действия. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a534070cf178f93fe999728893ab5de5e707d9ab
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055003"
---
# <a name="reportroot-getteamsuseractivitytotalusercounts"></a><span data-ttu-id="58e2f-104">reportRoot: getTeamsUserActivityTotalUserCounts</span><span class="sxs-lookup"><span data-stu-id="58e2f-104">reportRoot: getTeamsUserActivityTotalUserCounts</span></span>

<span data-ttu-id="58e2f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58e2f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e2f-106">Получите число пользователей, Microsoft Teams лицензированных или не лицензированных пользователей по типу действия.</span><span class="sxs-lookup"><span data-stu-id="58e2f-106">Get the number of Microsoft Teams licensed or non-licensed users by activity type.</span></span> <span data-ttu-id="58e2f-107">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="58e2f-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="58e2f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58e2f-108">Permissions</span></span>

<span data-ttu-id="58e2f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58e2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e2f-111">Permission type</span></span>                        | <span data-ttu-id="58e2f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e2f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="58e2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e2f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="58e2f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e2f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="58e2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e2f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e2f-116">Not supported.</span></span>                           |
| <span data-ttu-id="58e2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58e2f-117">Application</span></span>                            | <span data-ttu-id="58e2f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e2f-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="58e2f-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="58e2f-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="58e2f-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="58e2f-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="58e2f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e2f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="58e2f-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="58e2f-122">Function parameters</span></span>

<span data-ttu-id="58e2f-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="58e2f-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="58e2f-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="58e2f-124">Parameter</span></span> | <span data-ttu-id="58e2f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="58e2f-125">Type</span></span>   | <span data-ttu-id="58e2f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="58e2f-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="58e2f-127">period</span><span class="sxs-lookup"><span data-stu-id="58e2f-127">period</span></span>    | <span data-ttu-id="58e2f-128">string</span><span class="sxs-lookup"><span data-stu-id="58e2f-128">string</span></span> | <span data-ttu-id="58e2f-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="58e2f-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="58e2f-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="58e2f-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="58e2f-131">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="58e2f-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="58e2f-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58e2f-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="58e2f-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58e2f-133">Optional query parameters</span></span>

<span data-ttu-id="58e2f-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="58e2f-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="58e2f-135">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="58e2f-135">The default output type is text/csv.</span></span> <span data-ttu-id="58e2f-136">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, заданный для `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="58e2f-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58e2f-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58e2f-137">Request headers</span></span>

| <span data-ttu-id="58e2f-138">Имя</span><span class="sxs-lookup"><span data-stu-id="58e2f-138">Name</span></span>          | <span data-ttu-id="58e2f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="58e2f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="58e2f-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58e2f-140">Authorization</span></span> | <span data-ttu-id="58e2f-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58e2f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="58e2f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e2f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="58e2f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="58e2f-144">CSV</span></span>

<span data-ttu-id="58e2f-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="58e2f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="58e2f-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="58e2f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="58e2f-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="58e2f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="58e2f-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="58e2f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="58e2f-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="58e2f-149">Report Refresh Date</span></span>
- <span data-ttu-id="58e2f-150">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="58e2f-150">Report Date</span></span>
- <span data-ttu-id="58e2f-151">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="58e2f-151">Team Chat Messages</span></span>
- <span data-ttu-id="58e2f-152">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="58e2f-152">Private Chat Messages</span></span>
- <span data-ttu-id="58e2f-153">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="58e2f-153">Calls</span></span>
- <span data-ttu-id="58e2f-154">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="58e2f-154">Meetings</span></span>
- <span data-ttu-id="58e2f-155">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="58e2f-155">Other Actions</span></span>
- <span data-ttu-id="58e2f-156">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="58e2f-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="58e2f-157">JSON</span><span class="sxs-lookup"><span data-stu-id="58e2f-157">JSON</span></span>

<span data-ttu-id="58e2f-158">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="58e2f-158">If successful, this method returns a `200 OK` response code and a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e2f-159">Пример</span><span class="sxs-lookup"><span data-stu-id="58e2f-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="58e2f-160">CSV</span><span class="sxs-lookup"><span data-stu-id="58e2f-160">CSV</span></span>

<span data-ttu-id="58e2f-161">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="58e2f-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="58e2f-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e2f-162">Request</span></span>

<span data-ttu-id="58e2f-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58e2f-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="58e2f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e2f-164">Response</span></span>

<span data-ttu-id="58e2f-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58e2f-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="58e2f-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="58e2f-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="58e2f-167">JSON</span><span class="sxs-lookup"><span data-stu-id="58e2f-167">JSON</span></span>

<span data-ttu-id="58e2f-168">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="58e2f-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="58e2f-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e2f-169">Request</span></span>

<span data-ttu-id="58e2f-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58e2f-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="58e2f-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e2f-171">Response</span></span>

<span data-ttu-id="58e2f-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58e2f-172">The following is an example of the response.</span></span>

> <span data-ttu-id="58e2f-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="58e2f-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
