---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Узнайте, сколько различных действий было в группах.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 85eab0e6fa7d4e0c541e8745144662fa4631fb4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508645"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="6bd03-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6bd03-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bd03-104">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="6bd03-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="6bd03-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="6bd03-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bd03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bd03-106">Permissions</span></span>

<span data-ttu-id="6bd03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bd03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bd03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bd03-109">Permission type</span></span>                        | <span data-ttu-id="6bd03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bd03-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6bd03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bd03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bd03-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bd03-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6bd03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bd03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bd03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bd03-114">Not supported.</span></span>                           |
| <span data-ttu-id="6bd03-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bd03-115">Application</span></span>                            | <span data-ttu-id="6bd03-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bd03-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6bd03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bd03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6bd03-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6bd03-118">Function parameters</span></span>

<span data-ttu-id="6bd03-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6bd03-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6bd03-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6bd03-120">Parameter</span></span> | <span data-ttu-id="6bd03-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6bd03-121">Type</span></span>   | <span data-ttu-id="6bd03-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6bd03-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6bd03-123">period</span><span class="sxs-lookup"><span data-stu-id="6bd03-123">period</span></span>    | <span data-ttu-id="6bd03-124">строка</span><span class="sxs-lookup"><span data-stu-id="6bd03-124">string</span></span> | <span data-ttu-id="6bd03-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6bd03-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6bd03-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6bd03-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6bd03-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6bd03-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6bd03-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bd03-128">Required.</span></span> |

<span data-ttu-id="6bd03-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6bd03-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6bd03-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="6bd03-130">The default output type is text/csv.</span></span> <span data-ttu-id="6bd03-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="6bd03-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bd03-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bd03-132">Request headers</span></span>

| <span data-ttu-id="6bd03-133">Имя</span><span class="sxs-lookup"><span data-stu-id="6bd03-133">Name</span></span>          | <span data-ttu-id="6bd03-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6bd03-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6bd03-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bd03-135">Authorization</span></span> | <span data-ttu-id="6bd03-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bd03-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6bd03-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bd03-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6bd03-139">CSV</span><span class="sxs-lookup"><span data-stu-id="6bd03-139">CSV</span></span>

<span data-ttu-id="6bd03-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6bd03-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6bd03-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6bd03-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6bd03-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6bd03-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6bd03-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6bd03-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6bd03-144">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="6bd03-144">Report Refresh Date</span></span>
- <span data-ttu-id="6bd03-145">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="6bd03-145">Exchange Emails Received</span></span>
- <span data-ttu-id="6bd03-146">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6bd03-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="6bd03-147">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6bd03-147">Yammer Messages Read</span></span>
- <span data-ttu-id="6bd03-148">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6bd03-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="6bd03-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="6bd03-149">Report Date</span></span>
- <span data-ttu-id="6bd03-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6bd03-150">Report Period</span></span>

<span data-ttu-id="6bd03-151">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="6bd03-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6bd03-152">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6bd03-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="6bd03-153">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6bd03-153">Yammer Messages Read</span></span>
- <span data-ttu-id="6bd03-154">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6bd03-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="6bd03-155">JSON</span><span class="sxs-lookup"><span data-stu-id="6bd03-155">JSON</span></span>

<span data-ttu-id="6bd03-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6bd03-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="6bd03-157">Следующие свойства объекта **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="6bd03-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6bd03-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="6bd03-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="6bd03-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="6bd03-159">yammerMessagesRead</span></span>
- <span data-ttu-id="6bd03-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="6bd03-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="6bd03-161">Пример</span><span class="sxs-lookup"><span data-stu-id="6bd03-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6bd03-162">CSV</span><span class="sxs-lookup"><span data-stu-id="6bd03-162">CSV</span></span>

<span data-ttu-id="6bd03-163">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="6bd03-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6bd03-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bd03-164">Request</span></span>

<span data-ttu-id="6bd03-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bd03-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6bd03-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bd03-166">Response</span></span>

<span data-ttu-id="6bd03-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6bd03-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6bd03-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6bd03-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="6bd03-169">JSON</span><span class="sxs-lookup"><span data-stu-id="6bd03-169">JSON</span></span>

<span data-ttu-id="6bd03-170">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="6bd03-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6bd03-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bd03-171">Request</span></span>

<span data-ttu-id="6bd03-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bd03-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6bd03-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bd03-173">Response</span></span>

<span data-ttu-id="6bd03-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bd03-174">The following is an example of the response.</span></span>

> <span data-ttu-id="6bd03-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6bd03-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
