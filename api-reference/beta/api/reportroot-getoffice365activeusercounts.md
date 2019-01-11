---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.openlocfilehash: 0213ee12ec73fc43a0a321fa77d4c0d2495e4210
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844487"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="3a864-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="3a864-103">reportRoot: getOffice365ActiveUserCounts</span></span>

> <span data-ttu-id="3a864-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a864-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a864-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a864-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a864-106">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="3a864-106">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="3a864-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="3a864-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a864-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a864-108">Permissions</span></span>

<span data-ttu-id="3a864-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a864-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a864-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a864-111">Permission type</span></span>                        | <span data-ttu-id="3a864-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a864-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3a864-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a864-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a864-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a864-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3a864-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a864-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a864-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a864-116">Not supported.</span></span>                           |
| <span data-ttu-id="3a864-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a864-117">Application</span></span>                            | <span data-ttu-id="3a864-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a864-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3a864-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a864-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3a864-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="3a864-120">Function parameters</span></span>

<span data-ttu-id="3a864-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3a864-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3a864-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="3a864-122">Parameter</span></span> | <span data-ttu-id="3a864-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3a864-123">Type</span></span>   | <span data-ttu-id="3a864-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3a864-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3a864-125">period</span><span class="sxs-lookup"><span data-stu-id="3a864-125">period</span></span>    | <span data-ttu-id="3a864-126">строка</span><span class="sxs-lookup"><span data-stu-id="3a864-126">string</span></span> | <span data-ttu-id="3a864-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3a864-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3a864-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3a864-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3a864-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3a864-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3a864-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a864-130">Required.</span></span> |

<span data-ttu-id="3a864-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a864-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3a864-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="3a864-132">The default output type is text/csv.</span></span> <span data-ttu-id="3a864-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="3a864-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a864-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a864-134">Request headers</span></span>

| <span data-ttu-id="3a864-135">Имя</span><span class="sxs-lookup"><span data-stu-id="3a864-135">Name</span></span>          | <span data-ttu-id="3a864-136">Описание</span><span class="sxs-lookup"><span data-stu-id="3a864-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3a864-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a864-137">Authorization</span></span> | <span data-ttu-id="3a864-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a864-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3a864-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a864-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3a864-141">CSV</span><span class="sxs-lookup"><span data-stu-id="3a864-141">CSV</span></span>

<span data-ttu-id="3a864-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3a864-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3a864-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3a864-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3a864-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3a864-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3a864-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3a864-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3a864-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3a864-146">Report Refresh Date</span></span>
- <span data-ttu-id="3a864-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="3a864-147">Office 365</span></span>
- <span data-ttu-id="3a864-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="3a864-148">Exchange</span></span>
- <span data-ttu-id="3a864-149">OneDrive</span><span class="sxs-lookup"><span data-stu-id="3a864-149">OneDrive</span></span>
- <span data-ttu-id="3a864-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="3a864-150">SharePoint</span></span>
- <span data-ttu-id="3a864-151">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="3a864-151">Skype For Business</span></span> 
- <span data-ttu-id="3a864-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="3a864-152">Yammer</span></span>
- <span data-ttu-id="3a864-153">Teams</span><span class="sxs-lookup"><span data-stu-id="3a864-153">Teams</span></span>
- <span data-ttu-id="3a864-154">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="3a864-154">Report Date</span></span>
- <span data-ttu-id="3a864-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3a864-155">Report Period</span></span>

<span data-ttu-id="3a864-156">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="3a864-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="3a864-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="3a864-157">Yammer</span></span>
- <span data-ttu-id="3a864-158">Teams</span><span class="sxs-lookup"><span data-stu-id="3a864-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="3a864-159">JSON</span><span class="sxs-lookup"><span data-stu-id="3a864-159">JSON</span></span>

<span data-ttu-id="3a864-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a864-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="3a864-161">Следующие свойства объекта **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="3a864-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="3a864-162">Yammer</span><span class="sxs-lookup"><span data-stu-id="3a864-162">yammer</span></span>
- <span data-ttu-id="3a864-163">группы</span><span class="sxs-lookup"><span data-stu-id="3a864-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="3a864-164">Пример</span><span class="sxs-lookup"><span data-stu-id="3a864-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3a864-165">CSV</span><span class="sxs-lookup"><span data-stu-id="3a864-165">CSV</span></span>

<span data-ttu-id="3a864-166">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="3a864-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3a864-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a864-167">Request</span></span>

<span data-ttu-id="3a864-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a864-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3a864-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a864-169">Response</span></span>

<span data-ttu-id="3a864-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3a864-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3a864-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3a864-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3a864-172">JSON</span><span class="sxs-lookup"><span data-stu-id="3a864-172">JSON</span></span>

<span data-ttu-id="3a864-173">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3a864-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3a864-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a864-174">Request</span></span>

<span data-ttu-id="3a864-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a864-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3a864-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a864-176">Response</span></span>

<span data-ttu-id="3a864-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a864-177">The following is an example of the response.</span></span>

> <span data-ttu-id="3a864-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a864-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
