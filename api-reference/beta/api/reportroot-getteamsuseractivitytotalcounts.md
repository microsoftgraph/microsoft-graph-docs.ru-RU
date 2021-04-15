---
title: 'reportRoot: getTeamsUserActivityTotalCounts'
description: Получение количества действий Microsoft Teams по типам. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. Действия выполняются лицензированными или не лицензированными пользователями Microsoft Teams.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0c5acd7387638aba2fa3a992441982f5918be37f
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766955"
---
# <a name="reportroot-getteamsuseractivitytotalcounts"></a><span data-ttu-id="65f98-105">reportRoot: getTeamsUserActivityTotalCounts</span><span class="sxs-lookup"><span data-stu-id="65f98-105">reportRoot: getTeamsUserActivityTotalCounts</span></span>

<span data-ttu-id="65f98-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f98-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65f98-107">Получение количества действий Microsoft Teams по типам.</span><span class="sxs-lookup"><span data-stu-id="65f98-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="65f98-108">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="65f98-108">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span> <span data-ttu-id="65f98-109">Действия выполняются лицензированными или не лицензированными пользователями Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="65f98-109">The activities are performed by Microsoft Teams licensed or non-licensed users.</span></span>

## <a name="permissions"></a><span data-ttu-id="65f98-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65f98-110">Permissions</span></span>

<span data-ttu-id="65f98-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65f98-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65f98-113">Permission type</span></span>                        | <span data-ttu-id="65f98-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65f98-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65f98-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65f98-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="65f98-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65f98-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65f98-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65f98-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65f98-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f98-118">Not supported.</span></span>                           |
| <span data-ttu-id="65f98-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65f98-119">Application</span></span>                            | <span data-ttu-id="65f98-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65f98-120">Reports.Read.All</span></span>                         |

><span data-ttu-id="65f98-121">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="65f98-121">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="65f98-122">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="65f98-122">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="65f98-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65f98-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="65f98-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="65f98-124">Function parameters</span></span>

<span data-ttu-id="65f98-125">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="65f98-125">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65f98-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="65f98-126">Parameter</span></span> | <span data-ttu-id="65f98-127">Тип</span><span class="sxs-lookup"><span data-stu-id="65f98-127">Type</span></span>   | <span data-ttu-id="65f98-128">Описание</span><span class="sxs-lookup"><span data-stu-id="65f98-128">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65f98-129">period</span><span class="sxs-lookup"><span data-stu-id="65f98-129">period</span></span>    | <span data-ttu-id="65f98-130">string</span><span class="sxs-lookup"><span data-stu-id="65f98-130">string</span></span> | <span data-ttu-id="65f98-131">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="65f98-131">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65f98-132">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="65f98-132">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65f98-133">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="65f98-133">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65f98-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f98-134">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="65f98-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65f98-135">Optional query parameters</span></span>

<span data-ttu-id="65f98-136">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="65f98-136">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="65f98-137">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="65f98-137">The default output type is text/csv.</span></span> <span data-ttu-id="65f98-138">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, заданный для `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="65f98-138">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65f98-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65f98-139">Request headers</span></span>

| <span data-ttu-id="65f98-140">Имя</span><span class="sxs-lookup"><span data-stu-id="65f98-140">Name</span></span>          | <span data-ttu-id="65f98-141">Описание</span><span class="sxs-lookup"><span data-stu-id="65f98-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="65f98-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65f98-142">Authorization</span></span> | <span data-ttu-id="65f98-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f98-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="65f98-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f98-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="65f98-146">CSV</span><span class="sxs-lookup"><span data-stu-id="65f98-146">CSV</span></span>

<span data-ttu-id="65f98-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="65f98-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65f98-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="65f98-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65f98-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="65f98-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65f98-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="65f98-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65f98-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="65f98-151">Report Refresh Date</span></span>
- <span data-ttu-id="65f98-152">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="65f98-152">Report Date</span></span>
- <span data-ttu-id="65f98-153">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="65f98-153">Team Chat Messages</span></span>
- <span data-ttu-id="65f98-154">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="65f98-154">Private Chat Messages</span></span>
- <span data-ttu-id="65f98-155">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="65f98-155">Calls</span></span>
- <span data-ttu-id="65f98-156">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="65f98-156">Meetings</span></span>
- <span data-ttu-id="65f98-157">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="65f98-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="65f98-158">JSON</span><span class="sxs-lookup"><span data-stu-id="65f98-158">JSON</span></span>

<span data-ttu-id="65f98-159">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="65f98-159">If successful, this method returns a `200 OK` response code and a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f98-160">Пример</span><span class="sxs-lookup"><span data-stu-id="65f98-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="65f98-161">CSV</span><span class="sxs-lookup"><span data-stu-id="65f98-161">CSV</span></span>

<span data-ttu-id="65f98-162">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="65f98-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="65f98-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f98-163">Request</span></span>

<span data-ttu-id="65f98-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65f98-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="65f98-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f98-165">Response</span></span>

<span data-ttu-id="65f98-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65f98-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="65f98-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="65f98-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="65f98-168">JSON</span><span class="sxs-lookup"><span data-stu-id="65f98-168">JSON</span></span>

<span data-ttu-id="65f98-169">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="65f98-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="65f98-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f98-170">Request</span></span>

<span data-ttu-id="65f98-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65f98-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="65f98-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f98-172">Response</span></span>

<span data-ttu-id="65f98-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65f98-173">The following is an example of the response.</span></span>

> <span data-ttu-id="65f98-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65f98-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
