---
title: 'reportRoot: getOneDriveUsageStorage'
description: Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: b6e84fc317ee896d034476687a38ccb8b6b8efa7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983659"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="275d4-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="275d4-103">reportRoot: getOneDriveUsageStorage</span></span>

<span data-ttu-id="275d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="275d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="275d4-105">Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="275d4-105">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="275d4-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)</span><span class="sxs-lookup"><span data-stu-id="275d4-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="275d4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="275d4-107">Permissions</span></span>

<span data-ttu-id="275d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="275d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="275d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="275d4-110">Permission type</span></span>                        | <span data-ttu-id="275d4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="275d4-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="275d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="275d4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="275d4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="275d4-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="275d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="275d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="275d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="275d4-115">Not supported.</span></span>                           |
| <span data-ttu-id="275d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="275d4-116">Application</span></span>                            | <span data-ttu-id="275d4-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="275d4-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="275d4-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="275d4-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="275d4-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="275d4-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="275d4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="275d4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="275d4-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="275d4-121">Function parameters</span></span>

<span data-ttu-id="275d4-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="275d4-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="275d4-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="275d4-123">Parameter</span></span> | <span data-ttu-id="275d4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="275d4-124">Type</span></span>   | <span data-ttu-id="275d4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="275d4-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="275d4-126">period</span><span class="sxs-lookup"><span data-stu-id="275d4-126">period</span></span>    | <span data-ttu-id="275d4-127">string</span><span class="sxs-lookup"><span data-stu-id="275d4-127">string</span></span> | <span data-ttu-id="275d4-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="275d4-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="275d4-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="275d4-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="275d4-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="275d4-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="275d4-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="275d4-131">Required.</span></span> |

<span data-ttu-id="275d4-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="275d4-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="275d4-133">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="275d4-133">The default output type is text/csv.</span></span> <span data-ttu-id="275d4-134">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="275d4-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="275d4-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="275d4-135">Request headers</span></span>

| <span data-ttu-id="275d4-136">Имя</span><span class="sxs-lookup"><span data-stu-id="275d4-136">Name</span></span>          | <span data-ttu-id="275d4-137">Описание</span><span class="sxs-lookup"><span data-stu-id="275d4-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="275d4-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="275d4-138">Authorization</span></span> | <span data-ttu-id="275d4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="275d4-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="275d4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="275d4-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="275d4-142">CSV</span><span class="sxs-lookup"><span data-stu-id="275d4-142">CSV</span></span>

<span data-ttu-id="275d4-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="275d4-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="275d4-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="275d4-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="275d4-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="275d4-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="275d4-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="275d4-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="275d4-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="275d4-147">Report Refresh Date</span></span>
- <span data-ttu-id="275d4-148">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="275d4-148">Site Type</span></span>
- <span data-ttu-id="275d4-149">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="275d4-149">Storage Used (Byte)</span></span>
- <span data-ttu-id="275d4-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="275d4-150">Report Date</span></span>
- <span data-ttu-id="275d4-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="275d4-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="275d4-152">JSON</span><span class="sxs-lookup"><span data-stu-id="275d4-152">JSON</span></span>

<span data-ttu-id="275d4-153">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[siteUsageStorage](../resources/siteusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="275d4-153">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="275d4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="275d4-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="275d4-155">CSV</span><span class="sxs-lookup"><span data-stu-id="275d4-155">CSV</span></span>

<span data-ttu-id="275d4-156">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="275d4-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="275d4-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="275d4-157">Request</span></span>

<span data-ttu-id="275d4-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="275d4-158">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="275d4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="275d4-159">Response</span></span>

<span data-ttu-id="275d4-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="275d4-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="275d4-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="275d4-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="275d4-162">JSON</span><span class="sxs-lookup"><span data-stu-id="275d4-162">JSON</span></span>

<span data-ttu-id="275d4-163">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="275d4-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="275d4-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="275d4-164">Request</span></span>

<span data-ttu-id="275d4-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="275d4-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="275d4-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="275d4-166">Response</span></span>

<span data-ttu-id="275d4-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="275d4-167">The following is an example of the response.</span></span>

> <span data-ttu-id="275d4-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="275d4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 132654293197, 
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


