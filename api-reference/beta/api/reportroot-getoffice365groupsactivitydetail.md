---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Получите сведения об активности в группах Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 347685329e73527c99b48b21573c026c0e1956f9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869159"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="5a5db-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="5a5db-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a5db-104">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="5a5db-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="5a5db-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="5a5db-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a5db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a5db-106">Permissions</span></span>

<span data-ttu-id="5a5db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a5db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a5db-109">Permission type</span></span>                        | <span data-ttu-id="5a5db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a5db-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5a5db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a5db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a5db-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a5db-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5a5db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a5db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a5db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a5db-114">Not supported.</span></span>                           |
| <span data-ttu-id="5a5db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a5db-115">Application</span></span>                            | <span data-ttu-id="5a5db-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a5db-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="5a5db-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a5db-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5a5db-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5a5db-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5a5db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a5db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5a5db-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5a5db-120">Function parameters</span></span>

<span data-ttu-id="5a5db-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5a5db-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5a5db-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a5db-122">Parameter</span></span> | <span data-ttu-id="5a5db-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5a5db-123">Type</span></span>   | <span data-ttu-id="5a5db-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5a5db-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5a5db-125">period</span><span class="sxs-lookup"><span data-stu-id="5a5db-125">period</span></span>    | <span data-ttu-id="5a5db-126">string</span><span class="sxs-lookup"><span data-stu-id="5a5db-126">string</span></span> | <span data-ttu-id="5a5db-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5a5db-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5a5db-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5a5db-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5a5db-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5a5db-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5a5db-130">date</span><span class="sxs-lookup"><span data-stu-id="5a5db-130">date</span></span>      | <span data-ttu-id="5a5db-131">Date</span><span class="sxs-lookup"><span data-stu-id="5a5db-131">Date</span></span>   | <span data-ttu-id="5a5db-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="5a5db-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5a5db-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5a5db-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5a5db-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="5a5db-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5a5db-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="5a5db-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="5a5db-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5a5db-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5a5db-137">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="5a5db-137">The default output type is text/csv.</span></span> <span data-ttu-id="5a5db-138">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5a5db-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a5db-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a5db-139">Request headers</span></span>

| <span data-ttu-id="5a5db-140">Имя</span><span class="sxs-lookup"><span data-stu-id="5a5db-140">Name</span></span>          | <span data-ttu-id="5a5db-141">Описание</span><span class="sxs-lookup"><span data-stu-id="5a5db-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5a5db-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a5db-142">Authorization</span></span> | <span data-ttu-id="5a5db-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a5db-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5a5db-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a5db-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5a5db-146">CSV</span><span class="sxs-lookup"><span data-stu-id="5a5db-146">CSV</span></span>

<span data-ttu-id="5a5db-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5a5db-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5a5db-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5a5db-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5a5db-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5a5db-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5a5db-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5a5db-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5a5db-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5a5db-151">Report Refresh Date</span></span>
- <span data-ttu-id="5a5db-152">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="5a5db-152">Group Display Name</span></span>
- <span data-ttu-id="5a5db-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="5a5db-153">Is Deleted</span></span>
- <span data-ttu-id="5a5db-154">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="5a5db-154">Owner Principal Name</span></span>
- <span data-ttu-id="5a5db-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="5a5db-155">Last Activity Date</span></span>
- <span data-ttu-id="5a5db-156">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="5a5db-156">Group Type</span></span>
- <span data-ttu-id="5a5db-157">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="5a5db-157">Member Count</span></span>
- <span data-ttu-id="5a5db-158">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="5a5db-158">External Member Count</span></span>
- <span data-ttu-id="5a5db-159">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="5a5db-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="5a5db-160">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="5a5db-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="5a5db-161">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5a5db-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="5a5db-162">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5a5db-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="5a5db-163">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5a5db-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="5a5db-164">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="5a5db-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="5a5db-165">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="5a5db-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="5a5db-166">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="5a5db-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="5a5db-167">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="5a5db-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="5a5db-168">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="5a5db-168">Group Id</span></span>
- <span data-ttu-id="5a5db-169">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="5a5db-169">Report Period</span></span>

<span data-ttu-id="5a5db-170">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="5a5db-170">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5a5db-171">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5a5db-171">Yammer Posted Message Count</span></span>
- <span data-ttu-id="5a5db-172">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5a5db-172">Yammer Read Message Count</span></span>
- <span data-ttu-id="5a5db-173">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="5a5db-173">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="5a5db-174">JSON</span><span class="sxs-lookup"><span data-stu-id="5a5db-174">JSON</span></span>

<span data-ttu-id="5a5db-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a5db-175">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="5a5db-176">Следующие свойства в объекте **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="5a5db-176">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5a5db-177">яммерпостедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="5a5db-177">yammerPostedMessageCount</span></span>
- <span data-ttu-id="5a5db-178">яммерреадмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="5a5db-178">yammerReadMessageCount</span></span>
- <span data-ttu-id="5a5db-179">яммерликедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="5a5db-179">yammerLikedMessageCount</span></span>

<span data-ttu-id="5a5db-180">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="5a5db-180">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="5a5db-181">Пример</span><span class="sxs-lookup"><span data-stu-id="5a5db-181">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5a5db-182">CSV</span><span class="sxs-lookup"><span data-stu-id="5a5db-182">CSV</span></span>

<span data-ttu-id="5a5db-183">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="5a5db-183">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5a5db-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a5db-184">Request</span></span>

<span data-ttu-id="5a5db-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a5db-185">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5a5db-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a5db-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a5db-187">C#</span><span class="sxs-lookup"><span data-stu-id="5a5db-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a5db-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a5db-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a5db-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a5db-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a5db-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a5db-190">Response</span></span>

<span data-ttu-id="5a5db-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a5db-191">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5a5db-192">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5a5db-192">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5a5db-193">JSON</span><span class="sxs-lookup"><span data-stu-id="5a5db-193">JSON</span></span>

<span data-ttu-id="5a5db-194">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="5a5db-194">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5a5db-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a5db-195">Request</span></span>

<span data-ttu-id="5a5db-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a5db-196">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5a5db-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a5db-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a5db-198">C#</span><span class="sxs-lookup"><span data-stu-id="5a5db-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a5db-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a5db-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a5db-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a5db-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5a5db-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a5db-201">Response</span></span>

<span data-ttu-id="5a5db-202">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a5db-202">The following is an example of the response.</span></span>

> <span data-ttu-id="5a5db-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a5db-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
