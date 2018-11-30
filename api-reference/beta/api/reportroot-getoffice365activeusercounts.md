---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
ms.openlocfilehash: 29cb7a18520774b192d5e9e71b62a7ca86fa9be5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077364"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="41abd-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="41abd-103">reportRoot: getOffice365ActiveUserCounts</span></span>

> <span data-ttu-id="41abd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="41abd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41abd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41abd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41abd-106">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="41abd-106">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="41abd-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="41abd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="41abd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41abd-108">Permissions</span></span>

<span data-ttu-id="41abd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41abd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41abd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41abd-111">Permission type</span></span>                        | <span data-ttu-id="41abd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41abd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="41abd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41abd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="41abd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41abd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="41abd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41abd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41abd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41abd-116">Not supported.</span></span>                           |
| <span data-ttu-id="41abd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41abd-117">Application</span></span>                            | <span data-ttu-id="41abd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41abd-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="41abd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41abd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="41abd-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="41abd-120">Function parameters</span></span>

<span data-ttu-id="41abd-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="41abd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="41abd-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="41abd-122">Parameter</span></span> | <span data-ttu-id="41abd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="41abd-123">Type</span></span>   | <span data-ttu-id="41abd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="41abd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="41abd-125">period</span><span class="sxs-lookup"><span data-stu-id="41abd-125">period</span></span>    | <span data-ttu-id="41abd-126">строка</span><span class="sxs-lookup"><span data-stu-id="41abd-126">string</span></span> | <span data-ttu-id="41abd-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="41abd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="41abd-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="41abd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="41abd-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="41abd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="41abd-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41abd-130">Required.</span></span> |

<span data-ttu-id="41abd-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="41abd-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="41abd-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="41abd-132">The default output type is text/csv.</span></span> <span data-ttu-id="41abd-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="41abd-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41abd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41abd-134">Request headers</span></span>

| <span data-ttu-id="41abd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="41abd-135">Name</span></span>          | <span data-ttu-id="41abd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="41abd-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="41abd-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41abd-137">Authorization</span></span> | <span data-ttu-id="41abd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41abd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="41abd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="41abd-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="41abd-141">CSV</span><span class="sxs-lookup"><span data-stu-id="41abd-141">CSV</span></span>

<span data-ttu-id="41abd-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="41abd-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="41abd-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="41abd-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="41abd-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="41abd-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="41abd-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="41abd-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="41abd-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="41abd-146">Report Refresh Date</span></span>
- <span data-ttu-id="41abd-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="41abd-147">Office 365</span></span>
- <span data-ttu-id="41abd-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="41abd-148">Exchange</span></span>
- <span data-ttu-id="41abd-149">OneDrive</span><span class="sxs-lookup"><span data-stu-id="41abd-149">OneDrive</span></span>
- <span data-ttu-id="41abd-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="41abd-150">SharePoint</span></span>
- <span data-ttu-id="41abd-151">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="41abd-151">Skype For Business</span></span> 
- <span data-ttu-id="41abd-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="41abd-152">Yammer</span></span>
- <span data-ttu-id="41abd-153">Teams</span><span class="sxs-lookup"><span data-stu-id="41abd-153">Teams</span></span>
- <span data-ttu-id="41abd-154">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="41abd-154">Report Date</span></span>
- <span data-ttu-id="41abd-155">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="41abd-155">Report Period</span></span>

<span data-ttu-id="41abd-156">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="41abd-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="41abd-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="41abd-157">Yammer</span></span>
- <span data-ttu-id="41abd-158">Teams</span><span class="sxs-lookup"><span data-stu-id="41abd-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="41abd-159">JSON</span><span class="sxs-lookup"><span data-stu-id="41abd-159">JSON</span></span>

<span data-ttu-id="41abd-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="41abd-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="41abd-161">Следующие свойства объекта **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="41abd-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="41abd-162">Yammer</span><span class="sxs-lookup"><span data-stu-id="41abd-162">yammer</span></span>
- <span data-ttu-id="41abd-163">группы</span><span class="sxs-lookup"><span data-stu-id="41abd-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="41abd-164">Пример</span><span class="sxs-lookup"><span data-stu-id="41abd-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="41abd-165">CSV</span><span class="sxs-lookup"><span data-stu-id="41abd-165">CSV</span></span>

<span data-ttu-id="41abd-166">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="41abd-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="41abd-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="41abd-167">Request</span></span>

<span data-ttu-id="41abd-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41abd-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="41abd-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="41abd-169">Response</span></span>

<span data-ttu-id="41abd-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41abd-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="41abd-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="41abd-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="41abd-172">JSON</span><span class="sxs-lookup"><span data-stu-id="41abd-172">JSON</span></span>

<span data-ttu-id="41abd-173">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="41abd-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="41abd-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="41abd-174">Request</span></span>

<span data-ttu-id="41abd-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41abd-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="41abd-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="41abd-176">Response</span></span>

<span data-ttu-id="41abd-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41abd-177">The following is an example of the response.</span></span>

> <span data-ttu-id="41abd-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41abd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
