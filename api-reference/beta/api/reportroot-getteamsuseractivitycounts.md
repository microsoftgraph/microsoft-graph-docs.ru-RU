---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Получение количества действий в Microsoft Teams по каждому типу. К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: fee00c7100f5fd041334ccac11530d2d52c967c6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982917"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="28617-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="28617-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="28617-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28617-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28617-106">Получение количества действий в Microsoft Teams по каждому типу.</span><span class="sxs-lookup"><span data-stu-id="28617-106">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="28617-107">К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="28617-107">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="28617-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28617-108">Permissions</span></span>

<span data-ttu-id="28617-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28617-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28617-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28617-111">Permission type</span></span>                        | <span data-ttu-id="28617-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28617-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="28617-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28617-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="28617-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28617-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="28617-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28617-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28617-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28617-116">Not supported.</span></span>                           |
| <span data-ttu-id="28617-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28617-117">Application</span></span>                            | <span data-ttu-id="28617-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28617-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="28617-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28617-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="28617-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="28617-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="28617-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28617-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="28617-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="28617-122">Function parameters</span></span>

<span data-ttu-id="28617-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="28617-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="28617-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="28617-124">Parameter</span></span> | <span data-ttu-id="28617-125">Тип</span><span class="sxs-lookup"><span data-stu-id="28617-125">Type</span></span>   | <span data-ttu-id="28617-126">Описание</span><span class="sxs-lookup"><span data-stu-id="28617-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="28617-127">period</span><span class="sxs-lookup"><span data-stu-id="28617-127">period</span></span>    | <span data-ttu-id="28617-128">string</span><span class="sxs-lookup"><span data-stu-id="28617-128">string</span></span> | <span data-ttu-id="28617-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="28617-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="28617-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="28617-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="28617-131">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="28617-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="28617-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28617-132">Required.</span></span> |

<span data-ttu-id="28617-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="28617-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="28617-134">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="28617-134">The default output type is text/csv.</span></span> <span data-ttu-id="28617-135">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="28617-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28617-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28617-136">Request headers</span></span>

| <span data-ttu-id="28617-137">Имя</span><span class="sxs-lookup"><span data-stu-id="28617-137">Name</span></span>          | <span data-ttu-id="28617-138">Описание</span><span class="sxs-lookup"><span data-stu-id="28617-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="28617-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28617-139">Authorization</span></span> | <span data-ttu-id="28617-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28617-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="28617-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="28617-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="28617-143">CSV</span><span class="sxs-lookup"><span data-stu-id="28617-143">CSV</span></span>

<span data-ttu-id="28617-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="28617-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="28617-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="28617-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="28617-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="28617-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="28617-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="28617-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="28617-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="28617-148">Report Refresh Date</span></span>
- <span data-ttu-id="28617-149">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="28617-149">Report Date</span></span>
- <span data-ttu-id="28617-150">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="28617-150">Team Chat Messages</span></span>
- <span data-ttu-id="28617-151">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="28617-151">Private Chat Messages</span></span>
- <span data-ttu-id="28617-152">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="28617-152">Calls</span></span>
- <span data-ttu-id="28617-153">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="28617-153">Meetings</span></span>
- <span data-ttu-id="28617-154">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="28617-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="28617-155">JSON</span><span class="sxs-lookup"><span data-stu-id="28617-155">JSON</span></span>

<span data-ttu-id="28617-156">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28617-156">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28617-157">Пример</span><span class="sxs-lookup"><span data-stu-id="28617-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="28617-158">CSV</span><span class="sxs-lookup"><span data-stu-id="28617-158">CSV</span></span>

<span data-ttu-id="28617-159">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="28617-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="28617-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="28617-160">Request</span></span>

<span data-ttu-id="28617-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28617-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="28617-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="28617-162">Response</span></span>

<span data-ttu-id="28617-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28617-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="28617-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="28617-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="28617-165">JSON</span><span class="sxs-lookup"><span data-stu-id="28617-165">JSON</span></span>

<span data-ttu-id="28617-166">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="28617-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="28617-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="28617-167">Request</span></span>

<span data-ttu-id="28617-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28617-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="28617-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="28617-169">Response</span></span>

<span data-ttu-id="28617-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28617-170">The following is an example of the response.</span></span>

> <span data-ttu-id="28617-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28617-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


