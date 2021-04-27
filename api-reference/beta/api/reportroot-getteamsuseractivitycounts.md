---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Получение количества действий в Microsoft Teams по каждому типу. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. Действия выполняются Microsoft Teams лицензированными пользователями.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: be6fd27c9e4b99e8d8311bf9f60e2ee057ac4ce2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049046"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="712e5-105">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="712e5-105">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="712e5-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="712e5-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="712e5-107">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="712e5-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="712e5-108">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="712e5-108">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span> <span data-ttu-id="712e5-109">Действия выполняются Microsoft Teams лицензированными пользователями.</span><span class="sxs-lookup"><span data-stu-id="712e5-109">The activities are performed by Microsoft Teams licensed users.</span></span>

## <a name="permissions"></a><span data-ttu-id="712e5-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="712e5-110">Permissions</span></span>

<span data-ttu-id="712e5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="712e5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="712e5-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="712e5-113">Permission type</span></span>                        | <span data-ttu-id="712e5-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="712e5-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="712e5-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="712e5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="712e5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="712e5-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="712e5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="712e5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="712e5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="712e5-118">Not supported.</span></span>                           |
| <span data-ttu-id="712e5-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="712e5-119">Application</span></span>                            | <span data-ttu-id="712e5-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="712e5-120">Reports.Read.All</span></span>                         |

<span data-ttu-id="712e5-121">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="712e5-121">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="712e5-122">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="712e5-122">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="712e5-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="712e5-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="712e5-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="712e5-124">Function parameters</span></span>

<span data-ttu-id="712e5-125">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="712e5-125">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="712e5-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="712e5-126">Parameter</span></span> | <span data-ttu-id="712e5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="712e5-127">Type</span></span>   | <span data-ttu-id="712e5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="712e5-128">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="712e5-129">period</span><span class="sxs-lookup"><span data-stu-id="712e5-129">period</span></span>    | <span data-ttu-id="712e5-130">string</span><span class="sxs-lookup"><span data-stu-id="712e5-130">string</span></span> | <span data-ttu-id="712e5-131">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="712e5-131">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="712e5-132">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="712e5-132">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="712e5-133">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="712e5-133">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="712e5-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="712e5-134">Required.</span></span> |

<span data-ttu-id="712e5-135">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="712e5-135">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="712e5-136">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="712e5-136">The default output type is text/csv.</span></span> <span data-ttu-id="712e5-137">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="712e5-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="712e5-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="712e5-138">Request headers</span></span>

| <span data-ttu-id="712e5-139">Имя</span><span class="sxs-lookup"><span data-stu-id="712e5-139">Name</span></span>          | <span data-ttu-id="712e5-140">Описание</span><span class="sxs-lookup"><span data-stu-id="712e5-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="712e5-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="712e5-141">Authorization</span></span> | <span data-ttu-id="712e5-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="712e5-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="712e5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="712e5-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="712e5-145">CSV</span><span class="sxs-lookup"><span data-stu-id="712e5-145">CSV</span></span>

<span data-ttu-id="712e5-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="712e5-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="712e5-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="712e5-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="712e5-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="712e5-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="712e5-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="712e5-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="712e5-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="712e5-150">Report Refresh Date</span></span>
- <span data-ttu-id="712e5-151">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="712e5-151">Report Date</span></span>
- <span data-ttu-id="712e5-152">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="712e5-152">Team Chat Messages</span></span>
- <span data-ttu-id="712e5-153">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="712e5-153">Private Chat Messages</span></span>
- <span data-ttu-id="712e5-154">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="712e5-154">Calls</span></span>
- <span data-ttu-id="712e5-155">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="712e5-155">Meetings</span></span>
- <span data-ttu-id="712e5-156">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="712e5-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="712e5-157">JSON</span><span class="sxs-lookup"><span data-stu-id="712e5-157">JSON</span></span>

<span data-ttu-id="712e5-158">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="712e5-158">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="712e5-159">Пример</span><span class="sxs-lookup"><span data-stu-id="712e5-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="712e5-160">CSV</span><span class="sxs-lookup"><span data-stu-id="712e5-160">CSV</span></span>

<span data-ttu-id="712e5-161">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="712e5-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="712e5-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="712e5-162">Request</span></span>

<span data-ttu-id="712e5-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="712e5-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="712e5-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="712e5-164">Response</span></span>

<span data-ttu-id="712e5-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="712e5-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="712e5-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="712e5-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="712e5-167">JSON</span><span class="sxs-lookup"><span data-stu-id="712e5-167">JSON</span></span>

<span data-ttu-id="712e5-168">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="712e5-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="712e5-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="712e5-169">Request</span></span>

<span data-ttu-id="712e5-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="712e5-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="712e5-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="712e5-171">Response</span></span>

<span data-ttu-id="712e5-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="712e5-172">The following is an example of the response.</span></span>

> <span data-ttu-id="712e5-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="712e5-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
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


