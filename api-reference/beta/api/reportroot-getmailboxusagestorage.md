---
title: 'reportRoot: getMailboxUsageStorage'
description: Узнайте, сколько места занято в хранилище организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: f2423c13102bd3fdf648765fe59df99aca61cf64
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981643"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="85256-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="85256-103">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="85256-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85256-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85256-105">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="85256-105">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="85256-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — использование почтовых ящиков](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="85256-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="85256-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85256-107">Permissions</span></span>

<span data-ttu-id="85256-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85256-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85256-110">Permission type</span></span>                        | <span data-ttu-id="85256-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85256-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="85256-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85256-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="85256-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="85256-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="85256-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85256-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85256-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85256-115">Not supported.</span></span>                           |
| <span data-ttu-id="85256-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85256-116">Application</span></span>                            | <span data-ttu-id="85256-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="85256-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="85256-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85256-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="85256-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="85256-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="85256-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85256-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="85256-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="85256-121">Function parameters</span></span>

<span data-ttu-id="85256-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="85256-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="85256-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="85256-123">Parameter</span></span> | <span data-ttu-id="85256-124">Тип</span><span class="sxs-lookup"><span data-stu-id="85256-124">Type</span></span>   | <span data-ttu-id="85256-125">Описание</span><span class="sxs-lookup"><span data-stu-id="85256-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="85256-126">period</span><span class="sxs-lookup"><span data-stu-id="85256-126">period</span></span>    | <span data-ttu-id="85256-127">string</span><span class="sxs-lookup"><span data-stu-id="85256-127">string</span></span> | <span data-ttu-id="85256-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="85256-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="85256-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="85256-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="85256-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="85256-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="85256-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85256-131">Required.</span></span> |

<span data-ttu-id="85256-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="85256-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="85256-133">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="85256-133">The default output type is text/csv.</span></span> <span data-ttu-id="85256-134">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="85256-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85256-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85256-135">Request headers</span></span>

| <span data-ttu-id="85256-136">Имя</span><span class="sxs-lookup"><span data-stu-id="85256-136">Name</span></span>          | <span data-ttu-id="85256-137">Описание</span><span class="sxs-lookup"><span data-stu-id="85256-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="85256-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85256-138">Authorization</span></span> | <span data-ttu-id="85256-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85256-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="85256-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="85256-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="85256-142">CSV</span><span class="sxs-lookup"><span data-stu-id="85256-142">CSV</span></span>

<span data-ttu-id="85256-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="85256-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="85256-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="85256-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="85256-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="85256-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="85256-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="85256-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="85256-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="85256-147">Report Refresh Date</span></span>
- <span data-ttu-id="85256-148">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="85256-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="85256-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="85256-149">Report Date</span></span>
- <span data-ttu-id="85256-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="85256-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="85256-151">JSON</span><span class="sxs-lookup"><span data-stu-id="85256-151">JSON</span></span>

<span data-ttu-id="85256-152">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85256-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85256-153">Пример</span><span class="sxs-lookup"><span data-stu-id="85256-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="85256-154">CSV</span><span class="sxs-lookup"><span data-stu-id="85256-154">CSV</span></span>

<span data-ttu-id="85256-155">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="85256-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="85256-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="85256-156">Request</span></span>

<span data-ttu-id="85256-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85256-157">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="85256-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="85256-158">Response</span></span>

<span data-ttu-id="85256-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85256-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="85256-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="85256-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="85256-161">JSON</span><span class="sxs-lookup"><span data-stu-id="85256-161">JSON</span></span>

<span data-ttu-id="85256-162">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="85256-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="85256-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="85256-163">Request</span></span>

<span data-ttu-id="85256-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85256-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="85256-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="85256-165">Response</span></span>

<span data-ttu-id="85256-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85256-166">The following is an example of the response.</span></span>

> <span data-ttu-id="85256-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85256-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "storageUsedInBytes": 5159432679270, 
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


