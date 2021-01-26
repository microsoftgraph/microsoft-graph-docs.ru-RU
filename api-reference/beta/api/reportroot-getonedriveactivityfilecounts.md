---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: d72a4a93fcfb9ba12d643e794d47f49239b619c6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983694"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="3e25a-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="3e25a-103">reportRoot: getOneDriveActivityFileCounts</span></span>

<span data-ttu-id="3e25a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e25a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e25a-105">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3e25a-105">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="3e25a-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365: действия в OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)</span><span class="sxs-lookup"><span data-stu-id="3e25a-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e25a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e25a-107">Permissions</span></span>

<span data-ttu-id="3e25a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e25a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e25a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e25a-110">Permission type</span></span>                        | <span data-ttu-id="3e25a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e25a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3e25a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e25a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e25a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e25a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3e25a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e25a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e25a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e25a-115">Not supported.</span></span>                           |
| <span data-ttu-id="3e25a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e25a-116">Application</span></span>                            | <span data-ttu-id="3e25a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e25a-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3e25a-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3e25a-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3e25a-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3e25a-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e25a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e25a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3e25a-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3e25a-121">Function parameters</span></span>

<span data-ttu-id="3e25a-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3e25a-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3e25a-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3e25a-123">Parameter</span></span> | <span data-ttu-id="3e25a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3e25a-124">Type</span></span>   | <span data-ttu-id="3e25a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3e25a-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3e25a-126">period</span><span class="sxs-lookup"><span data-stu-id="3e25a-126">period</span></span>    | <span data-ttu-id="3e25a-127">string</span><span class="sxs-lookup"><span data-stu-id="3e25a-127">string</span></span> | <span data-ttu-id="3e25a-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3e25a-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3e25a-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3e25a-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3e25a-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3e25a-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3e25a-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e25a-131">Required.</span></span> |

<span data-ttu-id="3e25a-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3e25a-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3e25a-133">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="3e25a-133">The default output type is text/csv.</span></span> <span data-ttu-id="3e25a-134">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="3e25a-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e25a-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e25a-135">Request headers</span></span>

| <span data-ttu-id="3e25a-136">Имя</span><span class="sxs-lookup"><span data-stu-id="3e25a-136">Name</span></span>          | <span data-ttu-id="3e25a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3e25a-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3e25a-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e25a-138">Authorization</span></span> | <span data-ttu-id="3e25a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e25a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3e25a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e25a-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3e25a-142">CSV</span><span class="sxs-lookup"><span data-stu-id="3e25a-142">CSV</span></span>

<span data-ttu-id="3e25a-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3e25a-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3e25a-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3e25a-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3e25a-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3e25a-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3e25a-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3e25a-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3e25a-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3e25a-147">Report Refresh Date</span></span>
- <span data-ttu-id="3e25a-148">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="3e25a-148">Viewed Or Edited</span></span>
- <span data-ttu-id="3e25a-149">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="3e25a-149">Synced</span></span>
- <span data-ttu-id="3e25a-150">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3e25a-150">Shared Internally</span></span>
- <span data-ttu-id="3e25a-151">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3e25a-151">Shared Externally</span></span>
- <span data-ttu-id="3e25a-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3e25a-152">Report Date</span></span>
- <span data-ttu-id="3e25a-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3e25a-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3e25a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="3e25a-154">JSON</span></span>

<span data-ttu-id="3e25a-155">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[siteActivitySummary](../resources/siteactivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e25a-155">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e25a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="3e25a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3e25a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="3e25a-157">CSV</span></span>

<span data-ttu-id="3e25a-158">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="3e25a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3e25a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e25a-159">Request</span></span>

<span data-ttu-id="3e25a-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e25a-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="3e25a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e25a-161">Response</span></span>

<span data-ttu-id="3e25a-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e25a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3e25a-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3e25a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3e25a-164">JSON</span><span class="sxs-lookup"><span data-stu-id="3e25a-164">JSON</span></span>

<span data-ttu-id="3e25a-165">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3e25a-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3e25a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e25a-166">Request</span></span>

<span data-ttu-id="3e25a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e25a-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="3e25a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e25a-168">Response</span></span>

<span data-ttu-id="3e25a-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e25a-169">The following is an example of the response.</span></span>

> <span data-ttu-id="3e25a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e25a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


