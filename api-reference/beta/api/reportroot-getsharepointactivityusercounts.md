---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: fba30f63decabb7b64c013321847c926eb0069de
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983281"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="3b337-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="3b337-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="3b337-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b337-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b337-106">Получение сведений о том, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3b337-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="3b337-107">Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="3b337-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="3b337-108">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : действия в SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="3b337-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b337-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b337-109">Permissions</span></span>

<span data-ttu-id="3b337-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b337-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b337-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b337-112">Permission type</span></span>                        | <span data-ttu-id="3b337-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b337-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3b337-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b337-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b337-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b337-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3b337-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b337-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b337-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b337-117">Not supported.</span></span>                           |
| <span data-ttu-id="3b337-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b337-118">Application</span></span>                            | <span data-ttu-id="3b337-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b337-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="3b337-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b337-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3b337-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3b337-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3b337-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b337-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3b337-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3b337-123">Function parameters</span></span>

<span data-ttu-id="3b337-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3b337-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3b337-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="3b337-125">Parameter</span></span> | <span data-ttu-id="3b337-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3b337-126">Type</span></span>   | <span data-ttu-id="3b337-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3b337-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3b337-128">period</span><span class="sxs-lookup"><span data-stu-id="3b337-128">period</span></span>    | <span data-ttu-id="3b337-129">string</span><span class="sxs-lookup"><span data-stu-id="3b337-129">string</span></span> | <span data-ttu-id="3b337-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3b337-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3b337-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3b337-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3b337-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3b337-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3b337-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b337-133">Required.</span></span> |

<span data-ttu-id="3b337-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3b337-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3b337-135">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="3b337-135">The default output type is text/csv.</span></span> <span data-ttu-id="3b337-136">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="3b337-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b337-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b337-137">Request headers</span></span>

| <span data-ttu-id="3b337-138">Имя</span><span class="sxs-lookup"><span data-stu-id="3b337-138">Name</span></span>          | <span data-ttu-id="3b337-139">Описание</span><span class="sxs-lookup"><span data-stu-id="3b337-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3b337-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b337-140">Authorization</span></span> | <span data-ttu-id="3b337-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b337-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3b337-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b337-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3b337-144">CSV</span><span class="sxs-lookup"><span data-stu-id="3b337-144">CSV</span></span>

<span data-ttu-id="3b337-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3b337-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3b337-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3b337-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3b337-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3b337-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3b337-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3b337-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3b337-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3b337-149">Report Refresh Date</span></span>
- <span data-ttu-id="3b337-150">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="3b337-150">Visited Page</span></span>
- <span data-ttu-id="3b337-151">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="3b337-151">Viewed Or Edited</span></span>
- <span data-ttu-id="3b337-152">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="3b337-152">Synced</span></span>
- <span data-ttu-id="3b337-153">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3b337-153">Shared Internally</span></span>
- <span data-ttu-id="3b337-154">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3b337-154">Shared Externally</span></span>
- <span data-ttu-id="3b337-155">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3b337-155">Report Date</span></span>
- <span data-ttu-id="3b337-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3b337-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3b337-157">JSON</span><span class="sxs-lookup"><span data-stu-id="3b337-157">JSON</span></span>

<span data-ttu-id="3b337-158">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b337-158">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b337-159">Пример</span><span class="sxs-lookup"><span data-stu-id="3b337-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3b337-160">CSV</span><span class="sxs-lookup"><span data-stu-id="3b337-160">CSV</span></span>

<span data-ttu-id="3b337-161">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="3b337-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3b337-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b337-162">Request</span></span>

<span data-ttu-id="3b337-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b337-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="3b337-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b337-164">Response</span></span>

<span data-ttu-id="3b337-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b337-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3b337-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3b337-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="3b337-167">JSON</span><span class="sxs-lookup"><span data-stu-id="3b337-167">JSON</span></span>

<span data-ttu-id="3b337-168">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3b337-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3b337-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b337-169">Request</span></span>

<span data-ttu-id="3b337-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b337-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="3b337-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b337-171">Response</span></span>

<span data-ttu-id="3b337-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b337-172">The following is an example of the response.</span></span>

> <span data-ttu-id="3b337-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b337-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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


