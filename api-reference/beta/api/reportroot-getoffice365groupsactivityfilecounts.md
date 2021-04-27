---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Получите общее количество файлов и их количество на всех сайтах группы, связанных с Microsoft 365 группой.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: b7afdbd57fe20229039beaf9d3217535dca4523f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052854"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="5741b-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="5741b-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="5741b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5741b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5741b-105">Получите общее количество файлов и их количество на всех сайтах группы, связанных с Microsoft 365 группой.</span><span class="sxs-lookup"><span data-stu-id="5741b-105">Get the total number of files and how many of them were active across all group sites associated with a Microsoft 365 group.</span></span>

> <span data-ttu-id="5741b-106">**Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft 365 групп.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)</span><span class="sxs-lookup"><span data-stu-id="5741b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="5741b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5741b-107">Permissions</span></span>

<span data-ttu-id="5741b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5741b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5741b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5741b-110">Permission type</span></span>                        | <span data-ttu-id="5741b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5741b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5741b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5741b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5741b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5741b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5741b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5741b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5741b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5741b-115">Not supported.</span></span>                           |
| <span data-ttu-id="5741b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5741b-116">Application</span></span>                            | <span data-ttu-id="5741b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5741b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5741b-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5741b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5741b-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5741b-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5741b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5741b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5741b-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5741b-121">Function parameters</span></span>

<span data-ttu-id="5741b-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5741b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5741b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="5741b-123">Parameter</span></span> | <span data-ttu-id="5741b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="5741b-124">Type</span></span>   | <span data-ttu-id="5741b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5741b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5741b-126">period</span><span class="sxs-lookup"><span data-stu-id="5741b-126">period</span></span>    | <span data-ttu-id="5741b-127">string</span><span class="sxs-lookup"><span data-stu-id="5741b-127">string</span></span> | <span data-ttu-id="5741b-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5741b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5741b-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5741b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5741b-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5741b-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5741b-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5741b-131">Required.</span></span> |

<span data-ttu-id="5741b-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5741b-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5741b-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="5741b-133">The default output type is text/csv.</span></span> <span data-ttu-id="5741b-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="5741b-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5741b-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5741b-135">Request headers</span></span>

| <span data-ttu-id="5741b-136">Имя</span><span class="sxs-lookup"><span data-stu-id="5741b-136">Name</span></span>          | <span data-ttu-id="5741b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="5741b-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5741b-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5741b-138">Authorization</span></span> | <span data-ttu-id="5741b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5741b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5741b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5741b-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5741b-142">CSV</span><span class="sxs-lookup"><span data-stu-id="5741b-142">CSV</span></span>

<span data-ttu-id="5741b-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5741b-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5741b-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5741b-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5741b-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5741b-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5741b-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5741b-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5741b-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5741b-147">Report Refresh Date</span></span>
- <span data-ttu-id="5741b-148">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="5741b-148">Total</span></span>
- <span data-ttu-id="5741b-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="5741b-149">Active</span></span>
- <span data-ttu-id="5741b-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="5741b-150">Report Date</span></span>
- <span data-ttu-id="5741b-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="5741b-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5741b-152">JSON</span><span class="sxs-lookup"><span data-stu-id="5741b-152">JSON</span></span>

<span data-ttu-id="5741b-153">В случае успеха этот метод возвращает код отклика и `200 OK` **[объект Office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5741b-153">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5741b-154">Пример</span><span class="sxs-lookup"><span data-stu-id="5741b-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5741b-155">CSV</span><span class="sxs-lookup"><span data-stu-id="5741b-155">CSV</span></span>

<span data-ttu-id="5741b-156">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="5741b-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5741b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5741b-157">Request</span></span>

<span data-ttu-id="5741b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5741b-158">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="5741b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5741b-159">Response</span></span>

<span data-ttu-id="5741b-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5741b-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5741b-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5741b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="5741b-162">JSON</span><span class="sxs-lookup"><span data-stu-id="5741b-162">JSON</span></span>

<span data-ttu-id="5741b-163">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="5741b-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5741b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="5741b-164">Request</span></span>

<span data-ttu-id="5741b-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5741b-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivityfilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="5741b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5741b-166">Response</span></span>

<span data-ttu-id="5741b-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5741b-167">The following is an example of the response.</span></span>

> <span data-ttu-id="5741b-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5741b-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 26, 
      "active": 5, 
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


