---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 8a5c8f37508268c52244e0aaa84e61fba4c00b95
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981342"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="0397d-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="0397d-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="0397d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0397d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0397d-105">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="0397d-105">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="0397d-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании почтовых приложений.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)</span><span class="sxs-lookup"><span data-stu-id="0397d-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="0397d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0397d-107">Permissions</span></span>

<span data-ttu-id="0397d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0397d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0397d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0397d-110">Permission type</span></span>                        | <span data-ttu-id="0397d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0397d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0397d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0397d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0397d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0397d-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0397d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0397d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0397d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0397d-115">Not supported.</span></span>                           |
| <span data-ttu-id="0397d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0397d-116">Application</span></span>                            | <span data-ttu-id="0397d-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0397d-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0397d-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0397d-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0397d-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0397d-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0397d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0397d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0397d-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0397d-121">Function parameters</span></span>

<span data-ttu-id="0397d-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0397d-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0397d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="0397d-123">Parameter</span></span> | <span data-ttu-id="0397d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0397d-124">Type</span></span>   | <span data-ttu-id="0397d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0397d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0397d-126">period</span><span class="sxs-lookup"><span data-stu-id="0397d-126">period</span></span>    | <span data-ttu-id="0397d-127">string</span><span class="sxs-lookup"><span data-stu-id="0397d-127">string</span></span> | <span data-ttu-id="0397d-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0397d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0397d-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0397d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0397d-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0397d-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0397d-131">date</span><span class="sxs-lookup"><span data-stu-id="0397d-131">date</span></span>      | <span data-ttu-id="0397d-132">Date</span><span class="sxs-lookup"><span data-stu-id="0397d-132">Date</span></span>   | <span data-ttu-id="0397d-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="0397d-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0397d-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="0397d-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0397d-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="0397d-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0397d-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="0397d-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0397d-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0397d-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0397d-138">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="0397d-138">The default output type is text/csv.</span></span> <span data-ttu-id="0397d-139">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="0397d-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0397d-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0397d-140">Request headers</span></span>

| <span data-ttu-id="0397d-141">Имя</span><span class="sxs-lookup"><span data-stu-id="0397d-141">Name</span></span>          | <span data-ttu-id="0397d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="0397d-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0397d-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0397d-143">Authorization</span></span> | <span data-ttu-id="0397d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0397d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0397d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0397d-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0397d-147">CSV</span><span class="sxs-lookup"><span data-stu-id="0397d-147">CSV</span></span>

<span data-ttu-id="0397d-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0397d-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0397d-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0397d-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0397d-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0397d-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0397d-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0397d-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0397d-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0397d-152">Report Refresh Date</span></span>
- <span data-ttu-id="0397d-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="0397d-153">User Principal Name</span></span>
- <span data-ttu-id="0397d-154">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="0397d-154">Display Name</span></span>
- <span data-ttu-id="0397d-155">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="0397d-155">Is Deleted</span></span>
- <span data-ttu-id="0397d-156">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="0397d-156">Deleted Date</span></span>
- <span data-ttu-id="0397d-157">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="0397d-157">Last Activity Date</span></span>
- <span data-ttu-id="0397d-158">"Mail For Mac" (Почта для Mac);</span><span class="sxs-lookup"><span data-stu-id="0397d-158">Mail For Mac</span></span>
- <span data-ttu-id="0397d-159">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="0397d-159">Outlook For Mac</span></span>
- <span data-ttu-id="0397d-160">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="0397d-160">Outlook For Windows</span></span>
- <span data-ttu-id="0397d-161">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="0397d-161">Outlook For Mobile</span></span>
- <span data-ttu-id="0397d-162">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="0397d-162">Other For Mobile</span></span>
- <span data-ttu-id="0397d-163">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="0397d-163">Outlook For Web</span></span>
- <span data-ttu-id="0397d-164">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="0397d-164">POP3 App</span></span>
- <span data-ttu-id="0397d-165">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="0397d-165">IMAP4 App</span></span>
- <span data-ttu-id="0397d-166">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="0397d-166">SMTP App</span></span>
- <span data-ttu-id="0397d-167">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="0397d-167">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0397d-168">JSON</span><span class="sxs-lookup"><span data-stu-id="0397d-168">JSON</span></span>

<span data-ttu-id="0397d-169">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0397d-169">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="0397d-170">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="0397d-170">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0397d-171">Пример</span><span class="sxs-lookup"><span data-stu-id="0397d-171">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0397d-172">CSV</span><span class="sxs-lookup"><span data-stu-id="0397d-172">CSV</span></span>

<span data-ttu-id="0397d-173">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="0397d-173">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0397d-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="0397d-174">Request</span></span>

<span data-ttu-id="0397d-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0397d-175">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="0397d-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="0397d-176">Response</span></span>

<span data-ttu-id="0397d-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0397d-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0397d-178">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0397d-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="0397d-179">JSON</span><span class="sxs-lookup"><span data-stu-id="0397d-179">JSON</span></span>

<span data-ttu-id="0397d-180">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="0397d-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0397d-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="0397d-181">Request</span></span>

<span data-ttu-id="0397d-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0397d-182">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="0397d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="0397d-183">Response</span></span>

<span data-ttu-id="0397d-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0397d-184">The following is an example of the response.</span></span>

> <span data-ttu-id="0397d-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0397d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
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


