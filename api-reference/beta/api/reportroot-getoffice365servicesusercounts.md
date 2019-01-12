---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1911b570d046f192d57435d58c7473333aa53e60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956173"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="218bd-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="218bd-103">reportRoot: getOffice365ServicesUserCounts</span></span>

> <span data-ttu-id="218bd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="218bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="218bd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="218bd-106">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="218bd-106">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="218bd-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="218bd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="218bd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="218bd-108">Permissions</span></span>

<span data-ttu-id="218bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="218bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="218bd-111">Permission type</span></span>                        | <span data-ttu-id="218bd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="218bd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="218bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="218bd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="218bd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="218bd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="218bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="218bd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218bd-116">Not supported.</span></span>                           |
| <span data-ttu-id="218bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="218bd-117">Application</span></span>                            | <span data-ttu-id="218bd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="218bd-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="218bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="218bd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="218bd-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="218bd-120">Function parameters</span></span>

<span data-ttu-id="218bd-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="218bd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="218bd-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="218bd-122">Parameter</span></span> | <span data-ttu-id="218bd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="218bd-123">Type</span></span>   | <span data-ttu-id="218bd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="218bd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="218bd-125">period</span><span class="sxs-lookup"><span data-stu-id="218bd-125">period</span></span>    | <span data-ttu-id="218bd-126">строка</span><span class="sxs-lookup"><span data-stu-id="218bd-126">string</span></span> | <span data-ttu-id="218bd-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="218bd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="218bd-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="218bd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="218bd-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="218bd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="218bd-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218bd-130">Required.</span></span> |

<span data-ttu-id="218bd-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="218bd-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="218bd-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="218bd-132">The default output type is text/csv.</span></span> <span data-ttu-id="218bd-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="218bd-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="218bd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="218bd-134">Request headers</span></span>

| <span data-ttu-id="218bd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="218bd-135">Name</span></span>          | <span data-ttu-id="218bd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="218bd-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="218bd-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="218bd-137">Authorization</span></span> | <span data-ttu-id="218bd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218bd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="218bd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="218bd-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="218bd-141">CSV</span><span class="sxs-lookup"><span data-stu-id="218bd-141">CSV</span></span>

<span data-ttu-id="218bd-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="218bd-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="218bd-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="218bd-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="218bd-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="218bd-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="218bd-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="218bd-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="218bd-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="218bd-146">Report Refresh Date</span></span>
- <span data-ttu-id="218bd-147">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="218bd-147">Exchange Active</span></span>
- <span data-ttu-id="218bd-148">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="218bd-148">Exchange Inactive</span></span>
- <span data-ttu-id="218bd-149">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="218bd-149">OneDrive Active</span></span>
- <span data-ttu-id="218bd-150">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="218bd-150">OneDrive Inactive</span></span>
- <span data-ttu-id="218bd-151">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="218bd-151">SharePoint Active</span></span>
- <span data-ttu-id="218bd-152">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="218bd-152">SharePoint Inactive</span></span>
- <span data-ttu-id="218bd-153">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="218bd-153">Skype For Business Active</span></span>
- <span data-ttu-id="218bd-154">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="218bd-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="218bd-155">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="218bd-155">Yammer Active</span></span>
- <span data-ttu-id="218bd-156">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="218bd-156">Yammer Inactive</span></span>
- <span data-ttu-id="218bd-157">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="218bd-157">Teams Active</span></span>
- <span data-ttu-id="218bd-158">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="218bd-158">Teams Inactive</span></span>
- <span data-ttu-id="218bd-159">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="218bd-159">Report Period</span></span>

<span data-ttu-id="218bd-160">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="218bd-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="218bd-161">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="218bd-161">Yammer Active</span></span>
- <span data-ttu-id="218bd-162">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="218bd-162">Yammer Inactive</span></span>
- <span data-ttu-id="218bd-163">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="218bd-163">Teams Active</span></span>
- <span data-ttu-id="218bd-164">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="218bd-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="218bd-165">JSON</span><span class="sxs-lookup"><span data-stu-id="218bd-165">JSON</span></span>

<span data-ttu-id="218bd-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="218bd-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="218bd-167">Следующие свойства объекта **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="218bd-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="218bd-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="218bd-168">yammerActive</span></span>
- <span data-ttu-id="218bd-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="218bd-169">yammerInactive</span></span>
- <span data-ttu-id="218bd-170">teamsActive</span><span class="sxs-lookup"><span data-stu-id="218bd-170">teamsActive</span></span>
- <span data-ttu-id="218bd-171">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="218bd-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="218bd-172">Пример</span><span class="sxs-lookup"><span data-stu-id="218bd-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="218bd-173">CSV</span><span class="sxs-lookup"><span data-stu-id="218bd-173">CSV</span></span>

<span data-ttu-id="218bd-174">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="218bd-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="218bd-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="218bd-175">Request</span></span>

<span data-ttu-id="218bd-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218bd-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="218bd-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="218bd-177">Response</span></span>

<span data-ttu-id="218bd-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="218bd-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="218bd-179">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="218bd-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="218bd-180">JSON</span><span class="sxs-lookup"><span data-stu-id="218bd-180">JSON</span></span> 

<span data-ttu-id="218bd-181">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="218bd-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="218bd-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="218bd-182">Request</span></span>

<span data-ttu-id="218bd-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218bd-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="218bd-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="218bd-184">Response</span></span>

<span data-ttu-id="218bd-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="218bd-185">The following is an example of the response.</span></span>

> <span data-ttu-id="218bd-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="218bd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "reportPeriod": "7"
    }
  ]
}
```
