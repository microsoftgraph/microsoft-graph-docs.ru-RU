---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Узнайте, сколько различных действий было в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ef7fd1b4b7b7cca7ed29bc5591ad576ad414fb7c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896310"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="ce3c8-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ce3c8-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="ce3c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce3c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce3c8-105">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-105">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="ce3c8-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="ce3c8-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce3c8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce3c8-107">Permissions</span></span>

<span data-ttu-id="ce3c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce3c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce3c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce3c8-110">Permission type</span></span>                        | <span data-ttu-id="ce3c8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ce3c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce3c8-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce3c8-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ce3c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce3c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-115">Not supported.</span></span>                           |
| <span data-ttu-id="ce3c8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce3c8-116">Application</span></span>                            | <span data-ttu-id="ce3c8-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce3c8-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ce3c8-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ce3c8-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ce3c8-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ce3c8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce3c8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ce3c8-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ce3c8-121">Function parameters</span></span>

<span data-ttu-id="ce3c8-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ce3c8-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="ce3c8-123">Parameter</span></span> | <span data-ttu-id="ce3c8-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ce3c8-124">Type</span></span>   | <span data-ttu-id="ce3c8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ce3c8-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ce3c8-126">period</span><span class="sxs-lookup"><span data-stu-id="ce3c8-126">period</span></span>    | <span data-ttu-id="ce3c8-127">string</span><span class="sxs-lookup"><span data-stu-id="ce3c8-127">string</span></span> | <span data-ttu-id="ce3c8-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ce3c8-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ce3c8-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ce3c8-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-131">Required.</span></span> |

<span data-ttu-id="ce3c8-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ce3c8-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-133">The default output type is text/csv.</span></span> <span data-ttu-id="ce3c8-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce3c8-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce3c8-135">Request headers</span></span>

| <span data-ttu-id="ce3c8-136">Имя</span><span class="sxs-lookup"><span data-stu-id="ce3c8-136">Name</span></span>          | <span data-ttu-id="ce3c8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ce3c8-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ce3c8-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce3c8-138">Authorization</span></span> | <span data-ttu-id="ce3c8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ce3c8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3c8-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ce3c8-142">CSV</span><span class="sxs-lookup"><span data-stu-id="ce3c8-142">CSV</span></span>

<span data-ttu-id="ce3c8-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ce3c8-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ce3c8-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ce3c8-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ce3c8-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ce3c8-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ce3c8-147">Report Refresh Date</span></span>
- <span data-ttu-id="ce3c8-148">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-148">Exchange Emails Received</span></span>
- <span data-ttu-id="ce3c8-149">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-149">Yammer Messages Posted</span></span>
- <span data-ttu-id="ce3c8-150">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-150">Yammer Messages Read</span></span>
- <span data-ttu-id="ce3c8-151">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-151">Yammer Messages Liked</span></span>
- <span data-ttu-id="ce3c8-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-152">Report Date</span></span>
- <span data-ttu-id="ce3c8-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-153">Report Period</span></span>

<span data-ttu-id="ce3c8-154">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="ce3c8-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="ce3c8-155">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-155">Yammer Messages Posted</span></span>
- <span data-ttu-id="ce3c8-156">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-156">Yammer Messages Read</span></span>
- <span data-ttu-id="ce3c8-157">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ce3c8-157">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="ce3c8-158">JSON</span><span class="sxs-lookup"><span data-stu-id="ce3c8-158">JSON</span></span>

<span data-ttu-id="ce3c8-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-159">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="ce3c8-160">Следующие свойства в объекте **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="ce3c8-160">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="ce3c8-161">яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="ce3c8-161">yammerMessagesPosted</span></span>
- <span data-ttu-id="ce3c8-162">яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="ce3c8-162">yammerMessagesRead</span></span>
- <span data-ttu-id="ce3c8-163">яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="ce3c8-163">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="ce3c8-164">Пример</span><span class="sxs-lookup"><span data-stu-id="ce3c8-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ce3c8-165">CSV</span><span class="sxs-lookup"><span data-stu-id="ce3c8-165">CSV</span></span>

<span data-ttu-id="ce3c8-166">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ce3c8-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce3c8-167">Request</span></span>

<span data-ttu-id="ce3c8-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="ce3c8-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3c8-169">Response</span></span>

<span data-ttu-id="ce3c8-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ce3c8-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ce3c8-172">JSON</span><span class="sxs-lookup"><span data-stu-id="ce3c8-172">JSON</span></span>

<span data-ttu-id="ce3c8-173">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ce3c8-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce3c8-174">Request</span></span>

<span data-ttu-id="ce3c8-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-175">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="ce3c8-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3c8-176">Response</span></span>

<span data-ttu-id="ce3c8-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-177">The following is an example of the response.</span></span>

> <span data-ttu-id="ce3c8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce3c8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
