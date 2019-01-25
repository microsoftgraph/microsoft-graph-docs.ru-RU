---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 409c489ca985c7a357be13ae0ee0a487b54f1eac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528174"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="f7c22-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="f7c22-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c22-104">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="f7c22-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="f7c22-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="f7c22-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c22-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c22-106">Permissions</span></span>

<span data-ttu-id="f7c22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7c22-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c22-109">Permission type</span></span>                        | <span data-ttu-id="f7c22-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c22-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f7c22-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c22-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7c22-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7c22-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f7c22-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c22-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c22-114">Not supported.</span></span>                           |
| <span data-ttu-id="f7c22-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7c22-115">Application</span></span>                            | <span data-ttu-id="f7c22-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7c22-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f7c22-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c22-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f7c22-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f7c22-118">Function parameters</span></span>

<span data-ttu-id="f7c22-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f7c22-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f7c22-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7c22-120">Parameter</span></span> | <span data-ttu-id="f7c22-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f7c22-121">Type</span></span>   | <span data-ttu-id="f7c22-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c22-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f7c22-123">period</span><span class="sxs-lookup"><span data-stu-id="f7c22-123">period</span></span>    | <span data-ttu-id="f7c22-124">строка</span><span class="sxs-lookup"><span data-stu-id="f7c22-124">string</span></span> | <span data-ttu-id="f7c22-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f7c22-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f7c22-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f7c22-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f7c22-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f7c22-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f7c22-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7c22-128">Required.</span></span> |

<span data-ttu-id="f7c22-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7c22-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f7c22-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="f7c22-130">The default output type is text/csv.</span></span> <span data-ttu-id="f7c22-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="f7c22-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7c22-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7c22-132">Request headers</span></span>

| <span data-ttu-id="f7c22-133">Имя</span><span class="sxs-lookup"><span data-stu-id="f7c22-133">Name</span></span>          | <span data-ttu-id="f7c22-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c22-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f7c22-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7c22-135">Authorization</span></span> | <span data-ttu-id="f7c22-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7c22-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f7c22-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7c22-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f7c22-139">CSV</span><span class="sxs-lookup"><span data-stu-id="f7c22-139">CSV</span></span>

<span data-ttu-id="f7c22-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f7c22-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f7c22-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c22-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f7c22-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f7c22-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f7c22-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f7c22-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="f7c22-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f7c22-144">Report Refresh Date</span></span>
- <span data-ttu-id="f7c22-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="f7c22-145">Office 365</span></span>
- <span data-ttu-id="f7c22-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="f7c22-146">Exchange</span></span>
- <span data-ttu-id="f7c22-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="f7c22-147">OneDrive</span></span>
- <span data-ttu-id="f7c22-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="f7c22-148">SharePoint</span></span>
- <span data-ttu-id="f7c22-149">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f7c22-149">Skype For Business</span></span> 
- <span data-ttu-id="f7c22-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="f7c22-150">Yammer</span></span>
- <span data-ttu-id="f7c22-151">Teams</span><span class="sxs-lookup"><span data-stu-id="f7c22-151">Teams</span></span>
- <span data-ttu-id="f7c22-152">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="f7c22-152">Report Date</span></span>
- <span data-ttu-id="f7c22-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="f7c22-153">Report Period</span></span>

<span data-ttu-id="f7c22-154">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="f7c22-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="f7c22-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="f7c22-155">Yammer</span></span>
- <span data-ttu-id="f7c22-156">Teams</span><span class="sxs-lookup"><span data-stu-id="f7c22-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="f7c22-157">JSON</span><span class="sxs-lookup"><span data-stu-id="f7c22-157">JSON</span></span>

<span data-ttu-id="f7c22-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7c22-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="f7c22-159">Следующие свойства объекта **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="f7c22-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="f7c22-160">Yammer</span><span class="sxs-lookup"><span data-stu-id="f7c22-160">yammer</span></span>
- <span data-ttu-id="f7c22-161">Команды</span><span class="sxs-lookup"><span data-stu-id="f7c22-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="f7c22-162">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c22-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f7c22-163">CSV</span><span class="sxs-lookup"><span data-stu-id="f7c22-163">CSV</span></span>

<span data-ttu-id="f7c22-164">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="f7c22-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f7c22-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c22-165">Request</span></span>

<span data-ttu-id="f7c22-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c22-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f7c22-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7c22-167">Response</span></span>

<span data-ttu-id="f7c22-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f7c22-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f7c22-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f7c22-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f7c22-170">JSON</span><span class="sxs-lookup"><span data-stu-id="f7c22-170">JSON</span></span>

<span data-ttu-id="f7c22-171">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="f7c22-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f7c22-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c22-172">Request</span></span>

<span data-ttu-id="f7c22-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c22-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f7c22-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7c22-174">Response</span></span>

<span data-ttu-id="f7c22-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c22-175">The following is an example of the response.</span></span>

> <span data-ttu-id="f7c22-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7c22-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
