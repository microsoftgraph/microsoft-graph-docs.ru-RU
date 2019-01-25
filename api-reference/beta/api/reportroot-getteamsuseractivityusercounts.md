---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 08b7a148f9ff19c738a3a2b5a5b8e066c8abe155
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530001"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="df701-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="df701-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df701-105">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="df701-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="df701-106">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="df701-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="df701-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df701-107">Permissions</span></span>

<span data-ttu-id="df701-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df701-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df701-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df701-110">Permission type</span></span>                        | <span data-ttu-id="df701-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df701-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="df701-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df701-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="df701-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df701-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="df701-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df701-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df701-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df701-115">Not supported.</span></span>                           |
| <span data-ttu-id="df701-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df701-116">Application</span></span>                            | <span data-ttu-id="df701-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df701-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="df701-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df701-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="df701-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="df701-119">Function parameters</span></span>

<span data-ttu-id="df701-120">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="df701-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="df701-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="df701-121">Parameter</span></span> | <span data-ttu-id="df701-122">Тип</span><span class="sxs-lookup"><span data-stu-id="df701-122">Type</span></span>   | <span data-ttu-id="df701-123">Описание</span><span class="sxs-lookup"><span data-stu-id="df701-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="df701-124">period</span><span class="sxs-lookup"><span data-stu-id="df701-124">period</span></span>    | <span data-ttu-id="df701-125">строка</span><span class="sxs-lookup"><span data-stu-id="df701-125">string</span></span> | <span data-ttu-id="df701-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="df701-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="df701-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="df701-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="df701-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="df701-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="df701-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df701-129">Required.</span></span> |

<span data-ttu-id="df701-130">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="df701-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="df701-131">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="df701-131">The default output type is text/csv.</span></span> <span data-ttu-id="df701-132">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="df701-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df701-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df701-133">Request headers</span></span>

| <span data-ttu-id="df701-134">Имя</span><span class="sxs-lookup"><span data-stu-id="df701-134">Name</span></span>          | <span data-ttu-id="df701-135">Описание</span><span class="sxs-lookup"><span data-stu-id="df701-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="df701-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df701-136">Authorization</span></span> | <span data-ttu-id="df701-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df701-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="df701-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="df701-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="df701-140">CSV</span><span class="sxs-lookup"><span data-stu-id="df701-140">CSV</span></span>

<span data-ttu-id="df701-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="df701-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="df701-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="df701-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="df701-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="df701-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="df701-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="df701-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="df701-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="df701-145">Report Refresh Date</span></span>
- <span data-ttu-id="df701-146">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="df701-146">Report Date</span></span>
- <span data-ttu-id="df701-147">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="df701-147">Team Chat Messages</span></span>
- <span data-ttu-id="df701-148">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="df701-148">Private Chat Messages</span></span>
- <span data-ttu-id="df701-149">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="df701-149">Calls</span></span>
- <span data-ttu-id="df701-150">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="df701-150">Meetings</span></span>
- <span data-ttu-id="df701-151">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="df701-151">Other Actions</span></span>
- <span data-ttu-id="df701-152">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="df701-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="df701-153">JSON</span><span class="sxs-lookup"><span data-stu-id="df701-153">JSON</span></span>

<span data-ttu-id="df701-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="df701-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df701-155">Пример</span><span class="sxs-lookup"><span data-stu-id="df701-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="df701-156">CSV</span><span class="sxs-lookup"><span data-stu-id="df701-156">CSV</span></span>

<span data-ttu-id="df701-157">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="df701-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="df701-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="df701-158">Request</span></span>

<span data-ttu-id="df701-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df701-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="df701-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="df701-160">Response</span></span>

<span data-ttu-id="df701-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="df701-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="df701-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="df701-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="df701-163">JSON</span><span class="sxs-lookup"><span data-stu-id="df701-163">JSON</span></span>

<span data-ttu-id="df701-164">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="df701-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="df701-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="df701-165">Request</span></span>

<span data-ttu-id="df701-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df701-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="df701-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="df701-167">Response</span></span>

<span data-ttu-id="df701-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df701-168">The following is an example of the response.</span></span>

> <span data-ttu-id="df701-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df701-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
