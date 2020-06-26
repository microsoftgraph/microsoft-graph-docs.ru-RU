---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2dec3f6ea849c3536f7bd976b963cf082a2ce5ff
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896758"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="c9d99-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="c9d99-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="c9d99-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d99-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d99-106">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c9d99-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="c9d99-107">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="c9d99-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="c9d99-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="c9d99-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9d99-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9d99-109">Permissions</span></span>

<span data-ttu-id="c9d99-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c9d99-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c9d99-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d99-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9d99-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9d99-112">Permission type</span></span>                        | <span data-ttu-id="c9d99-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9d99-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c9d99-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9d99-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9d99-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9d99-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c9d99-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9d99-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9d99-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9d99-117">Not supported.</span></span>                           |
| <span data-ttu-id="c9d99-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9d99-118">Application</span></span>                            | <span data-ttu-id="c9d99-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9d99-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="c9d99-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c9d99-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c9d99-121">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c9d99-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c9d99-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9d99-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c9d99-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c9d99-123">Function parameters</span></span>

<span data-ttu-id="c9d99-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c9d99-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c9d99-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9d99-125">Parameter</span></span> | <span data-ttu-id="c9d99-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c9d99-126">Type</span></span>   | <span data-ttu-id="c9d99-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c9d99-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c9d99-128">period</span><span class="sxs-lookup"><span data-stu-id="c9d99-128">period</span></span>    | <span data-ttu-id="c9d99-129">string</span><span class="sxs-lookup"><span data-stu-id="c9d99-129">string</span></span> | <span data-ttu-id="c9d99-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c9d99-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c9d99-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c9d99-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c9d99-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c9d99-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c9d99-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9d99-133">Required.</span></span> |

<span data-ttu-id="c9d99-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d99-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c9d99-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c9d99-135">The default output type is text/csv.</span></span> <span data-ttu-id="c9d99-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c9d99-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9d99-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9d99-137">Request headers</span></span>

| <span data-ttu-id="c9d99-138">Имя</span><span class="sxs-lookup"><span data-stu-id="c9d99-138">Name</span></span>          | <span data-ttu-id="c9d99-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c9d99-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c9d99-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9d99-140">Authorization</span></span> | <span data-ttu-id="c9d99-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c9d99-141">Bearer {token}.</span></span> <span data-ttu-id="c9d99-142">Required.</span><span class="sxs-lookup"><span data-stu-id="c9d99-142">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c9d99-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9d99-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c9d99-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c9d99-144">CSV</span></span>

<span data-ttu-id="c9d99-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c9d99-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c9d99-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d99-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c9d99-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c9d99-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c9d99-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c9d99-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c9d99-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c9d99-149">Report Refresh Date</span></span>
- <span data-ttu-id="c9d99-150">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="c9d99-150">Site Type</span></span>
- <span data-ttu-id="c9d99-151">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="c9d99-151">Total</span></span>
- <span data-ttu-id="c9d99-152">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="c9d99-152">Active</span></span>
- <span data-ttu-id="c9d99-153">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="c9d99-153">Report Date</span></span>
- <span data-ttu-id="c9d99-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="c9d99-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c9d99-155">JSON</span><span class="sxs-lookup"><span data-stu-id="c9d99-155">JSON</span></span>

<span data-ttu-id="c9d99-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажеаккаунткаунтс](../resources/onedriveusageaccountcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d99-156">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9d99-157">Пример</span><span class="sxs-lookup"><span data-stu-id="c9d99-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c9d99-158">CSV</span><span class="sxs-lookup"><span data-stu-id="c9d99-158">CSV</span></span>

<span data-ttu-id="c9d99-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c9d99-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c9d99-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9d99-160">Request</span></span>

<span data-ttu-id="c9d99-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9d99-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="c9d99-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9d99-162">Response</span></span>

<span data-ttu-id="c9d99-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d99-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c9d99-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c9d99-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="c9d99-165">JSON</span><span class="sxs-lookup"><span data-stu-id="c9d99-165">JSON</span></span>

<span data-ttu-id="c9d99-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c9d99-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c9d99-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9d99-167">Request</span></span>

<span data-ttu-id="c9d99-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9d99-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="c9d99-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9d99-169">Response</span></span>

<span data-ttu-id="c9d99-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9d99-170">The following is an example of the response.</span></span>

> <span data-ttu-id="c9d99-171">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="c9d99-171">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c9d99-172">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c9d99-172">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
