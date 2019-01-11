---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Normal
ms.openlocfilehash: 09fbb0ce1a4c652d4e24194b36edd790b1ec63f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865158"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="c0eb3-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="c0eb3-103">reportRoot: getMailboxUsageDetail</span></span>

> <span data-ttu-id="c0eb3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0eb3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0eb3-106">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-106">Get details about mailbox usage.</span></span>

> <span data-ttu-id="c0eb3-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="c0eb3-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0eb3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0eb3-108">Permissions</span></span>

<span data-ttu-id="c0eb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0eb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0eb3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0eb3-111">Permission type</span></span>                        | <span data-ttu-id="c0eb3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c0eb3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0eb3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0eb3-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c0eb3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0eb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-116">Not supported.</span></span>                           |
| <span data-ttu-id="c0eb3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0eb3-117">Application</span></span>                            | <span data-ttu-id="c0eb3-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0eb3-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c0eb3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0eb3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c0eb3-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="c0eb3-120">Function parameters</span></span>

<span data-ttu-id="c0eb3-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c0eb3-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="c0eb3-122">Parameter</span></span> | <span data-ttu-id="c0eb3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c0eb3-123">Type</span></span>   | <span data-ttu-id="c0eb3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c0eb3-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c0eb3-125">period</span><span class="sxs-lookup"><span data-stu-id="c0eb3-125">period</span></span>    | <span data-ttu-id="c0eb3-126">строка</span><span class="sxs-lookup"><span data-stu-id="c0eb3-126">string</span></span> | <span data-ttu-id="c0eb3-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c0eb3-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c0eb3-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c0eb3-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-130">Required.</span></span> |

<span data-ttu-id="c0eb3-131">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-131">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c0eb3-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-132">The default output type is text/csv.</span></span> <span data-ttu-id="c0eb3-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0eb3-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0eb3-134">Request headers</span></span>

| <span data-ttu-id="c0eb3-135">Имя</span><span class="sxs-lookup"><span data-stu-id="c0eb3-135">Name</span></span>          | <span data-ttu-id="c0eb3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c0eb3-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c0eb3-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0eb3-137">Authorization</span></span> | <span data-ttu-id="c0eb3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c0eb3-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0eb3-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c0eb3-141">CSV</span><span class="sxs-lookup"><span data-stu-id="c0eb3-141">CSV</span></span>

<span data-ttu-id="c0eb3-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c0eb3-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c0eb3-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c0eb3-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c0eb3-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c0eb3-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c0eb3-146">Report Refresh Date</span></span>
- <span data-ttu-id="c0eb3-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c0eb3-147">User Principal Name</span></span>
- <span data-ttu-id="c0eb3-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="c0eb3-148">Display Name</span></span>
- <span data-ttu-id="c0eb3-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="c0eb3-149">Is Deleted</span></span>
- <span data-ttu-id="c0eb3-150">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-150">Deleted Date</span></span>
- <span data-ttu-id="c0eb3-151">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-151">Created Date</span></span>
- <span data-ttu-id="c0eb3-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-152">Last Activity Date</span></span>
- <span data-ttu-id="c0eb3-153">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-153">Item Count</span></span>
- <span data-ttu-id="c0eb3-154">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="c0eb3-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="c0eb3-155">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="c0eb3-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="c0eb3-156">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="c0eb3-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="c0eb3-157">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="c0eb3-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="c0eb3-158">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="c0eb3-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c0eb3-159">JSON</span><span class="sxs-lookup"><span data-stu-id="c0eb3-159">JSON</span></span>

<span data-ttu-id="c0eb3-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="c0eb3-161">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c0eb3-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c0eb3-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c0eb3-163">CSV</span><span class="sxs-lookup"><span data-stu-id="c0eb3-163">CSV</span></span>

<span data-ttu-id="c0eb3-164">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c0eb3-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0eb3-165">Request</span></span>

<span data-ttu-id="c0eb3-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c0eb3-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0eb3-167">Response</span></span>

<span data-ttu-id="c0eb3-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c0eb3-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c0eb3-170">JSON</span><span class="sxs-lookup"><span data-stu-id="c0eb3-170">JSON</span></span>

<span data-ttu-id="c0eb3-171">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c0eb3-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0eb3-172">Request</span></span>

<span data-ttu-id="c0eb3-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c0eb3-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0eb3-174">Response</span></span>

<span data-ttu-id="c0eb3-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-175">The following is an example of the response.</span></span>

> <span data-ttu-id="c0eb3-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0eb3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
