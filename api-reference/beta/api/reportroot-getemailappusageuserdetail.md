---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.
localization_priority: Normal
ms.openlocfilehash: a00dae579d90ae705c0c63d7d37065c9bf7850f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876911"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="8eb08-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="8eb08-103">reportRoot: getEmailAppUsageUserDetail</span></span>

> <span data-ttu-id="8eb08-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8eb08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eb08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eb08-106">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="8eb08-106">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="8eb08-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="8eb08-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8eb08-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb08-108">Permissions</span></span>

<span data-ttu-id="8eb08-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8eb08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb08-111">Permission type</span></span>                        | <span data-ttu-id="8eb08-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eb08-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8eb08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eb08-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8eb08-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eb08-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8eb08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eb08-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eb08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb08-116">Not supported.</span></span>                           |
| <span data-ttu-id="8eb08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8eb08-117">Application</span></span>                            | <span data-ttu-id="8eb08-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eb08-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8eb08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eb08-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="8eb08-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="8eb08-120">Function parameters</span></span>

<span data-ttu-id="8eb08-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8eb08-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8eb08-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8eb08-122">Parameter</span></span> | <span data-ttu-id="8eb08-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb08-123">Type</span></span>   | <span data-ttu-id="8eb08-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb08-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8eb08-125">period</span><span class="sxs-lookup"><span data-stu-id="8eb08-125">period</span></span>    | <span data-ttu-id="8eb08-126">строка</span><span class="sxs-lookup"><span data-stu-id="8eb08-126">string</span></span> | <span data-ttu-id="8eb08-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8eb08-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8eb08-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8eb08-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8eb08-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8eb08-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8eb08-130">date</span><span class="sxs-lookup"><span data-stu-id="8eb08-130">date</span></span>      | <span data-ttu-id="8eb08-131">Date</span><span class="sxs-lookup"><span data-stu-id="8eb08-131">Date</span></span>   | <span data-ttu-id="8eb08-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="8eb08-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8eb08-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="8eb08-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8eb08-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="8eb08-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8eb08-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="8eb08-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="8eb08-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb08-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8eb08-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="8eb08-137">The default output type is text/csv.</span></span> <span data-ttu-id="8eb08-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="8eb08-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8eb08-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eb08-139">Request headers</span></span>

| <span data-ttu-id="8eb08-140">Имя</span><span class="sxs-lookup"><span data-stu-id="8eb08-140">Name</span></span>          | <span data-ttu-id="8eb08-141">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb08-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8eb08-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8eb08-142">Authorization</span></span> | <span data-ttu-id="8eb08-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eb08-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8eb08-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb08-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8eb08-146">CSV</span><span class="sxs-lookup"><span data-stu-id="8eb08-146">CSV</span></span>

<span data-ttu-id="8eb08-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8eb08-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8eb08-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8eb08-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8eb08-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8eb08-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8eb08-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8eb08-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8eb08-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8eb08-151">Report Refresh Date</span></span>
- <span data-ttu-id="8eb08-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="8eb08-152">User Principal Name</span></span>
- <span data-ttu-id="8eb08-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="8eb08-153">Display Name</span></span>
- <span data-ttu-id="8eb08-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="8eb08-154">Is Deleted</span></span>
- <span data-ttu-id="8eb08-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="8eb08-155">Deleted Date</span></span>
- <span data-ttu-id="8eb08-156">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="8eb08-156">Last Activity Date</span></span>
- <span data-ttu-id="8eb08-157">"Mail For Mac" (Почта для Mac);</span><span class="sxs-lookup"><span data-stu-id="8eb08-157">Mail For Mac</span></span>
- <span data-ttu-id="8eb08-158">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="8eb08-158">Outlook For Mac</span></span>
- <span data-ttu-id="8eb08-159">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="8eb08-159">Outlook For Windows</span></span>
- <span data-ttu-id="8eb08-160">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="8eb08-160">Outlook For Mobile</span></span>
- <span data-ttu-id="8eb08-161">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="8eb08-161">Other For Mobile</span></span>
- <span data-ttu-id="8eb08-162">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="8eb08-162">Outlook For Web</span></span>
- <span data-ttu-id="8eb08-163">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="8eb08-163">POP3 App</span></span>
- <span data-ttu-id="8eb08-164">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="8eb08-164">IMAP4 App</span></span>
- <span data-ttu-id="8eb08-165">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="8eb08-165">SMTP App</span></span>
- <span data-ttu-id="8eb08-166">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="8eb08-166">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8eb08-167">JSON</span><span class="sxs-lookup"><span data-stu-id="8eb08-167">JSON</span></span>

<span data-ttu-id="8eb08-168">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb08-168">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="8eb08-169">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="8eb08-169">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="8eb08-170">Пример</span><span class="sxs-lookup"><span data-stu-id="8eb08-170">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8eb08-171">CSV</span><span class="sxs-lookup"><span data-stu-id="8eb08-171">CSV</span></span>

<span data-ttu-id="8eb08-172">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="8eb08-172">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8eb08-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eb08-173">Request</span></span>

<span data-ttu-id="8eb08-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eb08-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8eb08-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb08-175">Response</span></span>

<span data-ttu-id="8eb08-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb08-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8eb08-177">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8eb08-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8eb08-178">JSON</span><span class="sxs-lookup"><span data-stu-id="8eb08-178">JSON</span></span>

<span data-ttu-id="8eb08-179">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="8eb08-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8eb08-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eb08-180">Request</span></span>

<span data-ttu-id="8eb08-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eb08-181">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8eb08-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb08-182">Response</span></span>

<span data-ttu-id="8eb08-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8eb08-183">The following is an example of the response.</span></span>

> <span data-ttu-id="8eb08-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8eb08-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
