---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b2a266af3f77932f8b043880dbeb22dcb3674153
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590385"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="4d2e2-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="4d2e2-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="4d2e2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d2e2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d2e2-106">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="4d2e2-107">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d2e2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2e2-108">Permissions</span></span>

<span data-ttu-id="4d2e2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d2e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2e2-111">Permission type</span></span>                        | <span data-ttu-id="4d2e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d2e2-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4d2e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d2e2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d2e2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d2e2-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4d2e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d2e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d2e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-116">Not supported.</span></span>                           |
| <span data-ttu-id="4d2e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d2e2-117">Application</span></span>                            | <span data-ttu-id="4d2e2-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d2e2-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="4d2e2-119">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4d2e2-120">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4d2e2-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4d2e2-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="4d2e2-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4d2e2-122">Function parameters</span></span>

<span data-ttu-id="4d2e2-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4d2e2-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="4d2e2-124">Parameter</span></span> | <span data-ttu-id="4d2e2-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4d2e2-125">Type</span></span>   | <span data-ttu-id="4d2e2-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2e2-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4d2e2-127">period</span><span class="sxs-lookup"><span data-stu-id="4d2e2-127">period</span></span>    | <span data-ttu-id="4d2e2-128">string</span><span class="sxs-lookup"><span data-stu-id="4d2e2-128">string</span></span> | <span data-ttu-id="4d2e2-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4d2e2-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4d2e2-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4d2e2-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-132">Required.</span></span> |

<span data-ttu-id="4d2e2-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4d2e2-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-134">The default output type is text/csv.</span></span> <span data-ttu-id="4d2e2-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d2e2-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d2e2-136">Request headers</span></span>

| <span data-ttu-id="4d2e2-137">Имя</span><span class="sxs-lookup"><span data-stu-id="4d2e2-137">Name</span></span>          | <span data-ttu-id="4d2e2-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2e2-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4d2e2-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d2e2-139">Authorization</span></span> | <span data-ttu-id="4d2e2-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4d2e2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e2-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4d2e2-143">CSV</span><span class="sxs-lookup"><span data-stu-id="4d2e2-143">CSV</span></span>

<span data-ttu-id="4d2e2-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4d2e2-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4d2e2-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4d2e2-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4d2e2-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4d2e2-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-148">Report Refresh Date</span></span>
- <span data-ttu-id="4d2e2-149">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-149">Report Date</span></span>
- <span data-ttu-id="4d2e2-150">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-150">Team Chat Messages</span></span>
- <span data-ttu-id="4d2e2-151">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-151">Private Chat Messages</span></span>
- <span data-ttu-id="4d2e2-152">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-152">Calls</span></span>
- <span data-ttu-id="4d2e2-153">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-153">Meetings</span></span>
- <span data-ttu-id="4d2e2-154">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="4d2e2-154">Other Actions</span></span>
- <span data-ttu-id="4d2e2-155">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4d2e2-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4d2e2-156">JSON</span><span class="sxs-lookup"><span data-stu-id="4d2e2-156">JSON</span></span>

<span data-ttu-id="4d2e2-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсусерактивитюсеркаунтс](../resources/teamsuseractivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-157">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d2e2-158">Пример</span><span class="sxs-lookup"><span data-stu-id="4d2e2-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4d2e2-159">CSV</span><span class="sxs-lookup"><span data-stu-id="4d2e2-159">CSV</span></span>

<span data-ttu-id="4d2e2-160">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4d2e2-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e2-161">Request</span></span>

<span data-ttu-id="4d2e2-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="4d2e2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e2-163">Response</span></span>

<span data-ttu-id="4d2e2-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4d2e2-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4d2e2-166">JSON</span><span class="sxs-lookup"><span data-stu-id="4d2e2-166">JSON</span></span>

<span data-ttu-id="4d2e2-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4d2e2-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e2-168">Request</span></span>

<span data-ttu-id="4d2e2-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="4d2e2-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e2-170">Response</span></span>

<span data-ttu-id="4d2e2-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-171">The following is an example of the response.</span></span>

> <span data-ttu-id="4d2e2-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d2e2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
