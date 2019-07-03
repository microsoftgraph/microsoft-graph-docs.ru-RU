---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получите сведения об активности в группах Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b7725ca7f56db7873d49729518a37dd3934ed3d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446887"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="d5128-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d5128-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5128-104">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="d5128-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="d5128-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="d5128-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5128-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5128-106">Permissions</span></span>

<span data-ttu-id="d5128-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5128-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5128-109">Permission type</span></span>                        | <span data-ttu-id="d5128-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5128-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5128-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5128-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5128-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5128-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d5128-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5128-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5128-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5128-114">Not supported.</span></span>                           |
| <span data-ttu-id="d5128-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5128-115">Application</span></span>                            | <span data-ttu-id="d5128-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5128-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d5128-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5128-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d5128-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d5128-118">Function parameters</span></span>

<span data-ttu-id="d5128-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d5128-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d5128-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="d5128-120">Parameter</span></span> | <span data-ttu-id="d5128-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d5128-121">Type</span></span>   | <span data-ttu-id="d5128-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d5128-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5128-123">period</span><span class="sxs-lookup"><span data-stu-id="d5128-123">period</span></span>    | <span data-ttu-id="d5128-124">string</span><span class="sxs-lookup"><span data-stu-id="d5128-124">string</span></span> | <span data-ttu-id="d5128-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d5128-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5128-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d5128-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5128-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d5128-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d5128-128">date</span><span class="sxs-lookup"><span data-stu-id="d5128-128">date</span></span>      | <span data-ttu-id="d5128-129">Date</span><span class="sxs-lookup"><span data-stu-id="d5128-129">Date</span></span>   | <span data-ttu-id="d5128-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="d5128-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d5128-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="d5128-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d5128-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="d5128-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d5128-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="d5128-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d5128-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d5128-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d5128-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="d5128-135">The default output type is text/csv.</span></span> <span data-ttu-id="d5128-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d5128-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5128-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5128-137">Request headers</span></span>

| <span data-ttu-id="d5128-138">Имя</span><span class="sxs-lookup"><span data-stu-id="d5128-138">Name</span></span>          | <span data-ttu-id="d5128-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d5128-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d5128-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5128-140">Authorization</span></span> | <span data-ttu-id="d5128-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5128-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d5128-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5128-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d5128-144">CSV</span><span class="sxs-lookup"><span data-stu-id="d5128-144">CSV</span></span>

<span data-ttu-id="d5128-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d5128-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5128-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d5128-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5128-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d5128-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5128-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d5128-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5128-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d5128-149">Report Refresh Date</span></span>
- <span data-ttu-id="d5128-150">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="d5128-150">Group Display Name</span></span>
- <span data-ttu-id="d5128-151">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="d5128-151">Is Deleted</span></span>
- <span data-ttu-id="d5128-152">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="d5128-152">Owner Principal Name</span></span>
- <span data-ttu-id="d5128-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="d5128-153">Last Activity Date</span></span>
- <span data-ttu-id="d5128-154">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="d5128-154">Group Type</span></span>
- <span data-ttu-id="d5128-155">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="d5128-155">Member Count</span></span>
- <span data-ttu-id="d5128-156">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="d5128-156">External Member Count</span></span>
- <span data-ttu-id="d5128-157">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="d5128-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="d5128-158">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="d5128-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="d5128-159">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="d5128-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="d5128-160">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="d5128-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="d5128-161">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="d5128-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="d5128-162">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="d5128-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="d5128-163">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="d5128-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="d5128-164">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="d5128-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="d5128-165">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="d5128-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="d5128-166">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="d5128-166">Report Period</span></span>

<span data-ttu-id="d5128-167">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="d5128-167">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="d5128-168">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="d5128-168">Yammer Posted Message Count</span></span>
- <span data-ttu-id="d5128-169">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="d5128-169">Yammer Read Message Count</span></span>
- <span data-ttu-id="d5128-170">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="d5128-170">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="d5128-171">JSON</span><span class="sxs-lookup"><span data-stu-id="d5128-171">JSON</span></span>

<span data-ttu-id="d5128-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5128-172">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="d5128-173">Следующие свойства в объекте **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="d5128-173">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="d5128-174">Яммерпостедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="d5128-174">yammerPostedMessageCount</span></span>
- <span data-ttu-id="d5128-175">Яммерреадмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="d5128-175">yammerReadMessageCount</span></span>
- <span data-ttu-id="d5128-176">Яммерликедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="d5128-176">yammerLikedMessageCount</span></span>

<span data-ttu-id="d5128-177">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="d5128-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d5128-178">Пример</span><span class="sxs-lookup"><span data-stu-id="d5128-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d5128-179">CSV</span><span class="sxs-lookup"><span data-stu-id="d5128-179">CSV</span></span>

<span data-ttu-id="d5128-180">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="d5128-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d5128-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5128-181">Request</span></span>

<span data-ttu-id="d5128-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5128-182">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5128-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5128-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5128-184">C#</span><span class="sxs-lookup"><span data-stu-id="d5128-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5128-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5128-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5128-186">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d5128-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5128-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5128-187">Response</span></span>

<span data-ttu-id="d5128-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5128-188">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d5128-189">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d5128-189">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="d5128-190">JSON</span><span class="sxs-lookup"><span data-stu-id="d5128-190">JSON</span></span>

<span data-ttu-id="d5128-191">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="d5128-191">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d5128-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5128-192">Request</span></span>

<span data-ttu-id="d5128-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5128-193">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5128-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5128-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5128-195">C#</span><span class="sxs-lookup"><span data-stu-id="d5128-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5128-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5128-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5128-197">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d5128-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5128-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5128-198">Response</span></span>

<span data-ttu-id="d5128-199">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d5128-199">The following is an example of the response.</span></span>

> <span data-ttu-id="d5128-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5128-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerDisplayName-value", 
      "lastActivityDate": "2017-08-31", 
      "groupType": "Private", 
      "memberCount": 5, 
      "externalMemberCount": 0, 
      "exchangeReceivedEmailCount": 341, 
      "sharePointActiveFileCount": 0, 
      "yammerPostedMessageCount": 0, 
      "yammerReadMessageCount": 0, 
      "yammerLikedMessageCount": 0, 
      "exchangeMailboxTotalItemCount": 343, 
      "exchangeMailboxStorageUsedInBytes": 3724609, 
      "sharePointTotalFileCount": 0, 
      "sharePointSiteStorageUsedInBytes": 0, 
      "reportPeriod": "30"
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
