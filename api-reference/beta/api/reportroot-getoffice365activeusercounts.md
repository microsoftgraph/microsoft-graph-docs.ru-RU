---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2b155d27a0c32f934b6e5ea980f5ba85a5c8c652
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053533"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="a9353-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="a9353-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="a9353-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9353-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9353-105">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="a9353-105">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="a9353-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="a9353-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9353-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9353-107">Permissions</span></span>

<span data-ttu-id="a9353-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9353-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9353-110">Permission type</span></span>                        | <span data-ttu-id="a9353-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9353-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a9353-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9353-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9353-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9353-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a9353-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9353-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9353-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9353-115">Not supported.</span></span>                           |
| <span data-ttu-id="a9353-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9353-116">Application</span></span>                            | <span data-ttu-id="a9353-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9353-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a9353-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a9353-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a9353-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a9353-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a9353-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9353-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a9353-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a9353-121">Function parameters</span></span>

<span data-ttu-id="a9353-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a9353-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a9353-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a9353-123">Parameter</span></span> | <span data-ttu-id="a9353-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a9353-124">Type</span></span>   | <span data-ttu-id="a9353-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a9353-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a9353-126">period</span><span class="sxs-lookup"><span data-stu-id="a9353-126">period</span></span>    | <span data-ttu-id="a9353-127">string</span><span class="sxs-lookup"><span data-stu-id="a9353-127">string</span></span> | <span data-ttu-id="a9353-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a9353-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a9353-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a9353-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a9353-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a9353-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a9353-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9353-131">Required.</span></span> |

<span data-ttu-id="a9353-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a9353-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a9353-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="a9353-133">The default output type is text/csv.</span></span> <span data-ttu-id="a9353-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="a9353-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9353-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9353-135">Request headers</span></span>

| <span data-ttu-id="a9353-136">Имя</span><span class="sxs-lookup"><span data-stu-id="a9353-136">Name</span></span>          | <span data-ttu-id="a9353-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a9353-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a9353-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9353-138">Authorization</span></span> | <span data-ttu-id="a9353-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9353-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a9353-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9353-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a9353-142">CSV</span><span class="sxs-lookup"><span data-stu-id="a9353-142">CSV</span></span>

<span data-ttu-id="a9353-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a9353-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a9353-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a9353-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a9353-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a9353-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a9353-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a9353-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="a9353-147">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a9353-147">Report Refresh Date</span></span>
- <span data-ttu-id="a9353-148">Office 365</span><span class="sxs-lookup"><span data-stu-id="a9353-148">Office 365</span></span>
- <span data-ttu-id="a9353-149">Exchange</span><span class="sxs-lookup"><span data-stu-id="a9353-149">Exchange</span></span>
- <span data-ttu-id="a9353-150">OneDrive</span><span class="sxs-lookup"><span data-stu-id="a9353-150">OneDrive</span></span>
- <span data-ttu-id="a9353-151">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="a9353-151">SharePoint</span></span>
- <span data-ttu-id="a9353-152">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="a9353-152">Skype For Business</span></span> 
- <span data-ttu-id="a9353-153">Yammer</span><span class="sxs-lookup"><span data-stu-id="a9353-153">Yammer</span></span>
- <span data-ttu-id="a9353-154">Teams</span><span class="sxs-lookup"><span data-stu-id="a9353-154">Teams</span></span>
- <span data-ttu-id="a9353-155">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="a9353-155">Report Date</span></span>
- <span data-ttu-id="a9353-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="a9353-156">Report Period</span></span>

<span data-ttu-id="a9353-157">Следующие столбцы не поддерживаются в Microsoft Graph Китае, выполняемых 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="a9353-157">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="a9353-158">Yammer</span><span class="sxs-lookup"><span data-stu-id="a9353-158">Yammer</span></span>
- <span data-ttu-id="a9353-159">Teams</span><span class="sxs-lookup"><span data-stu-id="a9353-159">Teams</span></span>

### <a name="json"></a><span data-ttu-id="a9353-160">JSON</span><span class="sxs-lookup"><span data-stu-id="a9353-160">JSON</span></span>

<span data-ttu-id="a9353-161">В случае успешной работы этот метод возвращает код отклика и `200 OK` **[объект Office365ActiveUserCounts](../resources/office365activeusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9353-161">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="a9353-162">Следующие свойства в **[объекте Office365ActiveUserCounts](../resources/office365activeusercounts.md)** не поддерживаются в Microsoft Graph Китае под управлением 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="a9353-162">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="a9353-163">yammer</span><span class="sxs-lookup"><span data-stu-id="a9353-163">yammer</span></span>
- <span data-ttu-id="a9353-164">teams</span><span class="sxs-lookup"><span data-stu-id="a9353-164">teams</span></span>

## <a name="example"></a><span data-ttu-id="a9353-165">Пример</span><span class="sxs-lookup"><span data-stu-id="a9353-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a9353-166">CSV</span><span class="sxs-lookup"><span data-stu-id="a9353-166">CSV</span></span>

<span data-ttu-id="a9353-167">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="a9353-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a9353-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9353-168">Request</span></span>

<span data-ttu-id="a9353-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9353-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a9353-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9353-170">Response</span></span>

<span data-ttu-id="a9353-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9353-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a9353-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a9353-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a9353-173">JSON</span><span class="sxs-lookup"><span data-stu-id="a9353-173">JSON</span></span>

<span data-ttu-id="a9353-174">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="a9353-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a9353-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9353-175">Request</span></span>

<span data-ttu-id="a9353-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9353-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a9353-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9353-177">Response</span></span>

<span data-ttu-id="a9353-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a9353-178">The following is an example of the response.</span></span>

> <span data-ttu-id="a9353-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a9353-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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


