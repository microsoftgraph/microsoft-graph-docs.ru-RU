---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Получение количества пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.
localization_priority: Normal
ms.openlocfilehash: 6df1ba5bd813839c965dbd8c2f6c77cd195a3e82
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872697"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="c7391-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c7391-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

> <span data-ttu-id="c7391-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7391-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7391-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7391-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7391-107">Получение количества пользователей Microsoft Teams по типу действия.</span><span class="sxs-lookup"><span data-stu-id="c7391-107">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="c7391-108">К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="c7391-108">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7391-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7391-109">Permissions</span></span>

<span data-ttu-id="c7391-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7391-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7391-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7391-112">Permission type</span></span>                        | <span data-ttu-id="c7391-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7391-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c7391-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7391-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7391-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7391-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c7391-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7391-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7391-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7391-117">Not supported.</span></span>                           |
| <span data-ttu-id="c7391-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7391-118">Application</span></span>                            | <span data-ttu-id="c7391-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7391-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c7391-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7391-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="c7391-121">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="c7391-121">Function parameters</span></span>

<span data-ttu-id="c7391-122">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c7391-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c7391-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="c7391-123">Parameter</span></span> | <span data-ttu-id="c7391-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c7391-124">Type</span></span>   | <span data-ttu-id="c7391-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c7391-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c7391-126">period</span><span class="sxs-lookup"><span data-stu-id="c7391-126">period</span></span>    | <span data-ttu-id="c7391-127">строка</span><span class="sxs-lookup"><span data-stu-id="c7391-127">string</span></span> | <span data-ttu-id="c7391-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c7391-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c7391-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c7391-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c7391-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c7391-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c7391-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7391-131">Required.</span></span> |

<span data-ttu-id="c7391-132">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7391-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c7391-133">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="c7391-133">The default output type is text/csv.</span></span> <span data-ttu-id="c7391-134">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="c7391-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7391-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7391-135">Request headers</span></span>

| <span data-ttu-id="c7391-136">Имя</span><span class="sxs-lookup"><span data-stu-id="c7391-136">Name</span></span>          | <span data-ttu-id="c7391-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c7391-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c7391-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7391-138">Authorization</span></span> | <span data-ttu-id="c7391-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7391-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c7391-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7391-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c7391-142">CSV</span><span class="sxs-lookup"><span data-stu-id="c7391-142">CSV</span></span>

<span data-ttu-id="c7391-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c7391-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c7391-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c7391-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c7391-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c7391-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c7391-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c7391-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c7391-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c7391-147">Report Refresh Date</span></span>
- <span data-ttu-id="c7391-148">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c7391-148">Report Date</span></span>
- <span data-ttu-id="c7391-149">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="c7391-149">Team Chat Messages</span></span>
- <span data-ttu-id="c7391-150">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="c7391-150">Private Chat Messages</span></span>
- <span data-ttu-id="c7391-151">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="c7391-151">Calls</span></span>
- <span data-ttu-id="c7391-152">Meetings (Собрания);</span><span class="sxs-lookup"><span data-stu-id="c7391-152">Meetings</span></span>
- <span data-ttu-id="c7391-153">Other Actions (Другие действия);</span><span class="sxs-lookup"><span data-stu-id="c7391-153">Other Actions</span></span>
- <span data-ttu-id="c7391-154">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c7391-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c7391-155">JSON</span><span class="sxs-lookup"><span data-stu-id="c7391-155">JSON</span></span>

<span data-ttu-id="c7391-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7391-156">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7391-157">Пример</span><span class="sxs-lookup"><span data-stu-id="c7391-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c7391-158">CSV</span><span class="sxs-lookup"><span data-stu-id="c7391-158">CSV</span></span>

<span data-ttu-id="c7391-159">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="c7391-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c7391-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7391-160">Request</span></span>

<span data-ttu-id="c7391-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7391-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c7391-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7391-162">Response</span></span>

<span data-ttu-id="c7391-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c7391-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c7391-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c7391-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c7391-165">JSON</span><span class="sxs-lookup"><span data-stu-id="c7391-165">JSON</span></span>

<span data-ttu-id="c7391-166">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="c7391-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c7391-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7391-167">Request</span></span>

<span data-ttu-id="c7391-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7391-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c7391-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7391-169">Response</span></span>

<span data-ttu-id="c7391-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7391-170">The following is an example of the response.</span></span>

> <span data-ttu-id="c7391-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7391-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
