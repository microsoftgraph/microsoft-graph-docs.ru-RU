---
title: 'reportRoot: getTeamsUserActivityTotalCounts'
description: Получение количества действий Microsoft Teams по типам. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. Эти действия выполняются Microsoft Teams или не лицензированными пользователями.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c41cbd1b71081ef90830b6552f99ad246e253945
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055017"
---
# <a name="reportroot-getteamsuseractivitytotalcounts"></a><span data-ttu-id="e8317-105">reportRoot: getTeamsUserActivityTotalCounts</span><span class="sxs-lookup"><span data-stu-id="e8317-105">reportRoot: getTeamsUserActivityTotalCounts</span></span>

<span data-ttu-id="e8317-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8317-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8317-107">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="e8317-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="e8317-108">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="e8317-108">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span> <span data-ttu-id="e8317-109">Эти действия выполняются Microsoft Teams или не лицензированными пользователями.</span><span class="sxs-lookup"><span data-stu-id="e8317-109">The activities are performed by Microsoft Teams licensed or non-licensed users.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8317-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8317-110">Permissions</span></span>

<span data-ttu-id="e8317-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8317-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8317-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8317-113">Permission type</span></span>                        | <span data-ttu-id="e8317-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8317-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e8317-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8317-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8317-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8317-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e8317-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8317-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8317-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8317-118">Not supported.</span></span>                           |
| <span data-ttu-id="e8317-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8317-119">Application</span></span>                            | <span data-ttu-id="e8317-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8317-120">Reports.Read.All</span></span>                         |

><span data-ttu-id="e8317-121">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e8317-121">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e8317-122">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e8317-122">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e8317-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8317-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="e8317-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e8317-124">Function parameters</span></span>

<span data-ttu-id="e8317-125">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e8317-125">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e8317-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="e8317-126">Parameter</span></span> | <span data-ttu-id="e8317-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e8317-127">Type</span></span>   | <span data-ttu-id="e8317-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e8317-128">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e8317-129">period</span><span class="sxs-lookup"><span data-stu-id="e8317-129">period</span></span>    | <span data-ttu-id="e8317-130">string</span><span class="sxs-lookup"><span data-stu-id="e8317-130">string</span></span> | <span data-ttu-id="e8317-131">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e8317-131">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e8317-132">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e8317-132">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e8317-133">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e8317-133">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e8317-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8317-134">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e8317-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8317-135">Optional query parameters</span></span>

<span data-ttu-id="e8317-136">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e8317-136">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e8317-137">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="e8317-137">The default output type is text/csv.</span></span> <span data-ttu-id="e8317-138">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, заданный для `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="e8317-138">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8317-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8317-139">Request headers</span></span>

| <span data-ttu-id="e8317-140">Имя</span><span class="sxs-lookup"><span data-stu-id="e8317-140">Name</span></span>          | <span data-ttu-id="e8317-141">Описание</span><span class="sxs-lookup"><span data-stu-id="e8317-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e8317-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8317-142">Authorization</span></span> | <span data-ttu-id="e8317-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8317-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e8317-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8317-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e8317-146">CSV</span><span class="sxs-lookup"><span data-stu-id="e8317-146">CSV</span></span>

<span data-ttu-id="e8317-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e8317-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e8317-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e8317-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e8317-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e8317-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e8317-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e8317-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e8317-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e8317-151">Report Refresh Date</span></span>
- <span data-ttu-id="e8317-152">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e8317-152">Report Date</span></span>
- <span data-ttu-id="e8317-153">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="e8317-153">Team Chat Messages</span></span>
- <span data-ttu-id="e8317-154">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="e8317-154">Private Chat Messages</span></span>
- <span data-ttu-id="e8317-155">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="e8317-155">Calls</span></span>
- <span data-ttu-id="e8317-156">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="e8317-156">Meetings</span></span>
- <span data-ttu-id="e8317-157">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="e8317-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e8317-158">JSON</span><span class="sxs-lookup"><span data-stu-id="e8317-158">JSON</span></span>

<span data-ttu-id="e8317-159">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e8317-159">If successful, this method returns a `200 OK` response code and a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8317-160">Пример</span><span class="sxs-lookup"><span data-stu-id="e8317-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e8317-161">CSV</span><span class="sxs-lookup"><span data-stu-id="e8317-161">CSV</span></span>

<span data-ttu-id="e8317-162">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="e8317-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e8317-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8317-163">Request</span></span>

<span data-ttu-id="e8317-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8317-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="e8317-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8317-165">Response</span></span>

<span data-ttu-id="e8317-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8317-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="e8317-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e8317-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e8317-168">JSON</span><span class="sxs-lookup"><span data-stu-id="e8317-168">JSON</span></span>

<span data-ttu-id="e8317-169">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="e8317-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e8317-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8317-170">Request</span></span>

<span data-ttu-id="e8317-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8317-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="e8317-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8317-172">Response</span></span>

<span data-ttu-id="e8317-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8317-173">The following is an example of the response.</span></span>

> <span data-ttu-id="e8317-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8317-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
