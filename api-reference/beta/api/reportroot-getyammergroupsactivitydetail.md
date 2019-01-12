---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d589f6b8d9a5e51fe77c7da13ce3c5c0f662acce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942880"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="70f08-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="70f08-103">reportRoot: getYammerGroupsActivityDetail</span></span>

> <span data-ttu-id="70f08-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70f08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70f08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70f08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70f08-106">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="70f08-106">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="70f08-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="70f08-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="70f08-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70f08-108">Permissions</span></span>

<span data-ttu-id="70f08-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70f08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70f08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70f08-111">Permission type</span></span>                        | <span data-ttu-id="70f08-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70f08-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70f08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70f08-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="70f08-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70f08-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="70f08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70f08-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70f08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70f08-116">Not supported.</span></span>                           |
| <span data-ttu-id="70f08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70f08-117">Application</span></span>                            | <span data-ttu-id="70f08-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70f08-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="70f08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70f08-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="70f08-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="70f08-120">Function parameters</span></span>

<span data-ttu-id="70f08-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="70f08-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="70f08-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="70f08-122">Parameter</span></span> | <span data-ttu-id="70f08-123">Тип</span><span class="sxs-lookup"><span data-stu-id="70f08-123">Type</span></span>   | <span data-ttu-id="70f08-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70f08-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70f08-125">period</span><span class="sxs-lookup"><span data-stu-id="70f08-125">period</span></span>    | <span data-ttu-id="70f08-126">строка</span><span class="sxs-lookup"><span data-stu-id="70f08-126">string</span></span> | <span data-ttu-id="70f08-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="70f08-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70f08-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="70f08-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70f08-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="70f08-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="70f08-130">date</span><span class="sxs-lookup"><span data-stu-id="70f08-130">date</span></span>      | <span data-ttu-id="70f08-131">Date</span><span class="sxs-lookup"><span data-stu-id="70f08-131">Date</span></span>   | <span data-ttu-id="70f08-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="70f08-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="70f08-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="70f08-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="70f08-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="70f08-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="70f08-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="70f08-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="70f08-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70f08-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="70f08-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="70f08-137">The default output type is text/csv.</span></span> <span data-ttu-id="70f08-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="70f08-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70f08-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70f08-139">Request headers</span></span>

| <span data-ttu-id="70f08-140">Имя</span><span class="sxs-lookup"><span data-stu-id="70f08-140">Name</span></span>          | <span data-ttu-id="70f08-141">Описание</span><span class="sxs-lookup"><span data-stu-id="70f08-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="70f08-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70f08-142">Authorization</span></span> | <span data-ttu-id="70f08-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70f08-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="70f08-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="70f08-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="70f08-146">CSV</span><span class="sxs-lookup"><span data-stu-id="70f08-146">CSV</span></span>

<span data-ttu-id="70f08-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="70f08-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70f08-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="70f08-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70f08-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="70f08-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70f08-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="70f08-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="70f08-151">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="70f08-151">Report Refresh Date</span></span>
- <span data-ttu-id="70f08-152">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="70f08-152">Group Display Name</span></span>
- <span data-ttu-id="70f08-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="70f08-153">Is Deleted</span></span>
- <span data-ttu-id="70f08-154">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="70f08-154">Owner Principal Name</span></span>
- <span data-ttu-id="70f08-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="70f08-155">Last Activity Date</span></span>
- <span data-ttu-id="70f08-156">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="70f08-156">Group Type</span></span>
- <span data-ttu-id="70f08-157">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="70f08-157">Office 365 Connected</span></span>
- <span data-ttu-id="70f08-158">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="70f08-158">Member Count</span></span>
- <span data-ttu-id="70f08-159">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="70f08-159">Posted Count</span></span>
- <span data-ttu-id="70f08-160">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="70f08-160">Read Count</span></span>
- <span data-ttu-id="70f08-161">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="70f08-161">Liked Count</span></span>
- <span data-ttu-id="70f08-162">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="70f08-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="70f08-163">JSON</span><span class="sxs-lookup"><span data-stu-id="70f08-163">JSON</span></span>

<span data-ttu-id="70f08-164">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="70f08-164">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="70f08-165">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="70f08-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="70f08-166">Пример</span><span class="sxs-lookup"><span data-stu-id="70f08-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="70f08-167">CSV</span><span class="sxs-lookup"><span data-stu-id="70f08-167">CSV</span></span>

<span data-ttu-id="70f08-168">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="70f08-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="70f08-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="70f08-169">Request</span></span>

<span data-ttu-id="70f08-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70f08-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="70f08-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="70f08-171">Response</span></span>

<span data-ttu-id="70f08-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="70f08-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="70f08-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="70f08-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="70f08-174">JSON</span><span class="sxs-lookup"><span data-stu-id="70f08-174">JSON</span></span>

<span data-ttu-id="70f08-175">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="70f08-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="70f08-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="70f08-176">Request</span></span>

<span data-ttu-id="70f08-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70f08-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="70f08-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="70f08-178">Response</span></span>

<span data-ttu-id="70f08-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70f08-179">The following is an example of the response.</span></span>

> <span data-ttu-id="70f08-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70f08-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
