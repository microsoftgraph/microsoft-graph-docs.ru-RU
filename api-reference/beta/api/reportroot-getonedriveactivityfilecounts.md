---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 26511642969211a41be0555a520e9358a68812b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454334"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="23b56-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="23b56-103">reportRoot: getOneDriveActivityFileCounts</span></span>

<span data-ttu-id="23b56-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="23b56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b56-105">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="23b56-105">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="23b56-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="23b56-106">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="23b56-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23b56-107">Permissions</span></span>

<span data-ttu-id="23b56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23b56-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23b56-110">Permission type</span></span>                        | <span data-ttu-id="23b56-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23b56-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23b56-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23b56-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="23b56-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b56-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23b56-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23b56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b56-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b56-115">Not supported.</span></span>                           |
| <span data-ttu-id="23b56-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23b56-116">Application</span></span>                            | <span data-ttu-id="23b56-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b56-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="23b56-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23b56-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="23b56-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="23b56-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="23b56-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23b56-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="23b56-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="23b56-121">Function parameters</span></span>

<span data-ttu-id="23b56-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="23b56-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="23b56-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="23b56-123">Parameter</span></span> | <span data-ttu-id="23b56-124">Тип</span><span class="sxs-lookup"><span data-stu-id="23b56-124">Type</span></span>   | <span data-ttu-id="23b56-125">Описание</span><span class="sxs-lookup"><span data-stu-id="23b56-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23b56-126">period</span><span class="sxs-lookup"><span data-stu-id="23b56-126">period</span></span>    | <span data-ttu-id="23b56-127">string</span><span class="sxs-lookup"><span data-stu-id="23b56-127">string</span></span> | <span data-ttu-id="23b56-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23b56-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23b56-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="23b56-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23b56-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="23b56-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="23b56-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23b56-131">Required.</span></span> |

<span data-ttu-id="23b56-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="23b56-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="23b56-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="23b56-133">The default output type is text/csv.</span></span> <span data-ttu-id="23b56-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="23b56-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23b56-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23b56-135">Request headers</span></span>

| <span data-ttu-id="23b56-136">Имя</span><span class="sxs-lookup"><span data-stu-id="23b56-136">Name</span></span>          | <span data-ttu-id="23b56-137">Описание</span><span class="sxs-lookup"><span data-stu-id="23b56-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23b56-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23b56-138">Authorization</span></span> | <span data-ttu-id="23b56-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23b56-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23b56-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b56-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="23b56-142">CSV</span><span class="sxs-lookup"><span data-stu-id="23b56-142">CSV</span></span>

<span data-ttu-id="23b56-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="23b56-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23b56-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="23b56-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23b56-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="23b56-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23b56-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="23b56-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="23b56-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="23b56-147">Report Refresh Date</span></span>
- <span data-ttu-id="23b56-148">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="23b56-148">Viewed Or Edited</span></span>
- <span data-ttu-id="23b56-149">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="23b56-149">Synced</span></span>
- <span data-ttu-id="23b56-150">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="23b56-150">Shared Internally</span></span>
- <span data-ttu-id="23b56-151">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="23b56-151">Shared Externally</span></span>
- <span data-ttu-id="23b56-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="23b56-152">Report Date</span></span>
- <span data-ttu-id="23b56-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="23b56-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="23b56-154">JSON</span><span class="sxs-lookup"><span data-stu-id="23b56-154">JSON</span></span>

<span data-ttu-id="23b56-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[ситеактивитисуммари](../resources/siteactivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23b56-155">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b56-156">Пример</span><span class="sxs-lookup"><span data-stu-id="23b56-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="23b56-157">CSV</span><span class="sxs-lookup"><span data-stu-id="23b56-157">CSV</span></span>

<span data-ttu-id="23b56-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="23b56-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="23b56-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b56-159">Request</span></span>

<span data-ttu-id="23b56-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b56-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b56-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b56-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="23b56-162">C#</span><span class="sxs-lookup"><span data-stu-id="23b56-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityfilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b56-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b56-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityfilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b56-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b56-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityfilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b56-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b56-165">Response</span></span>

<span data-ttu-id="23b56-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b56-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="23b56-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="23b56-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="23b56-168">JSON</span><span class="sxs-lookup"><span data-stu-id="23b56-168">JSON</span></span>

<span data-ttu-id="23b56-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="23b56-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="23b56-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b56-170">Request</span></span>

<span data-ttu-id="23b56-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b56-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23b56-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="23b56-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="23b56-173">C#</span><span class="sxs-lookup"><span data-stu-id="23b56-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityfilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23b56-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b56-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityfilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23b56-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b56-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityfilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23b56-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b56-176">Response</span></span>

<span data-ttu-id="23b56-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b56-177">The following is an example of the response.</span></span>

> <span data-ttu-id="23b56-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23b56-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
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
