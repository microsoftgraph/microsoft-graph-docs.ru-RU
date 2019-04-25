---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2ed01152d4670b0bcb1ebccab1e12302c5bb19fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546127"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="e996e-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="e996e-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e996e-104">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="e996e-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="e996e-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="e996e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e996e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e996e-106">Permissions</span></span>

<span data-ttu-id="e996e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e996e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e996e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e996e-109">Permission type</span></span>                        | <span data-ttu-id="e996e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e996e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e996e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e996e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e996e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e996e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e996e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e996e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e996e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e996e-114">Not supported.</span></span>                           |
| <span data-ttu-id="e996e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e996e-115">Application</span></span>                            | <span data-ttu-id="e996e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e996e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e996e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e996e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e996e-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e996e-118">Function parameters</span></span>

<span data-ttu-id="e996e-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e996e-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e996e-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="e996e-120">Parameter</span></span> | <span data-ttu-id="e996e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e996e-121">Type</span></span>   | <span data-ttu-id="e996e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e996e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e996e-123">period</span><span class="sxs-lookup"><span data-stu-id="e996e-123">period</span></span>    | <span data-ttu-id="e996e-124">string</span><span class="sxs-lookup"><span data-stu-id="e996e-124">string</span></span> | <span data-ttu-id="e996e-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e996e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e996e-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e996e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e996e-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e996e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e996e-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e996e-128">Required.</span></span> |

<span data-ttu-id="e996e-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e996e-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e996e-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="e996e-130">The default output type is text/csv.</span></span> <span data-ttu-id="e996e-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e996e-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e996e-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e996e-132">Request headers</span></span>

| <span data-ttu-id="e996e-133">Имя</span><span class="sxs-lookup"><span data-stu-id="e996e-133">Name</span></span>          | <span data-ttu-id="e996e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e996e-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e996e-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e996e-135">Authorization</span></span> | <span data-ttu-id="e996e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e996e-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e996e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e996e-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e996e-139">CSV</span><span class="sxs-lookup"><span data-stu-id="e996e-139">CSV</span></span>

<span data-ttu-id="e996e-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e996e-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e996e-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e996e-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e996e-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e996e-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e996e-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e996e-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e996e-144">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="e996e-144">Report Refresh Date</span></span>
- <span data-ttu-id="e996e-145">Under Limit (ограничение не превышено)</span><span class="sxs-lookup"><span data-stu-id="e996e-145">Under Limit</span></span>
- <span data-ttu-id="e996e-146">Warning Issued (выведено предупреждение)</span><span class="sxs-lookup"><span data-stu-id="e996e-146">Warning Issued</span></span>
- <span data-ttu-id="e996e-147">Send Prohibited (отправка запрещена)</span><span class="sxs-lookup"><span data-stu-id="e996e-147">Send Prohibited</span></span>
- <span data-ttu-id="e996e-148">Send/Receive Prohibited (отправка и получение запрещены)</span><span class="sxs-lookup"><span data-stu-id="e996e-148">Send/Receive Prohibited</span></span>
- <span data-ttu-id="e996e-149">Indeterminate (не определено)</span><span class="sxs-lookup"><span data-stu-id="e996e-149">Indeterminate</span></span>
- <span data-ttu-id="e996e-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="e996e-150">Report Date</span></span>
- <span data-ttu-id="e996e-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="e996e-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e996e-152">JSON</span><span class="sxs-lookup"><span data-stu-id="e996e-152">JSON</span></span>

<span data-ttu-id="e996e-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажекуотастатусмаилбокскаунтс](../resources/mailboxusagequotastatusmailboxcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e996e-153">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e996e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e996e-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e996e-155">CSV</span><span class="sxs-lookup"><span data-stu-id="e996e-155">CSV</span></span>

<span data-ttu-id="e996e-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="e996e-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e996e-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="e996e-157">Request</span></span>

<span data-ttu-id="e996e-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e996e-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e996e-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e996e-159">Response</span></span>

<span data-ttu-id="e996e-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e996e-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e996e-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e996e-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e996e-162">JSON</span><span class="sxs-lookup"><span data-stu-id="e996e-162">JSON</span></span>

<span data-ttu-id="e996e-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="e996e-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e996e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e996e-164">Request</span></span>

<span data-ttu-id="e996e-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e996e-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e996e-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e996e-166">Response</span></span>

<span data-ttu-id="e996e-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e996e-167">The following is an example of the response.</span></span>

> <span data-ttu-id="e996e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e996e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageQuotaMailboxStatusCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "underLimit": 155, 
      "warningIssued": 0, 
      "sendProhibited": 0, 
      "sendReceiveProhibited": 0, 
      "indeterminate": 14, 
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
    "Error: /api-reference/beta/api/reportroot-getmailboxusagequotastatusmailboxcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
