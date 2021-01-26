---
title: 'reportRoot: getSharePointActivityPages'
description: Узнайте, сколько уникальных страниц посетили пользователи.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: d1a99b4bc0e621b9e1956dd0a7782e42d3c9dffa
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983316"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="714ed-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="714ed-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="714ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="714ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="714ed-105">Получите количество уникальных страниц, посещенных пользователями.</span><span class="sxs-lookup"><span data-stu-id="714ed-105">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="714ed-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : действия в SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="714ed-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="714ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="714ed-107">Permissions</span></span>

<span data-ttu-id="714ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="714ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="714ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="714ed-110">Permission type</span></span>                        | <span data-ttu-id="714ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="714ed-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="714ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="714ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="714ed-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="714ed-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="714ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="714ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="714ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="714ed-115">Not supported.</span></span>                           |
| <span data-ttu-id="714ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="714ed-116">Application</span></span>                            | <span data-ttu-id="714ed-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="714ed-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="714ed-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="714ed-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="714ed-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="714ed-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="714ed-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="714ed-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="714ed-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="714ed-121">Function parameters</span></span>

<span data-ttu-id="714ed-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="714ed-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="714ed-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="714ed-123">Parameter</span></span> | <span data-ttu-id="714ed-124">Тип</span><span class="sxs-lookup"><span data-stu-id="714ed-124">Type</span></span>   | <span data-ttu-id="714ed-125">Описание</span><span class="sxs-lookup"><span data-stu-id="714ed-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="714ed-126">period</span><span class="sxs-lookup"><span data-stu-id="714ed-126">period</span></span>    | <span data-ttu-id="714ed-127">string</span><span class="sxs-lookup"><span data-stu-id="714ed-127">string</span></span> | <span data-ttu-id="714ed-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="714ed-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="714ed-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="714ed-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="714ed-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="714ed-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="714ed-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="714ed-131">Required.</span></span> |

<span data-ttu-id="714ed-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="714ed-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="714ed-133">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="714ed-133">The default output type is text/csv.</span></span> <span data-ttu-id="714ed-134">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="714ed-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="714ed-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="714ed-135">Request headers</span></span>

| <span data-ttu-id="714ed-136">Имя</span><span class="sxs-lookup"><span data-stu-id="714ed-136">Name</span></span>          | <span data-ttu-id="714ed-137">Описание</span><span class="sxs-lookup"><span data-stu-id="714ed-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="714ed-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="714ed-138">Authorization</span></span> | <span data-ttu-id="714ed-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="714ed-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="714ed-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="714ed-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="714ed-142">CSV</span><span class="sxs-lookup"><span data-stu-id="714ed-142">CSV</span></span>

<span data-ttu-id="714ed-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="714ed-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="714ed-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="714ed-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="714ed-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="714ed-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="714ed-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="714ed-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="714ed-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="714ed-147">Report Refresh Date</span></span>
- <span data-ttu-id="714ed-148">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="714ed-148">Visited Page Count</span></span>
- <span data-ttu-id="714ed-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="714ed-149">Report Date</span></span>
- <span data-ttu-id="714ed-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="714ed-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="714ed-151">JSON</span><span class="sxs-lookup"><span data-stu-id="714ed-151">JSON</span></span>

<span data-ttu-id="714ed-152">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[sharePointActivityPages](../resources/sharepointactivitypages.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="714ed-152">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="714ed-153">Пример</span><span class="sxs-lookup"><span data-stu-id="714ed-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="714ed-154">CSV</span><span class="sxs-lookup"><span data-stu-id="714ed-154">CSV</span></span>

<span data-ttu-id="714ed-155">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="714ed-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="714ed-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="714ed-156">Request</span></span>

<span data-ttu-id="714ed-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="714ed-157">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="714ed-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="714ed-158">Response</span></span>

<span data-ttu-id="714ed-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="714ed-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="714ed-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="714ed-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="714ed-161">JSON</span><span class="sxs-lookup"><span data-stu-id="714ed-161">JSON</span></span>

<span data-ttu-id="714ed-162">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="714ed-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="714ed-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="714ed-163">Request</span></span>

<span data-ttu-id="714ed-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="714ed-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="714ed-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="714ed-165">Response</span></span>

<span data-ttu-id="714ed-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="714ed-166">The following is an example of the response.</span></span>

> <span data-ttu-id="714ed-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="714ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
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


