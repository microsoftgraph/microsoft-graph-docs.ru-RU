---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждого почтового приложения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a4a53b7f0acd79594f4e567efe60fa2eefd775d3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896401"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="b00cf-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="b00cf-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="b00cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b00cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b00cf-105">Узнайте, сколько уникальных пользователей у каждого почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="b00cf-105">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="b00cf-106">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="b00cf-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b00cf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b00cf-107">Permissions</span></span>

<span data-ttu-id="b00cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b00cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b00cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b00cf-110">Permission type</span></span>                        | <span data-ttu-id="b00cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b00cf-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b00cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b00cf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b00cf-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b00cf-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b00cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b00cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b00cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b00cf-115">Not supported.</span></span>                           |
| <span data-ttu-id="b00cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b00cf-116">Application</span></span>                            | <span data-ttu-id="b00cf-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b00cf-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="b00cf-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b00cf-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b00cf-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b00cf-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b00cf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b00cf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b00cf-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b00cf-121">Function parameters</span></span>

<span data-ttu-id="b00cf-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b00cf-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b00cf-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="b00cf-123">Parameter</span></span> | <span data-ttu-id="b00cf-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b00cf-124">Type</span></span>   | <span data-ttu-id="b00cf-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b00cf-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b00cf-126">period</span><span class="sxs-lookup"><span data-stu-id="b00cf-126">period</span></span>    | <span data-ttu-id="b00cf-127">string</span><span class="sxs-lookup"><span data-stu-id="b00cf-127">string</span></span> | <span data-ttu-id="b00cf-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b00cf-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b00cf-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b00cf-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b00cf-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b00cf-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b00cf-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b00cf-131">Required.</span></span> |

<span data-ttu-id="b00cf-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b00cf-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b00cf-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="b00cf-133">The default output type is text/csv.</span></span> <span data-ttu-id="b00cf-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b00cf-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b00cf-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b00cf-135">Request headers</span></span>

| <span data-ttu-id="b00cf-136">Имя</span><span class="sxs-lookup"><span data-stu-id="b00cf-136">Name</span></span>          | <span data-ttu-id="b00cf-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b00cf-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b00cf-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b00cf-138">Authorization</span></span> | <span data-ttu-id="b00cf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b00cf-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b00cf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00cf-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b00cf-142">CSV</span><span class="sxs-lookup"><span data-stu-id="b00cf-142">CSV</span></span>

<span data-ttu-id="b00cf-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b00cf-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b00cf-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b00cf-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b00cf-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b00cf-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b00cf-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b00cf-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b00cf-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b00cf-147">Report Refresh Date</span></span>
- <span data-ttu-id="b00cf-148">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="b00cf-148">Mail For Mac</span></span>
- <span data-ttu-id="b00cf-149">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="b00cf-149">Outlook For Mac</span></span>
- <span data-ttu-id="b00cf-150">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="b00cf-150">Outlook For Windows</span></span>
- <span data-ttu-id="b00cf-151">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="b00cf-151">Outlook For Mobile</span></span>
- <span data-ttu-id="b00cf-152">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="b00cf-152">Other For Mobile</span></span>
- <span data-ttu-id="b00cf-153">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="b00cf-153">Outlook For Web</span></span>
- <span data-ttu-id="b00cf-154">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="b00cf-154">POP3 App</span></span>
- <span data-ttu-id="b00cf-155">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="b00cf-155">IMAP4 App</span></span>
- <span data-ttu-id="b00cf-156">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="b00cf-156">SMTP App</span></span>
- <span data-ttu-id="b00cf-157">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b00cf-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b00cf-158">JSON</span><span class="sxs-lookup"><span data-stu-id="b00cf-158">JSON</span></span>

<span data-ttu-id="b00cf-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеаппсусеркаунтс](../resources/emailappusageappsusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b00cf-159">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b00cf-160">Пример</span><span class="sxs-lookup"><span data-stu-id="b00cf-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b00cf-161">CSV</span><span class="sxs-lookup"><span data-stu-id="b00cf-161">CSV</span></span>

<span data-ttu-id="b00cf-162">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="b00cf-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b00cf-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b00cf-163">Request</span></span>

<span data-ttu-id="b00cf-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b00cf-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="b00cf-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00cf-165">Response</span></span>

<span data-ttu-id="b00cf-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b00cf-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b00cf-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b00cf-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="b00cf-168">JSON</span><span class="sxs-lookup"><span data-stu-id="b00cf-168">JSON</span></span>

<span data-ttu-id="b00cf-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="b00cf-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b00cf-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="b00cf-170">Request</span></span>

<span data-ttu-id="b00cf-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b00cf-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="b00cf-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00cf-172">Response</span></span>

<span data-ttu-id="b00cf-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b00cf-173">The following is an example of the response.</span></span>

> <span data-ttu-id="b00cf-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b00cf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageAppsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 4, 
      "outlookForMac": 105, 
      "outlookForWindows": 1589, 
      "outlookForMobile": 1116, 
      "otherForMobile": 485, 
      "outlookForWeb": 753, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
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
