---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Узнайте, сколько всего существовало групп и в скольких из них выполнялись действия с беседами.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: cf75cd1ada88b1de4fead4edfada4f004bca2809
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982763"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="40765-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="40765-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

<span data-ttu-id="40765-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40765-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40765-105">Узнайте, сколько всего существовало групп и в скольких из них была активность.</span><span class="sxs-lookup"><span data-stu-id="40765-105">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="40765-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 о](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)действиях в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="40765-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="40765-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40765-107">Permissions</span></span>

<span data-ttu-id="40765-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40765-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40765-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40765-110">Permission type</span></span>                        | <span data-ttu-id="40765-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40765-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="40765-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40765-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="40765-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40765-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="40765-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40765-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40765-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40765-115">Not supported.</span></span>                           |
| <span data-ttu-id="40765-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40765-116">Application</span></span>                            | <span data-ttu-id="40765-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40765-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="40765-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="40765-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="40765-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="40765-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="40765-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40765-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="40765-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="40765-121">Function parameters</span></span>

<span data-ttu-id="40765-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="40765-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="40765-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="40765-123">Parameter</span></span> | <span data-ttu-id="40765-124">Тип</span><span class="sxs-lookup"><span data-stu-id="40765-124">Type</span></span>   | <span data-ttu-id="40765-125">Описание</span><span class="sxs-lookup"><span data-stu-id="40765-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="40765-126">period</span><span class="sxs-lookup"><span data-stu-id="40765-126">period</span></span>    | <span data-ttu-id="40765-127">string</span><span class="sxs-lookup"><span data-stu-id="40765-127">string</span></span> | <span data-ttu-id="40765-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="40765-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="40765-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="40765-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="40765-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="40765-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="40765-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40765-131">Required.</span></span> |

<span data-ttu-id="40765-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="40765-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="40765-133">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="40765-133">The default output type is text/csv.</span></span> <span data-ttu-id="40765-134">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="40765-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40765-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40765-135">Request headers</span></span>

| <span data-ttu-id="40765-136">Имя</span><span class="sxs-lookup"><span data-stu-id="40765-136">Name</span></span>          | <span data-ttu-id="40765-137">Описание</span><span class="sxs-lookup"><span data-stu-id="40765-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="40765-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40765-138">Authorization</span></span> | <span data-ttu-id="40765-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40765-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="40765-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="40765-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="40765-142">CSV</span><span class="sxs-lookup"><span data-stu-id="40765-142">CSV</span></span>

<span data-ttu-id="40765-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="40765-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="40765-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="40765-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="40765-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="40765-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="40765-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="40765-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="40765-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="40765-147">Report Refresh Date</span></span>
- <span data-ttu-id="40765-148">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="40765-148">Total</span></span>
- <span data-ttu-id="40765-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="40765-149">Active</span></span>
- <span data-ttu-id="40765-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="40765-150">Report Date</span></span>
- <span data-ttu-id="40765-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="40765-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="40765-152">JSON</span><span class="sxs-lookup"><span data-stu-id="40765-152">JSON</span></span>

<span data-ttu-id="40765-153">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40765-153">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40765-154">Пример</span><span class="sxs-lookup"><span data-stu-id="40765-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="40765-155">CSV</span><span class="sxs-lookup"><span data-stu-id="40765-155">CSV</span></span>

<span data-ttu-id="40765-156">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="40765-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="40765-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="40765-157">Request</span></span>

<span data-ttu-id="40765-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40765-158">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammergroupsactivitygroupcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="40765-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="40765-159">Response</span></span>

<span data-ttu-id="40765-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40765-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="40765-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="40765-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="40765-162">JSON</span><span class="sxs-lookup"><span data-stu-id="40765-162">JSON</span></span>

<span data-ttu-id="40765-163">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="40765-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="40765-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="40765-164">Request</span></span>

<span data-ttu-id="40765-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40765-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammergroupsactivitygroupcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="40765-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="40765-166">Response</span></span>

<span data-ttu-id="40765-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40765-167">The following is an example of the response.</span></span>

> <span data-ttu-id="40765-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40765-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01",
      "total": 50, 
      "active": 41, 
      "reportDate": "2017-09-01", 
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


