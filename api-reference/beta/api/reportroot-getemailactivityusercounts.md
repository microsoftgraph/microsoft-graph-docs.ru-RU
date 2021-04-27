---
title: 'reportRoot: getEmailActivityUserCounts'
description: Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 8a3441cb31fb46d64551932a62a83ce38f12dba6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050992"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="374a1-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="374a1-103">reportRoot: getEmailActivityUserCounts</span></span>

<span data-ttu-id="374a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="374a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="374a1-105">Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма.</span><span class="sxs-lookup"><span data-stu-id="374a1-105">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="374a1-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Действия с почтой](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="374a1-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="374a1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="374a1-107">Permissions</span></span>

<span data-ttu-id="374a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="374a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="374a1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="374a1-110">Permission type</span></span>                        | <span data-ttu-id="374a1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="374a1-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="374a1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="374a1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="374a1-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="374a1-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="374a1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="374a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="374a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="374a1-115">Not supported.</span></span>                           |
| <span data-ttu-id="374a1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="374a1-116">Application</span></span>                            | <span data-ttu-id="374a1-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="374a1-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="374a1-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="374a1-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="374a1-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="374a1-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="374a1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="374a1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="374a1-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="374a1-121">Function parameters</span></span>

<span data-ttu-id="374a1-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="374a1-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="374a1-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="374a1-123">Parameter</span></span> | <span data-ttu-id="374a1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="374a1-124">Type</span></span>   | <span data-ttu-id="374a1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="374a1-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="374a1-126">period</span><span class="sxs-lookup"><span data-stu-id="374a1-126">period</span></span>    | <span data-ttu-id="374a1-127">string</span><span class="sxs-lookup"><span data-stu-id="374a1-127">string</span></span> | <span data-ttu-id="374a1-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="374a1-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="374a1-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="374a1-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="374a1-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="374a1-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="374a1-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="374a1-131">Required.</span></span> |

<span data-ttu-id="374a1-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="374a1-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="374a1-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="374a1-133">The default output type is text/csv.</span></span> <span data-ttu-id="374a1-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="374a1-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="374a1-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="374a1-135">Request headers</span></span>

| <span data-ttu-id="374a1-136">Имя</span><span class="sxs-lookup"><span data-stu-id="374a1-136">Name</span></span>          | <span data-ttu-id="374a1-137">Описание</span><span class="sxs-lookup"><span data-stu-id="374a1-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="374a1-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="374a1-138">Authorization</span></span> | <span data-ttu-id="374a1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="374a1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="374a1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="374a1-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="374a1-142">CSV</span><span class="sxs-lookup"><span data-stu-id="374a1-142">CSV</span></span>

<span data-ttu-id="374a1-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="374a1-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="374a1-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="374a1-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="374a1-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="374a1-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="374a1-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="374a1-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="374a1-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="374a1-147">Report Refresh Date</span></span>
- <span data-ttu-id="374a1-148">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="374a1-148">Send</span></span>
- <span data-ttu-id="374a1-149">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="374a1-149">Receive</span></span>
- <span data-ttu-id="374a1-150">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="374a1-150">Read</span></span>
- <span data-ttu-id="374a1-151">Созданная встреча</span><span class="sxs-lookup"><span data-stu-id="374a1-151">Meeting Created</span></span>
- <span data-ttu-id="374a1-152">Взаимодействие в собрании</span><span class="sxs-lookup"><span data-stu-id="374a1-152">Meeting Interacted</span></span>
- <span data-ttu-id="374a1-153">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="374a1-153">Report Date</span></span>
- <span data-ttu-id="374a1-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="374a1-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="374a1-155">JSON</span><span class="sxs-lookup"><span data-stu-id="374a1-155">JSON</span></span>

<span data-ttu-id="374a1-156">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект **[emailActivitySummary](../resources/emailactivitysummary.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="374a1-156">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="374a1-157">Пример</span><span class="sxs-lookup"><span data-stu-id="374a1-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="374a1-158">CSV</span><span class="sxs-lookup"><span data-stu-id="374a1-158">CSV</span></span>

<span data-ttu-id="374a1-159">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="374a1-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="374a1-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="374a1-160">Request</span></span>

<span data-ttu-id="374a1-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="374a1-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="374a1-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="374a1-162">Response</span></span>

<span data-ttu-id="374a1-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="374a1-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="374a1-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="374a1-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="374a1-165">JSON</span><span class="sxs-lookup"><span data-stu-id="374a1-165">JSON</span></span>

<span data-ttu-id="374a1-166">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="374a1-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="374a1-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="374a1-167">Request</span></span>

<span data-ttu-id="374a1-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="374a1-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="374a1-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="374a1-169">Response</span></span>

<span data-ttu-id="374a1-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="374a1-170">The following is an example of the response.</span></span>

> <span data-ttu-id="374a1-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="374a1-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
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


