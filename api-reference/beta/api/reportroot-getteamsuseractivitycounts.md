---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Получение количества действий в Microsoft Teams по каждому типу. К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.
ms.openlocfilehash: 2ad0382dec905aab3490a66047916e5028d7b75f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080358"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="14d9d-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="14d9d-104">reportRoot: getTeamsUserActivityCounts</span></span>

> <span data-ttu-id="14d9d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14d9d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14d9d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14d9d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14d9d-107">Получение количества действий в Microsoft Teams по каждому типу.</span><span class="sxs-lookup"><span data-stu-id="14d9d-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="14d9d-108">К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="14d9d-108">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="14d9d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14d9d-109">Permissions</span></span>

<span data-ttu-id="14d9d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14d9d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14d9d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14d9d-112">Permission type</span></span>                        | <span data-ttu-id="14d9d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14d9d-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="14d9d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14d9d-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="14d9d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="14d9d-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="14d9d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14d9d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14d9d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14d9d-117">Not supported.</span></span>                           |
| <span data-ttu-id="14d9d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14d9d-118">Application</span></span>                            | <span data-ttu-id="14d9d-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="14d9d-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="14d9d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14d9d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="14d9d-121">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="14d9d-121">Function parameters</span></span>

<span data-ttu-id="14d9d-122">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="14d9d-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="14d9d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="14d9d-123">Parameter</span></span> | <span data-ttu-id="14d9d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="14d9d-124">Type</span></span>   | <span data-ttu-id="14d9d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="14d9d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="14d9d-126">period</span><span class="sxs-lookup"><span data-stu-id="14d9d-126">period</span></span>    | <span data-ttu-id="14d9d-127">строка</span><span class="sxs-lookup"><span data-stu-id="14d9d-127">string</span></span> | <span data-ttu-id="14d9d-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="14d9d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="14d9d-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="14d9d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="14d9d-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="14d9d-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="14d9d-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14d9d-131">Required.</span></span> |

<span data-ttu-id="14d9d-132">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="14d9d-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="14d9d-133">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="14d9d-133">The default output type is text/csv.</span></span> <span data-ttu-id="14d9d-134">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="14d9d-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14d9d-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14d9d-135">Request headers</span></span>

| <span data-ttu-id="14d9d-136">Имя</span><span class="sxs-lookup"><span data-stu-id="14d9d-136">Name</span></span>          | <span data-ttu-id="14d9d-137">Описание</span><span class="sxs-lookup"><span data-stu-id="14d9d-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="14d9d-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14d9d-138">Authorization</span></span> | <span data-ttu-id="14d9d-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14d9d-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="14d9d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="14d9d-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="14d9d-142">CSV</span><span class="sxs-lookup"><span data-stu-id="14d9d-142">CSV</span></span>

<span data-ttu-id="14d9d-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="14d9d-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="14d9d-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="14d9d-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="14d9d-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="14d9d-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="14d9d-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="14d9d-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="14d9d-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="14d9d-147">Report Refresh Date</span></span>
- <span data-ttu-id="14d9d-148">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="14d9d-148">Report Date</span></span>
- <span data-ttu-id="14d9d-149">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="14d9d-149">Team Chat Messages</span></span>
- <span data-ttu-id="14d9d-150">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="14d9d-150">Private Chat Messages</span></span>
- <span data-ttu-id="14d9d-151">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="14d9d-151">Calls</span></span>
- <span data-ttu-id="14d9d-152">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="14d9d-152">Meetings</span></span>
- <span data-ttu-id="14d9d-153">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="14d9d-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="14d9d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="14d9d-154">JSON</span></span>

<span data-ttu-id="14d9d-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14d9d-155">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d9d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="14d9d-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="14d9d-157">CSV</span><span class="sxs-lookup"><span data-stu-id="14d9d-157">CSV</span></span>

<span data-ttu-id="14d9d-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="14d9d-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="14d9d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="14d9d-159">Request</span></span>

<span data-ttu-id="14d9d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14d9d-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="14d9d-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="14d9d-161">Response</span></span>

<span data-ttu-id="14d9d-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14d9d-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="14d9d-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="14d9d-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="14d9d-164">JSON</span><span class="sxs-lookup"><span data-stu-id="14d9d-164">JSON</span></span>

<span data-ttu-id="14d9d-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="14d9d-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="14d9d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="14d9d-166">Request</span></span>

<span data-ttu-id="14d9d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14d9d-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="14d9d-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="14d9d-168">Response</span></span>

<span data-ttu-id="14d9d-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14d9d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="14d9d-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14d9d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
