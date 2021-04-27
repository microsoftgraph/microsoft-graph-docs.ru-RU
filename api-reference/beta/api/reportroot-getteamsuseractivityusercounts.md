---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получите количество лицензированных Microsoft Teams по типу действия. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: c43667c435d7183c0298d99a743c5c81abd4751d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055010"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="2d831-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2d831-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="2d831-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d831-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d831-106">Получите количество лицензированных Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="2d831-106">Get the number of Microsoft Teams licensed users by activity type.</span></span> <span data-ttu-id="2d831-107">Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний.</span><span class="sxs-lookup"><span data-stu-id="2d831-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d831-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d831-108">Permissions</span></span>

<span data-ttu-id="2d831-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d831-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d831-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d831-111">Permission type</span></span>                        | <span data-ttu-id="2d831-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d831-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2d831-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d831-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d831-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d831-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2d831-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d831-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d831-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d831-116">Not supported.</span></span>                           |
| <span data-ttu-id="2d831-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d831-117">Application</span></span>                            | <span data-ttu-id="2d831-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d831-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="2d831-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2d831-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2d831-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2d831-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2d831-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d831-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="2d831-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2d831-122">Function parameters</span></span>

<span data-ttu-id="2d831-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2d831-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2d831-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d831-124">Parameter</span></span> | <span data-ttu-id="2d831-125">Тип</span><span class="sxs-lookup"><span data-stu-id="2d831-125">Type</span></span>   | <span data-ttu-id="2d831-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2d831-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2d831-127">period</span><span class="sxs-lookup"><span data-stu-id="2d831-127">period</span></span>    | <span data-ttu-id="2d831-128">string</span><span class="sxs-lookup"><span data-stu-id="2d831-128">string</span></span> | <span data-ttu-id="2d831-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2d831-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2d831-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2d831-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2d831-131">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2d831-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2d831-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d831-132">Required.</span></span> |

<span data-ttu-id="2d831-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2d831-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2d831-134">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="2d831-134">The default output type is text/csv.</span></span> <span data-ttu-id="2d831-135">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="2d831-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d831-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d831-136">Request headers</span></span>

| <span data-ttu-id="2d831-137">Имя</span><span class="sxs-lookup"><span data-stu-id="2d831-137">Name</span></span>          | <span data-ttu-id="2d831-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2d831-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2d831-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d831-139">Authorization</span></span> | <span data-ttu-id="2d831-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d831-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2d831-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d831-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2d831-143">CSV</span><span class="sxs-lookup"><span data-stu-id="2d831-143">CSV</span></span>

<span data-ttu-id="2d831-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2d831-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2d831-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2d831-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2d831-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2d831-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2d831-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2d831-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2d831-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2d831-148">Report Refresh Date</span></span>
- <span data-ttu-id="2d831-149">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="2d831-149">Report Date</span></span>
- <span data-ttu-id="2d831-150">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="2d831-150">Team Chat Messages</span></span>
- <span data-ttu-id="2d831-151">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="2d831-151">Private Chat Messages</span></span>
- <span data-ttu-id="2d831-152">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="2d831-152">Calls</span></span>
- <span data-ttu-id="2d831-153">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="2d831-153">Meetings</span></span>
- <span data-ttu-id="2d831-154">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="2d831-154">Other Actions</span></span>
- <span data-ttu-id="2d831-155">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="2d831-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2d831-156">JSON</span><span class="sxs-lookup"><span data-stu-id="2d831-156">JSON</span></span>

<span data-ttu-id="2d831-157">В случае успешной работы этот метод возвращает код ответа и `200 OK` **[объект teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2d831-157">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d831-158">Пример</span><span class="sxs-lookup"><span data-stu-id="2d831-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2d831-159">CSV</span><span class="sxs-lookup"><span data-stu-id="2d831-159">CSV</span></span>

<span data-ttu-id="2d831-160">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="2d831-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2d831-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d831-161">Request</span></span>

<span data-ttu-id="2d831-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d831-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="2d831-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d831-163">Response</span></span>

<span data-ttu-id="2d831-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d831-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2d831-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2d831-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="2d831-166">JSON</span><span class="sxs-lookup"><span data-stu-id="2d831-166">JSON</span></span>

<span data-ttu-id="2d831-167">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="2d831-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2d831-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d831-168">Request</span></span>

<span data-ttu-id="2d831-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d831-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="2d831-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d831-170">Response</span></span>

<span data-ttu-id="2d831-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2d831-171">The following is an example of the response.</span></span>

> <span data-ttu-id="2d831-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2d831-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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


