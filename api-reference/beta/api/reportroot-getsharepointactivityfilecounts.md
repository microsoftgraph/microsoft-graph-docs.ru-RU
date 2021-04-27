---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: e737189ab394ebea93807a4a69f064506e2a158f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049109"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="68e4d-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="68e4d-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="68e4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e4d-105">Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint.</span><span class="sxs-lookup"><span data-stu-id="68e4d-105">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="68e4d-106">**Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — SharePoint действий.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="68e4d-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="68e4d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68e4d-107">Permissions</span></span>

<span data-ttu-id="68e4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68e4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68e4d-110">Permission type</span></span>                        | <span data-ttu-id="68e4d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68e4d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="68e4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68e4d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="68e4d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="68e4d-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="68e4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68e4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e4d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e4d-115">Not supported.</span></span>                           |
| <span data-ttu-id="68e4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68e4d-116">Application</span></span>                            | <span data-ttu-id="68e4d-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="68e4d-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="68e4d-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68e4d-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="68e4d-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="68e4d-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="68e4d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68e4d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="68e4d-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="68e4d-121">Function parameters</span></span>

<span data-ttu-id="68e4d-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="68e4d-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="68e4d-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="68e4d-123">Parameter</span></span> | <span data-ttu-id="68e4d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="68e4d-124">Type</span></span>   | <span data-ttu-id="68e4d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="68e4d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="68e4d-126">period</span><span class="sxs-lookup"><span data-stu-id="68e4d-126">period</span></span>    | <span data-ttu-id="68e4d-127">string</span><span class="sxs-lookup"><span data-stu-id="68e4d-127">string</span></span> | <span data-ttu-id="68e4d-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="68e4d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="68e4d-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="68e4d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="68e4d-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="68e4d-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="68e4d-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68e4d-131">Required.</span></span> |

<span data-ttu-id="68e4d-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="68e4d-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="68e4d-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="68e4d-133">The default output type is text/csv.</span></span> <span data-ttu-id="68e4d-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="68e4d-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68e4d-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68e4d-135">Request headers</span></span>

| <span data-ttu-id="68e4d-136">Имя</span><span class="sxs-lookup"><span data-stu-id="68e4d-136">Name</span></span>          | <span data-ttu-id="68e4d-137">Описание</span><span class="sxs-lookup"><span data-stu-id="68e4d-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="68e4d-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68e4d-138">Authorization</span></span> | <span data-ttu-id="68e4d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68e4d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="68e4d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e4d-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="68e4d-142">CSV</span><span class="sxs-lookup"><span data-stu-id="68e4d-142">CSV</span></span>

<span data-ttu-id="68e4d-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="68e4d-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="68e4d-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="68e4d-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="68e4d-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="68e4d-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="68e4d-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="68e4d-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="68e4d-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="68e4d-147">Report Refresh Date</span></span>
- <span data-ttu-id="68e4d-148">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="68e4d-148">Viewed Or Edited</span></span>
- <span data-ttu-id="68e4d-149">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="68e4d-149">Synced</span></span>
- <span data-ttu-id="68e4d-150">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="68e4d-150">Shared Internally</span></span>
- <span data-ttu-id="68e4d-151">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="68e4d-151">Shared Externally</span></span>
- <span data-ttu-id="68e4d-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="68e4d-152">Report Date</span></span>
- <span data-ttu-id="68e4d-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="68e4d-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="68e4d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="68e4d-154">JSON</span></span>

<span data-ttu-id="68e4d-155">В случае успешной работы этот метод возвращает код ответа и `200 OK` **[объект siteActivitySummary](../resources/siteactivitysummary.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68e4d-155">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68e4d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="68e4d-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="68e4d-157">CSV</span><span class="sxs-lookup"><span data-stu-id="68e4d-157">CSV</span></span>

<span data-ttu-id="68e4d-158">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="68e4d-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="68e4d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="68e4d-159">Request</span></span>

<span data-ttu-id="68e4d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68e4d-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="68e4d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e4d-161">Response</span></span>

<span data-ttu-id="68e4d-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68e4d-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="68e4d-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="68e4d-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="68e4d-164">JSON</span><span class="sxs-lookup"><span data-stu-id="68e4d-164">JSON</span></span>

<span data-ttu-id="68e4d-165">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="68e4d-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="68e4d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="68e4d-166">Request</span></span>

<span data-ttu-id="68e4d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68e4d-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="68e4d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e4d-168">Response</span></span>

<span data-ttu-id="68e4d-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="68e4d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="68e4d-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68e4d-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
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


