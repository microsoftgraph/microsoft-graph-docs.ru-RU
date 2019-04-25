---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4887910d6b0bdc1474be83ad0fc146a41051e396
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546092"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="02e25-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="02e25-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02e25-104">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="02e25-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="02e25-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="02e25-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="02e25-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02e25-106">Permissions</span></span>

<span data-ttu-id="02e25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02e25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02e25-109">Permission type</span></span>                        | <span data-ttu-id="02e25-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02e25-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="02e25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02e25-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="02e25-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e25-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="02e25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02e25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02e25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e25-114">Not supported.</span></span>                           |
| <span data-ttu-id="02e25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02e25-115">Application</span></span>                            | <span data-ttu-id="02e25-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e25-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="02e25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02e25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="02e25-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="02e25-118">Function parameters</span></span>

<span data-ttu-id="02e25-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="02e25-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="02e25-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="02e25-120">Parameter</span></span> | <span data-ttu-id="02e25-121">Тип</span><span class="sxs-lookup"><span data-stu-id="02e25-121">Type</span></span>   | <span data-ttu-id="02e25-122">Описание</span><span class="sxs-lookup"><span data-stu-id="02e25-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="02e25-123">period</span><span class="sxs-lookup"><span data-stu-id="02e25-123">period</span></span>    | <span data-ttu-id="02e25-124">string</span><span class="sxs-lookup"><span data-stu-id="02e25-124">string</span></span> | <span data-ttu-id="02e25-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="02e25-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="02e25-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="02e25-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="02e25-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="02e25-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="02e25-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02e25-128">Required.</span></span> |

<span data-ttu-id="02e25-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="02e25-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="02e25-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="02e25-130">The default output type is text/csv.</span></span> <span data-ttu-id="02e25-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="02e25-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02e25-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02e25-132">Request headers</span></span>

| <span data-ttu-id="02e25-133">Имя</span><span class="sxs-lookup"><span data-stu-id="02e25-133">Name</span></span>          | <span data-ttu-id="02e25-134">Описание</span><span class="sxs-lookup"><span data-stu-id="02e25-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="02e25-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02e25-135">Authorization</span></span> | <span data-ttu-id="02e25-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02e25-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="02e25-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e25-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="02e25-139">CSV</span><span class="sxs-lookup"><span data-stu-id="02e25-139">CSV</span></span>

<span data-ttu-id="02e25-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="02e25-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="02e25-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="02e25-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="02e25-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="02e25-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="02e25-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="02e25-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="02e25-144">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="02e25-144">Report Refresh Date</span></span>
- <span data-ttu-id="02e25-145">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="02e25-145">Mail For Mac</span></span>
- <span data-ttu-id="02e25-146">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="02e25-146">Outlook For Mac</span></span>
- <span data-ttu-id="02e25-147">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="02e25-147">Outlook For Windows</span></span>
- <span data-ttu-id="02e25-148">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="02e25-148">Outlook For Mobile</span></span>
- <span data-ttu-id="02e25-149">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="02e25-149">Other For Mobile</span></span>
- <span data-ttu-id="02e25-150">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="02e25-150">Outlook For Web</span></span>
- <span data-ttu-id="02e25-151">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="02e25-151">POP3 App</span></span>
- <span data-ttu-id="02e25-152">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="02e25-152">IMAP4 App</span></span>
- <span data-ttu-id="02e25-153">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="02e25-153">SMTP App</span></span>
- <span data-ttu-id="02e25-154">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="02e25-154">Report Date</span></span>
- <span data-ttu-id="02e25-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="02e25-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="02e25-156">JSON</span><span class="sxs-lookup"><span data-stu-id="02e25-156">JSON</span></span>

<span data-ttu-id="02e25-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеусеркаунтс](../resources/emailappusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02e25-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e25-158">Пример</span><span class="sxs-lookup"><span data-stu-id="02e25-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="02e25-159">CSV</span><span class="sxs-lookup"><span data-stu-id="02e25-159">CSV</span></span>

<span data-ttu-id="02e25-160">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="02e25-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="02e25-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="02e25-161">Request</span></span>

<span data-ttu-id="02e25-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02e25-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="02e25-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e25-163">Response</span></span>

<span data-ttu-id="02e25-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02e25-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="02e25-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="02e25-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="02e25-166">JSON</span><span class="sxs-lookup"><span data-stu-id="02e25-166">JSON</span></span>

<span data-ttu-id="02e25-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="02e25-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="02e25-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="02e25-168">Request</span></span>

<span data-ttu-id="02e25-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02e25-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="02e25-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e25-170">Response</span></span>

<span data-ttu-id="02e25-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02e25-171">The following is an example of the response.</span></span>

> <span data-ttu-id="02e25-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02e25-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
