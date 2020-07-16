---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 44d8b81da9c8f8c758c45eba9fea360e65b6f917
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896373"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="3f6bd-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="3f6bd-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="3f6bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f6bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f6bd-105">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="3f6bd-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Mailbox Reporting](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="3f6bd-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f6bd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f6bd-107">Permissions</span></span>

<span data-ttu-id="3f6bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f6bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f6bd-110">Permission type</span></span>                        | <span data-ttu-id="3f6bd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3f6bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f6bd-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f6bd-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3f6bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f6bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-115">Not supported.</span></span>                           |
| <span data-ttu-id="3f6bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f6bd-116">Application</span></span>                            | <span data-ttu-id="3f6bd-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f6bd-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3f6bd-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3f6bd-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3f6bd-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3f6bd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f6bd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3f6bd-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3f6bd-121">Function parameters</span></span>

<span data-ttu-id="3f6bd-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3f6bd-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3f6bd-123">Parameter</span></span> | <span data-ttu-id="3f6bd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3f6bd-124">Type</span></span>   | <span data-ttu-id="3f6bd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3f6bd-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3f6bd-126">period</span><span class="sxs-lookup"><span data-stu-id="3f6bd-126">period</span></span>    | <span data-ttu-id="3f6bd-127">string</span><span class="sxs-lookup"><span data-stu-id="3f6bd-127">string</span></span> | <span data-ttu-id="3f6bd-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3f6bd-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3f6bd-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3f6bd-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-131">Required.</span></span> |

<span data-ttu-id="3f6bd-132">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-132">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3f6bd-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-133">The default output type is text/csv.</span></span> <span data-ttu-id="3f6bd-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f6bd-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f6bd-135">Request headers</span></span>

| <span data-ttu-id="3f6bd-136">Имя</span><span class="sxs-lookup"><span data-stu-id="3f6bd-136">Name</span></span>          | <span data-ttu-id="3f6bd-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3f6bd-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3f6bd-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f6bd-138">Authorization</span></span> | <span data-ttu-id="3f6bd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3f6bd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f6bd-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3f6bd-142">CSV</span><span class="sxs-lookup"><span data-stu-id="3f6bd-142">CSV</span></span>

<span data-ttu-id="3f6bd-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3f6bd-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3f6bd-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3f6bd-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3f6bd-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3f6bd-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3f6bd-147">Report Refresh Date</span></span>
- <span data-ttu-id="3f6bd-148">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="3f6bd-148">User Principal Name</span></span>
- <span data-ttu-id="3f6bd-149">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="3f6bd-149">Display Name</span></span>
- <span data-ttu-id="3f6bd-150">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="3f6bd-150">Is Deleted</span></span>
- <span data-ttu-id="3f6bd-151">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-151">Deleted Date</span></span>
- <span data-ttu-id="3f6bd-152">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-152">Created Date</span></span>
- <span data-ttu-id="3f6bd-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-153">Last Activity Date</span></span>
- <span data-ttu-id="3f6bd-154">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-154">Item Count</span></span>
- <span data-ttu-id="3f6bd-155">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="3f6bd-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="3f6bd-156">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="3f6bd-156">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="3f6bd-157">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="3f6bd-157">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="3f6bd-158">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="3f6bd-158">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="3f6bd-159">Deleted Item Count (количество удаленных элементов)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-159">Deleted Item Count</span></span>
- <span data-ttu-id="3f6bd-160">Deleted Item Size (Byte) [размер удаленных элементов (байт)]</span><span class="sxs-lookup"><span data-stu-id="3f6bd-160">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="3f6bd-161">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3f6bd-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3f6bd-162">JSON</span><span class="sxs-lookup"><span data-stu-id="3f6bd-162">JSON</span></span>

<span data-ttu-id="3f6bd-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажедетаил](../resources/mailboxusagedetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-163">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="3f6bd-164">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3f6bd-165">Пример</span><span class="sxs-lookup"><span data-stu-id="3f6bd-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3f6bd-166">CSV</span><span class="sxs-lookup"><span data-stu-id="3f6bd-166">CSV</span></span>

<span data-ttu-id="3f6bd-167">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3f6bd-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f6bd-168">Request</span></span>

<span data-ttu-id="3f6bd-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="3f6bd-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f6bd-170">Response</span></span>

<span data-ttu-id="3f6bd-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3f6bd-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="3f6bd-173">JSON</span><span class="sxs-lookup"><span data-stu-id="3f6bd-173">JSON</span></span>

<span data-ttu-id="3f6bd-174">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3f6bd-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f6bd-175">Request</span></span>

<span data-ttu-id="3f6bd-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="3f6bd-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f6bd-177">Response</span></span>

<span data-ttu-id="3f6bd-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-178">The following is an example of the response.</span></span>

> <span data-ttu-id="3f6bd-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f6bd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "deletedItemCount": 138481,
      "deletedItemSizeInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
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
