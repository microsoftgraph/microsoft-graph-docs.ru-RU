---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: de6e6966df4741c82a97e28eac4c2cd82b678555
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331706"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="da928-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="da928-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da928-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="da928-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="da928-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="da928-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="da928-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da928-106">Permissions</span></span>

<span data-ttu-id="da928-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da928-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da928-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da928-109">Permission type</span></span>                        | <span data-ttu-id="da928-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da928-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="da928-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da928-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da928-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da928-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="da928-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da928-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da928-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da928-114">Not supported.</span></span>                           |
| <span data-ttu-id="da928-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da928-115">Application</span></span>                            | <span data-ttu-id="da928-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da928-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="da928-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da928-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="da928-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="da928-118">Function parameters</span></span>

<span data-ttu-id="da928-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="da928-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="da928-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="da928-120">Parameter</span></span> | <span data-ttu-id="da928-121">Тип</span><span class="sxs-lookup"><span data-stu-id="da928-121">Type</span></span>   | <span data-ttu-id="da928-122">Описание</span><span class="sxs-lookup"><span data-stu-id="da928-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="da928-123">period</span><span class="sxs-lookup"><span data-stu-id="da928-123">period</span></span>    | <span data-ttu-id="da928-124">string</span><span class="sxs-lookup"><span data-stu-id="da928-124">string</span></span> | <span data-ttu-id="da928-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="da928-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="da928-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="da928-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="da928-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="da928-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="da928-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da928-128">Required.</span></span> |

<span data-ttu-id="da928-129">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da928-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="da928-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="da928-130">The default output type is text/csv.</span></span> <span data-ttu-id="da928-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="da928-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da928-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da928-132">Request headers</span></span>

| <span data-ttu-id="da928-133">Имя</span><span class="sxs-lookup"><span data-stu-id="da928-133">Name</span></span>          | <span data-ttu-id="da928-134">Описание</span><span class="sxs-lookup"><span data-stu-id="da928-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="da928-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da928-135">Authorization</span></span> | <span data-ttu-id="da928-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da928-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="da928-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da928-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="da928-139">CSV</span><span class="sxs-lookup"><span data-stu-id="da928-139">CSV</span></span>

<span data-ttu-id="da928-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="da928-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="da928-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="da928-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="da928-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="da928-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="da928-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="da928-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="da928-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="da928-144">Report Refresh Date</span></span>
- <span data-ttu-id="da928-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="da928-145">User Principal Name</span></span>
- <span data-ttu-id="da928-146">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="da928-146">Display Name</span></span>
- <span data-ttu-id="da928-147">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="da928-147">Is Deleted</span></span>
- <span data-ttu-id="da928-148">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="da928-148">Deleted Date</span></span>
- <span data-ttu-id="da928-149">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="da928-149">Created Date</span></span>
- <span data-ttu-id="da928-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="da928-150">Last Activity Date</span></span>
- <span data-ttu-id="da928-151">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="da928-151">Item Count</span></span>
- <span data-ttu-id="da928-152">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="da928-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="da928-153">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="da928-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="da928-154">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="da928-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="da928-155">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="da928-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="da928-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="da928-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="da928-157">JSON</span><span class="sxs-lookup"><span data-stu-id="da928-157">JSON</span></span>

<span data-ttu-id="da928-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажедетаил](../resources/mailboxusagedetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da928-158">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="da928-159">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="da928-159">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="da928-160">Пример</span><span class="sxs-lookup"><span data-stu-id="da928-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="da928-161">CSV</span><span class="sxs-lookup"><span data-stu-id="da928-161">CSV</span></span>

<span data-ttu-id="da928-162">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="da928-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="da928-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="da928-163">Request</span></span>

<span data-ttu-id="da928-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da928-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="da928-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="da928-165">Response</span></span>

<span data-ttu-id="da928-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da928-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="da928-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="da928-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="da928-168">JSON</span><span class="sxs-lookup"><span data-stu-id="da928-168">JSON</span></span>

<span data-ttu-id="da928-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="da928-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="da928-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="da928-170">Request</span></span>

<span data-ttu-id="da928-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da928-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="da928-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="da928-172">Response</span></span>

<span data-ttu-id="da928-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da928-173">The following is an example of the response.</span></span>

> <span data-ttu-id="da928-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da928-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
