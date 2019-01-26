---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 64b0c6dfec05f21c492c5e7898ee23792f1136fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573440"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="05eef-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="05eef-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05eef-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="05eef-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="05eef-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="05eef-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="05eef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05eef-106">Permissions</span></span>

<span data-ttu-id="05eef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05eef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05eef-109">Permission type</span></span>                        | <span data-ttu-id="05eef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05eef-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="05eef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05eef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05eef-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05eef-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="05eef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05eef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05eef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05eef-114">Not supported.</span></span>                           |
| <span data-ttu-id="05eef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05eef-115">Application</span></span>                            | <span data-ttu-id="05eef-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05eef-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="05eef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05eef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="05eef-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="05eef-118">Function parameters</span></span>

<span data-ttu-id="05eef-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="05eef-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="05eef-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="05eef-120">Parameter</span></span> | <span data-ttu-id="05eef-121">Тип</span><span class="sxs-lookup"><span data-stu-id="05eef-121">Type</span></span>   | <span data-ttu-id="05eef-122">Описание</span><span class="sxs-lookup"><span data-stu-id="05eef-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="05eef-123">period</span><span class="sxs-lookup"><span data-stu-id="05eef-123">period</span></span>    | <span data-ttu-id="05eef-124">строка</span><span class="sxs-lookup"><span data-stu-id="05eef-124">string</span></span> | <span data-ttu-id="05eef-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="05eef-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="05eef-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="05eef-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="05eef-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="05eef-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="05eef-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05eef-128">Required.</span></span> |

<span data-ttu-id="05eef-129">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05eef-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="05eef-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="05eef-130">The default output type is text/csv.</span></span> <span data-ttu-id="05eef-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="05eef-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05eef-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05eef-132">Request headers</span></span>

| <span data-ttu-id="05eef-133">Имя</span><span class="sxs-lookup"><span data-stu-id="05eef-133">Name</span></span>          | <span data-ttu-id="05eef-134">Описание</span><span class="sxs-lookup"><span data-stu-id="05eef-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="05eef-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05eef-135">Authorization</span></span> | <span data-ttu-id="05eef-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05eef-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="05eef-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="05eef-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="05eef-139">CSV</span><span class="sxs-lookup"><span data-stu-id="05eef-139">CSV</span></span>

<span data-ttu-id="05eef-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="05eef-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="05eef-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="05eef-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="05eef-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="05eef-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="05eef-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="05eef-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="05eef-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="05eef-144">Report Refresh Date</span></span>
- <span data-ttu-id="05eef-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="05eef-145">User Principal Name</span></span>
- <span data-ttu-id="05eef-146">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="05eef-146">Display Name</span></span>
- <span data-ttu-id="05eef-147">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="05eef-147">Is Deleted</span></span>
- <span data-ttu-id="05eef-148">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="05eef-148">Deleted Date</span></span>
- <span data-ttu-id="05eef-149">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="05eef-149">Created Date</span></span>
- <span data-ttu-id="05eef-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="05eef-150">Last Activity Date</span></span>
- <span data-ttu-id="05eef-151">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="05eef-151">Item Count</span></span>
- <span data-ttu-id="05eef-152">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="05eef-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="05eef-153">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="05eef-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="05eef-154">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="05eef-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="05eef-155">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="05eef-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="05eef-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="05eef-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="05eef-157">JSON</span><span class="sxs-lookup"><span data-stu-id="05eef-157">JSON</span></span>

<span data-ttu-id="05eef-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="05eef-158">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="05eef-159">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="05eef-159">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="05eef-160">Пример</span><span class="sxs-lookup"><span data-stu-id="05eef-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="05eef-161">CSV</span><span class="sxs-lookup"><span data-stu-id="05eef-161">CSV</span></span>

<span data-ttu-id="05eef-162">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="05eef-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="05eef-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="05eef-163">Request</span></span>

<span data-ttu-id="05eef-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05eef-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="05eef-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="05eef-165">Response</span></span>

<span data-ttu-id="05eef-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05eef-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="05eef-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="05eef-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="05eef-168">JSON</span><span class="sxs-lookup"><span data-stu-id="05eef-168">JSON</span></span>

<span data-ttu-id="05eef-169">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="05eef-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="05eef-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="05eef-170">Request</span></span>

<span data-ttu-id="05eef-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05eef-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="05eef-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="05eef-172">Response</span></span>

<span data-ttu-id="05eef-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05eef-173">The following is an example of the response.</span></span>

> <span data-ttu-id="05eef-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05eef-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "createdDate": "2016-03-30", 
      "lastActivityDate": "2017-09-01", 
      "itemCount": 138481, 
      "storageUsedInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getmailboxusagedetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
