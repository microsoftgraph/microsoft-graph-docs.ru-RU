---
title: 'reportRoot: getTeamsUserActivityDistributionUserCounts'
description: Получите количество лицензированных Microsoft Teams по типу действия за выбранный период. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 69bdcafd963c96274034f53158337d0e38c3d654
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053519"
---
# <a name="reportroot-getteamsuseractivitydistributionusercounts"></a><span data-ttu-id="7db68-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7db68-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span></span>

<span data-ttu-id="7db68-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7db68-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7db68-106">Получите количество лицензированных Microsoft Teams по типу действия за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="7db68-106">Get the number of Microsoft Teams licensed users by activity type over the selected period.</span></span> <span data-ttu-id="7db68-107">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="7db68-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="7db68-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7db68-108">Permissions</span></span>

<span data-ttu-id="7db68-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7db68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7db68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7db68-111">Permission type</span></span>                        | <span data-ttu-id="7db68-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7db68-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7db68-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7db68-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7db68-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7db68-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7db68-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7db68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7db68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7db68-116">Not supported.</span></span>                           |
| <span data-ttu-id="7db68-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7db68-117">Application</span></span>                            | <span data-ttu-id="7db68-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7db68-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="7db68-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7db68-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7db68-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7db68-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7db68-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7db68-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="7db68-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="7db68-122">Function parameters</span></span>

<span data-ttu-id="7db68-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7db68-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7db68-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="7db68-124">Parameter</span></span> | <span data-ttu-id="7db68-125">Тип</span><span class="sxs-lookup"><span data-stu-id="7db68-125">Type</span></span>   | <span data-ttu-id="7db68-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7db68-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7db68-127">period</span><span class="sxs-lookup"><span data-stu-id="7db68-127">period</span></span>    | <span data-ttu-id="7db68-128">string</span><span class="sxs-lookup"><span data-stu-id="7db68-128">string</span></span> | <span data-ttu-id="7db68-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7db68-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7db68-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7db68-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7db68-131">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7db68-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7db68-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7db68-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="7db68-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7db68-133">Optional query parameters</span></span>

<span data-ttu-id="7db68-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7db68-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7db68-135">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="7db68-135">The default output type is text/csv.</span></span> <span data-ttu-id="7db68-136">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, заданный для `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="7db68-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7db68-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7db68-137">Request headers</span></span>

| <span data-ttu-id="7db68-138">Имя</span><span class="sxs-lookup"><span data-stu-id="7db68-138">Name</span></span>          | <span data-ttu-id="7db68-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7db68-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7db68-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7db68-140">Authorization</span></span> | <span data-ttu-id="7db68-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7db68-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7db68-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7db68-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7db68-144">CSV</span><span class="sxs-lookup"><span data-stu-id="7db68-144">CSV</span></span>

<span data-ttu-id="7db68-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7db68-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7db68-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7db68-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7db68-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7db68-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7db68-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7db68-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7db68-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7db68-149">Report Refresh Date</span></span>
- <span data-ttu-id="7db68-150">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="7db68-150">Team Chat Messages</span></span>
- <span data-ttu-id="7db68-151">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="7db68-151">Private Chat Messages</span></span>
- <span data-ttu-id="7db68-152">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="7db68-152">Calls</span></span>
- <span data-ttu-id="7db68-153">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="7db68-153">Meetings</span></span>
- <span data-ttu-id="7db68-154">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="7db68-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7db68-155">JSON</span><span class="sxs-lookup"><span data-stu-id="7db68-155">JSON</span></span>

<span data-ttu-id="7db68-156">В случае успеха этот метод возвращает код ответа и объект `200 OK` [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7db68-156">If successful, this method returns a `200 OK` response code and a [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7db68-157">Пример</span><span class="sxs-lookup"><span data-stu-id="7db68-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7db68-158">CSV</span><span class="sxs-lookup"><span data-stu-id="7db68-158">CSV</span></span>

<span data-ttu-id="7db68-159">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="7db68-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7db68-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="7db68-160">Request</span></span>

<span data-ttu-id="7db68-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7db68-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7db68-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7db68-162">Response</span></span>

<span data-ttu-id="7db68-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7db68-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7db68-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7db68-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="7db68-165">JSON</span><span class="sxs-lookup"><span data-stu-id="7db68-165">JSON</span></span>

<span data-ttu-id="7db68-166">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="7db68-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7db68-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="7db68-167">Request</span></span>

<span data-ttu-id="7db68-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7db68-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7db68-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7db68-169">Response</span></span>

<span data-ttu-id="7db68-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7db68-170">The following is an example of the response.</span></span>

> <span data-ttu-id="7db68-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7db68-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsuseractivitydistributionusercounts)", 
  "value": [
    {
      "reportRefreshDate": "2020-09-01", 
      "teamChatMessages": 0, 
      "privateChatMessages": 0, 
      "calls": 0, 
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


