---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 15744a267736d0413d01a760cad459fd7c4aae46
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054947"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="08597-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="08597-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="08597-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08597-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08597-105">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="08597-105">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="08597-106">**Примечание:** Сведения о различных представлениях отчетов и именах см. в [Microsoft 365 отчетов — Yammer групп.](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)</span><span class="sxs-lookup"><span data-stu-id="08597-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="08597-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08597-107">Permissions</span></span>

<span data-ttu-id="08597-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08597-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08597-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08597-110">Permission type</span></span>                        | <span data-ttu-id="08597-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08597-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="08597-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08597-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="08597-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08597-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="08597-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08597-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08597-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08597-115">Not supported.</span></span>                           |
| <span data-ttu-id="08597-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08597-116">Application</span></span>                            | <span data-ttu-id="08597-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08597-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="08597-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08597-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="08597-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="08597-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="08597-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08597-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="08597-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="08597-121">Function parameters</span></span>

<span data-ttu-id="08597-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="08597-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="08597-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="08597-123">Parameter</span></span> | <span data-ttu-id="08597-124">Тип</span><span class="sxs-lookup"><span data-stu-id="08597-124">Type</span></span>   | <span data-ttu-id="08597-125">Описание</span><span class="sxs-lookup"><span data-stu-id="08597-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="08597-126">period</span><span class="sxs-lookup"><span data-stu-id="08597-126">period</span></span>    | <span data-ttu-id="08597-127">string</span><span class="sxs-lookup"><span data-stu-id="08597-127">string</span></span> | <span data-ttu-id="08597-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="08597-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="08597-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="08597-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="08597-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="08597-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="08597-131">date</span><span class="sxs-lookup"><span data-stu-id="08597-131">date</span></span>      | <span data-ttu-id="08597-132">Date</span><span class="sxs-lookup"><span data-stu-id="08597-132">Date</span></span>   | <span data-ttu-id="08597-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="08597-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="08597-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="08597-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="08597-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="08597-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="08597-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="08597-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="08597-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08597-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="08597-138">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="08597-138">The default output type is text/csv.</span></span> <span data-ttu-id="08597-139">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="08597-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08597-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08597-140">Request headers</span></span>

| <span data-ttu-id="08597-141">Имя</span><span class="sxs-lookup"><span data-stu-id="08597-141">Name</span></span>          | <span data-ttu-id="08597-142">Описание</span><span class="sxs-lookup"><span data-stu-id="08597-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="08597-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08597-143">Authorization</span></span> | <span data-ttu-id="08597-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08597-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="08597-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="08597-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="08597-147">CSV</span><span class="sxs-lookup"><span data-stu-id="08597-147">CSV</span></span>

<span data-ttu-id="08597-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="08597-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="08597-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="08597-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="08597-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="08597-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="08597-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="08597-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="08597-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="08597-152">Report Refresh Date</span></span>
- <span data-ttu-id="08597-153">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="08597-153">Group Display Name</span></span>
- <span data-ttu-id="08597-154">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="08597-154">Is Deleted</span></span>
- <span data-ttu-id="08597-155">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="08597-155">Owner Principal Name</span></span>
- <span data-ttu-id="08597-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="08597-156">Last Activity Date</span></span>
- <span data-ttu-id="08597-157">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="08597-157">Group Type</span></span>
- <span data-ttu-id="08597-158">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="08597-158">Office 365 Connected</span></span>
- <span data-ttu-id="08597-159">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="08597-159">Member Count</span></span>
- <span data-ttu-id="08597-160">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="08597-160">Posted Count</span></span>
- <span data-ttu-id="08597-161">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="08597-161">Read Count</span></span>
- <span data-ttu-id="08597-162">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="08597-162">Liked Count</span></span>
- <span data-ttu-id="08597-163">Имя отображения сети</span><span class="sxs-lookup"><span data-stu-id="08597-163">Network Display Name</span></span>
- <span data-ttu-id="08597-164">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="08597-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="08597-165">JSON</span><span class="sxs-lookup"><span data-stu-id="08597-165">JSON</span></span>

<span data-ttu-id="08597-166">В случае успеха этот метод возвращает код ответа и `200 OK` **[объект yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="08597-166">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="08597-167">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="08597-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="08597-168">Пример</span><span class="sxs-lookup"><span data-stu-id="08597-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="08597-169">CSV</span><span class="sxs-lookup"><span data-stu-id="08597-169">CSV</span></span>

<span data-ttu-id="08597-170">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="08597-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="08597-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="08597-171">Request</span></span>

<span data-ttu-id="08597-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08597-172">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="08597-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="08597-173">Response</span></span>

<span data-ttu-id="08597-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08597-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="08597-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="08597-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Network Display Name,Report Period
```

### <a name="json"></a><span data-ttu-id="08597-176">JSON</span><span class="sxs-lookup"><span data-stu-id="08597-176">JSON</span></span>

<span data-ttu-id="08597-177">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="08597-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="08597-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="08597-178">Request</span></span>

<span data-ttu-id="08597-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08597-179">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="08597-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="08597-180">Response</span></span>

<span data-ttu-id="08597-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08597-181">The following is an example of the response.</span></span>

> <span data-ttu-id="08597-182">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="08597-182">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "networkDisplayName": "networkDisplayName-value",
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


