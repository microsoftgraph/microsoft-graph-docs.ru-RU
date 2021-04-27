---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 75c860601fe1572482fc2e128634d77c3ac4b6c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050971"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="bbc4c-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="bbc4c-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="bbc4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbc4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc4c-105">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-105">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="bbc4c-106">**Примечание:** Сведения о различных представлениях отчетов и именах [см. в Microsoft 365 отчетов .](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc4c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbc4c-107">Permissions</span></span>

<span data-ttu-id="bbc4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbc4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbc4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbc4c-110">Permission type</span></span>                        | <span data-ttu-id="bbc4c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bbc4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbc4c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbc4c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bbc4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-115">Not supported.</span></span>                           |
| <span data-ttu-id="bbc4c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbc4c-116">Application</span></span>                            | <span data-ttu-id="bbc4c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbc4c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="bbc4c-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="bbc4c-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="bbc4c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="bbc4c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbc4c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bbc4c-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="bbc4c-121">Function parameters</span></span>

<span data-ttu-id="bbc4c-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bbc4c-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="bbc4c-123">Parameter</span></span> | <span data-ttu-id="bbc4c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bbc4c-124">Type</span></span>   | <span data-ttu-id="bbc4c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bbc4c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bbc4c-126">period</span><span class="sxs-lookup"><span data-stu-id="bbc4c-126">period</span></span>    | <span data-ttu-id="bbc4c-127">string</span><span class="sxs-lookup"><span data-stu-id="bbc4c-127">string</span></span> | <span data-ttu-id="bbc4c-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bbc4c-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bbc4c-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bbc4c-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-131">Required.</span></span> |

<span data-ttu-id="bbc4c-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bbc4c-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-133">The default output type is text/csv.</span></span> <span data-ttu-id="bbc4c-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbc4c-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbc4c-135">Request headers</span></span>

| <span data-ttu-id="bbc4c-136">Имя</span><span class="sxs-lookup"><span data-stu-id="bbc4c-136">Name</span></span>          | <span data-ttu-id="bbc4c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bbc4c-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bbc4c-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbc4c-138">Authorization</span></span> | <span data-ttu-id="bbc4c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bbc4c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbc4c-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bbc4c-142">CSV</span><span class="sxs-lookup"><span data-stu-id="bbc4c-142">CSV</span></span>

<span data-ttu-id="bbc4c-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bbc4c-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bbc4c-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bbc4c-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="bbc4c-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bbc4c-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-147">Report Refresh Date</span></span>
- <span data-ttu-id="bbc4c-148">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-148">Mail For Mac</span></span>
- <span data-ttu-id="bbc4c-149">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-149">Outlook For Mac</span></span>
- <span data-ttu-id="bbc4c-150">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-150">Outlook For Windows</span></span>
- <span data-ttu-id="bbc4c-151">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-151">Outlook For Mobile</span></span>
- <span data-ttu-id="bbc4c-152">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-152">Other For Mobile</span></span>
- <span data-ttu-id="bbc4c-153">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-153">Outlook For Web</span></span>
- <span data-ttu-id="bbc4c-154">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-154">POP3 App</span></span>
- <span data-ttu-id="bbc4c-155">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="bbc4c-155">IMAP4 App</span></span>
- <span data-ttu-id="bbc4c-156">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-156">SMTP App</span></span>
- <span data-ttu-id="bbc4c-157">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-157">Report Date</span></span>
- <span data-ttu-id="bbc4c-158">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="bbc4c-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bbc4c-159">JSON</span><span class="sxs-lookup"><span data-stu-id="bbc4c-159">JSON</span></span>

<span data-ttu-id="bbc4c-160">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-160">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc4c-161">Пример</span><span class="sxs-lookup"><span data-stu-id="bbc4c-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bbc4c-162">CSV</span><span class="sxs-lookup"><span data-stu-id="bbc4c-162">CSV</span></span>

<span data-ttu-id="bbc4c-163">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc4c-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbc4c-164">Request</span></span>

<span data-ttu-id="bbc4c-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="bbc4c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbc4c-166">Response</span></span>

<span data-ttu-id="bbc4c-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bbc4c-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="bbc4c-169">JSON</span><span class="sxs-lookup"><span data-stu-id="bbc4c-169">JSON</span></span>

<span data-ttu-id="bbc4c-170">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc4c-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbc4c-171">Request</span></span>

<span data-ttu-id="bbc4c-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-172">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="bbc4c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbc4c-173">Response</span></span>

<span data-ttu-id="bbc4c-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-174">The following is an example of the response.</span></span>

> <span data-ttu-id="bbc4c-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bbc4c-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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


