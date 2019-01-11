---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.openlocfilehash: c1b15824ab5313d1c581509936a84f5af2daee84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856289"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="e9296-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="e9296-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

> <span data-ttu-id="e9296-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9296-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9296-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9296-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9296-107">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e9296-107">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="e9296-108">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="e9296-108">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="e9296-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="e9296-109">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9296-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9296-110">Permissions</span></span>

<span data-ttu-id="e9296-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9296-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9296-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9296-113">Permission type</span></span>                        | <span data-ttu-id="e9296-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9296-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e9296-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9296-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9296-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9296-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e9296-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9296-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9296-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9296-118">Not supported.</span></span>                           |
| <span data-ttu-id="e9296-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9296-119">Application</span></span>                            | <span data-ttu-id="e9296-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9296-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e9296-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9296-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e9296-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="e9296-122">Function parameters</span></span>

<span data-ttu-id="e9296-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e9296-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e9296-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="e9296-124">Parameter</span></span> | <span data-ttu-id="e9296-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e9296-125">Type</span></span>   | <span data-ttu-id="e9296-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e9296-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e9296-127">period</span><span class="sxs-lookup"><span data-stu-id="e9296-127">period</span></span>    | <span data-ttu-id="e9296-128">строка</span><span class="sxs-lookup"><span data-stu-id="e9296-128">string</span></span> | <span data-ttu-id="e9296-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e9296-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e9296-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e9296-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e9296-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e9296-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e9296-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9296-132">Required.</span></span> |

<span data-ttu-id="e9296-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9296-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e9296-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="e9296-134">The default output type is text/csv.</span></span> <span data-ttu-id="e9296-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="e9296-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9296-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9296-136">Request headers</span></span>

| <span data-ttu-id="e9296-137">Имя</span><span class="sxs-lookup"><span data-stu-id="e9296-137">Name</span></span>          | <span data-ttu-id="e9296-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e9296-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e9296-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9296-139">Authorization</span></span> | <span data-ttu-id="e9296-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9296-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e9296-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9296-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e9296-143">CSV</span><span class="sxs-lookup"><span data-stu-id="e9296-143">CSV</span></span>

<span data-ttu-id="e9296-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e9296-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e9296-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e9296-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e9296-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e9296-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e9296-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e9296-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e9296-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e9296-148">Report Refresh Date</span></span>
- <span data-ttu-id="e9296-149">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="e9296-149">Total</span></span>
- <span data-ttu-id="e9296-150">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="e9296-150">Active</span></span>
- <span data-ttu-id="e9296-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e9296-151">Report Date</span></span>
- <span data-ttu-id="e9296-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="e9296-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e9296-153">JSON</span><span class="sxs-lookup"><span data-stu-id="e9296-153">JSON</span></span>

<span data-ttu-id="e9296-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9296-154">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9296-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e9296-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e9296-156">CSV</span><span class="sxs-lookup"><span data-stu-id="e9296-156">CSV</span></span>

<span data-ttu-id="e9296-157">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="e9296-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e9296-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9296-158">Request</span></span>

<span data-ttu-id="e9296-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9296-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e9296-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9296-160">Response</span></span>

<span data-ttu-id="e9296-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9296-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e9296-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e9296-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e9296-163">JSON</span><span class="sxs-lookup"><span data-stu-id="e9296-163">JSON</span></span>

<span data-ttu-id="e9296-164">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="e9296-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e9296-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9296-165">Request</span></span>

<span data-ttu-id="e9296-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9296-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e9296-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9296-167">Response</span></span>

<span data-ttu-id="e9296-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9296-168">The following is an example of the response.</span></span>

> <span data-ttu-id="e9296-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9296-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
