---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Сведения о Microsoft 365 групп по группам.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: dde570c4cdfb55adb6ccf72ff3702e928b8f2944
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036671"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="021ab-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="021ab-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="021ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="021ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="021ab-105">Сведения о Microsoft 365 групп по группам.</span><span class="sxs-lookup"><span data-stu-id="021ab-105">Get details about Microsoft 365 groups activity by group.</span></span>

> <span data-ttu-id="021ab-106">**Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft 365 групп.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="021ab-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="021ab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="021ab-107">Permissions</span></span>

<span data-ttu-id="021ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="021ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="021ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="021ab-110">Permission type</span></span>                        | <span data-ttu-id="021ab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="021ab-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="021ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="021ab-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="021ab-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="021ab-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="021ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="021ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="021ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="021ab-115">Not supported.</span></span>                           |
| <span data-ttu-id="021ab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="021ab-116">Application</span></span>                            | <span data-ttu-id="021ab-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="021ab-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="021ab-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="021ab-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="021ab-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="021ab-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="021ab-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="021ab-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="021ab-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="021ab-121">Function parameters</span></span>

<span data-ttu-id="021ab-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="021ab-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="021ab-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="021ab-123">Parameter</span></span> | <span data-ttu-id="021ab-124">Тип</span><span class="sxs-lookup"><span data-stu-id="021ab-124">Type</span></span>   | <span data-ttu-id="021ab-125">Описание</span><span class="sxs-lookup"><span data-stu-id="021ab-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="021ab-126">period</span><span class="sxs-lookup"><span data-stu-id="021ab-126">period</span></span>    | <span data-ttu-id="021ab-127">string</span><span class="sxs-lookup"><span data-stu-id="021ab-127">string</span></span> | <span data-ttu-id="021ab-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="021ab-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="021ab-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="021ab-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="021ab-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="021ab-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="021ab-131">date</span><span class="sxs-lookup"><span data-stu-id="021ab-131">date</span></span>      | <span data-ttu-id="021ab-132">Date</span><span class="sxs-lookup"><span data-stu-id="021ab-132">Date</span></span>   | <span data-ttu-id="021ab-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="021ab-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="021ab-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="021ab-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="021ab-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="021ab-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="021ab-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="021ab-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="021ab-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="021ab-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="021ab-138">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="021ab-138">The default output type is text/csv.</span></span> <span data-ttu-id="021ab-139">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="021ab-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="021ab-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="021ab-140">Request headers</span></span>

| <span data-ttu-id="021ab-141">Имя</span><span class="sxs-lookup"><span data-stu-id="021ab-141">Name</span></span>          | <span data-ttu-id="021ab-142">Описание</span><span class="sxs-lookup"><span data-stu-id="021ab-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="021ab-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="021ab-143">Authorization</span></span> | <span data-ttu-id="021ab-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="021ab-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="021ab-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="021ab-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="021ab-147">CSV</span><span class="sxs-lookup"><span data-stu-id="021ab-147">CSV</span></span>

<span data-ttu-id="021ab-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="021ab-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="021ab-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="021ab-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="021ab-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="021ab-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="021ab-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="021ab-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="021ab-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="021ab-152">Report Refresh Date</span></span>
- <span data-ttu-id="021ab-153">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="021ab-153">Group Display Name</span></span>
- <span data-ttu-id="021ab-154">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="021ab-154">Is Deleted</span></span>
- <span data-ttu-id="021ab-155">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="021ab-155">Owner Principal Name</span></span>
- <span data-ttu-id="021ab-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="021ab-156">Last Activity Date</span></span>
- <span data-ttu-id="021ab-157">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="021ab-157">Group Type</span></span>
- <span data-ttu-id="021ab-158">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="021ab-158">Member Count</span></span>
- <span data-ttu-id="021ab-159">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="021ab-159">External Member Count</span></span>
- <span data-ttu-id="021ab-160">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="021ab-160">Exchange Received Email Count</span></span>
- <span data-ttu-id="021ab-161">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="021ab-161">SharePoint Active File Count</span></span>
- <span data-ttu-id="021ab-162">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="021ab-162">Yammer Posted Message Count</span></span>
- <span data-ttu-id="021ab-163">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="021ab-163">Yammer Read Message Count</span></span>
- <span data-ttu-id="021ab-164">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="021ab-164">Yammer Liked Message Count</span></span>
- <span data-ttu-id="021ab-165">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="021ab-165">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="021ab-166">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="021ab-166">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="021ab-167">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="021ab-167">SharePoint Total File Count</span></span>
- <span data-ttu-id="021ab-168">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="021ab-168">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="021ab-169">Group Id</span><span class="sxs-lookup"><span data-stu-id="021ab-169">Group Id</span></span>
- <span data-ttu-id="021ab-170">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="021ab-170">Report Period</span></span>

<span data-ttu-id="021ab-171">Следующие столбцы не поддерживаются в Microsoft Graph Китае, выполняемых 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="021ab-171">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="021ab-172">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="021ab-172">Yammer Posted Message Count</span></span>
- <span data-ttu-id="021ab-173">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="021ab-173">Yammer Read Message Count</span></span>
- <span data-ttu-id="021ab-174">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="021ab-174">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="021ab-175">JSON</span><span class="sxs-lookup"><span data-stu-id="021ab-175">JSON</span></span>

<span data-ttu-id="021ab-176">В случае успеха этот метод возвращает код ответа и `200 OK` **[объект Office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="021ab-176">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="021ab-177">Следующие свойства в **[объекте Office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** не поддерживаются в Microsoft Graph Китае под управлением 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="021ab-177">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="021ab-178">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="021ab-178">yammerPostedMessageCount</span></span>
- <span data-ttu-id="021ab-179">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="021ab-179">yammerReadMessageCount</span></span>
- <span data-ttu-id="021ab-180">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="021ab-180">yammerLikedMessageCount</span></span>

<span data-ttu-id="021ab-181">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="021ab-181">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="021ab-182">Пример</span><span class="sxs-lookup"><span data-stu-id="021ab-182">Example</span></span>

### <a name="csv"></a><span data-ttu-id="021ab-183">CSV</span><span class="sxs-lookup"><span data-stu-id="021ab-183">CSV</span></span>

<span data-ttu-id="021ab-184">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="021ab-184">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="021ab-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="021ab-185">Request</span></span>

<span data-ttu-id="021ab-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="021ab-186">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="021ab-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="021ab-187">Response</span></span>

<span data-ttu-id="021ab-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="021ab-188">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="021ab-189">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="021ab-189">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
```

### <a name="json"></a><span data-ttu-id="021ab-190">JSON</span><span class="sxs-lookup"><span data-stu-id="021ab-190">JSON</span></span>

<span data-ttu-id="021ab-191">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="021ab-191">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="021ab-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="021ab-192">Request</span></span>

<span data-ttu-id="021ab-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="021ab-193">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="021ab-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="021ab-194">Response</span></span>

<span data-ttu-id="021ab-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="021ab-195">The following is an example of the response.</span></span>

> <span data-ttu-id="021ab-196">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="021ab-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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


