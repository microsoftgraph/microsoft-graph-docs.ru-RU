---
title: 'reportRoot: getTeamsUserActivityDistributionUserCounts'
description: Получите число лицензированных пользователей Microsoft Teams по типу активности за выбранный период. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 91a9f503ad2798f154d7415e93e7c4be28cd7c32
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766967"
---
# <a name="reportroot-getteamsuseractivitydistributionusercounts"></a><span data-ttu-id="80133-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="80133-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span></span>

<span data-ttu-id="80133-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80133-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80133-106">Получите число лицензированных пользователей Microsoft Teams по типу активности за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="80133-106">Get the number of Microsoft Teams licensed users by activity type over the selected period.</span></span> <span data-ttu-id="80133-107">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="80133-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="80133-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80133-108">Permissions</span></span>

<span data-ttu-id="80133-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80133-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80133-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80133-111">Permission type</span></span>                        | <span data-ttu-id="80133-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80133-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="80133-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80133-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="80133-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="80133-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="80133-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80133-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80133-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80133-116">Not supported.</span></span>                           |
| <span data-ttu-id="80133-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80133-117">Application</span></span>                            | <span data-ttu-id="80133-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="80133-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="80133-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="80133-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="80133-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="80133-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="80133-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80133-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="80133-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="80133-122">Function parameters</span></span>

<span data-ttu-id="80133-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="80133-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="80133-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="80133-124">Parameter</span></span> | <span data-ttu-id="80133-125">Тип</span><span class="sxs-lookup"><span data-stu-id="80133-125">Type</span></span>   | <span data-ttu-id="80133-126">Описание</span><span class="sxs-lookup"><span data-stu-id="80133-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="80133-127">period</span><span class="sxs-lookup"><span data-stu-id="80133-127">period</span></span>    | <span data-ttu-id="80133-128">string</span><span class="sxs-lookup"><span data-stu-id="80133-128">string</span></span> | <span data-ttu-id="80133-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="80133-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="80133-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="80133-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="80133-131">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="80133-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="80133-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80133-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="80133-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="80133-133">Optional query parameters</span></span>

<span data-ttu-id="80133-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="80133-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="80133-135">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="80133-135">The default output type is text/csv.</span></span> <span data-ttu-id="80133-136">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, заданный для `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="80133-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80133-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80133-137">Request headers</span></span>

| <span data-ttu-id="80133-138">Имя</span><span class="sxs-lookup"><span data-stu-id="80133-138">Name</span></span>          | <span data-ttu-id="80133-139">Описание</span><span class="sxs-lookup"><span data-stu-id="80133-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="80133-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80133-140">Authorization</span></span> | <span data-ttu-id="80133-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80133-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="80133-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="80133-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="80133-144">CSV</span><span class="sxs-lookup"><span data-stu-id="80133-144">CSV</span></span>

<span data-ttu-id="80133-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="80133-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="80133-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="80133-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="80133-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="80133-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="80133-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="80133-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="80133-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="80133-149">Report Refresh Date</span></span>
- <span data-ttu-id="80133-150">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="80133-150">Team Chat Messages</span></span>
- <span data-ttu-id="80133-151">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="80133-151">Private Chat Messages</span></span>
- <span data-ttu-id="80133-152">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="80133-152">Calls</span></span>
- <span data-ttu-id="80133-153">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="80133-153">Meetings</span></span>
- <span data-ttu-id="80133-154">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="80133-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="80133-155">JSON</span><span class="sxs-lookup"><span data-stu-id="80133-155">JSON</span></span>

<span data-ttu-id="80133-156">В случае успеха этот метод возвращает код ответа и объект `200 OK` [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="80133-156">If successful, this method returns a `200 OK` response code and a [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80133-157">Пример</span><span class="sxs-lookup"><span data-stu-id="80133-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="80133-158">CSV</span><span class="sxs-lookup"><span data-stu-id="80133-158">CSV</span></span>

<span data-ttu-id="80133-159">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="80133-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="80133-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="80133-160">Request</span></span>

<span data-ttu-id="80133-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80133-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="80133-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="80133-162">Response</span></span>

<span data-ttu-id="80133-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80133-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="80133-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="80133-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="80133-165">JSON</span><span class="sxs-lookup"><span data-stu-id="80133-165">JSON</span></span>

<span data-ttu-id="80133-166">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="80133-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="80133-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="80133-167">Request</span></span>

<span data-ttu-id="80133-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80133-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="80133-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="80133-169">Response</span></span>

<span data-ttu-id="80133-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80133-170">The following is an example of the response.</span></span>

> <span data-ttu-id="80133-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80133-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


