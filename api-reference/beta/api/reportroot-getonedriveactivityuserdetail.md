---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
ms.openlocfilehash: b992960a366ba6b8596b8b276abcd88afb5e8855
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076420"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="97296-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="97296-103">reportRoot: getOneDriveActivityUserDetail</span></span>

> <span data-ttu-id="97296-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97296-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97296-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97296-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97296-106">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="97296-106">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="97296-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="97296-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="97296-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97296-108">Permissions</span></span>

<span data-ttu-id="97296-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97296-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97296-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97296-111">Permission type</span></span>                        | <span data-ttu-id="97296-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97296-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="97296-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97296-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="97296-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97296-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="97296-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97296-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97296-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97296-116">Not supported.</span></span>                           |
| <span data-ttu-id="97296-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97296-117">Application</span></span>                            | <span data-ttu-id="97296-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97296-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="97296-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97296-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="97296-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="97296-120">Function parameters</span></span>

<span data-ttu-id="97296-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="97296-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="97296-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="97296-122">Parameter</span></span> | <span data-ttu-id="97296-123">Тип</span><span class="sxs-lookup"><span data-stu-id="97296-123">Type</span></span>   | <span data-ttu-id="97296-124">Описание</span><span class="sxs-lookup"><span data-stu-id="97296-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="97296-125">period</span><span class="sxs-lookup"><span data-stu-id="97296-125">period</span></span>    | <span data-ttu-id="97296-126">строка</span><span class="sxs-lookup"><span data-stu-id="97296-126">string</span></span> | <span data-ttu-id="97296-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="97296-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="97296-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="97296-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="97296-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="97296-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="97296-130">date</span><span class="sxs-lookup"><span data-stu-id="97296-130">date</span></span>      | <span data-ttu-id="97296-131">Date</span><span class="sxs-lookup"><span data-stu-id="97296-131">Date</span></span>   | <span data-ttu-id="97296-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="97296-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="97296-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="97296-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="97296-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="97296-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="97296-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="97296-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="97296-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97296-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="97296-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="97296-137">The default output type is text/csv.</span></span> <span data-ttu-id="97296-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="97296-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97296-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97296-139">Request headers</span></span>

| <span data-ttu-id="97296-140">Имя</span><span class="sxs-lookup"><span data-stu-id="97296-140">Name</span></span>          | <span data-ttu-id="97296-141">Описание</span><span class="sxs-lookup"><span data-stu-id="97296-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="97296-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97296-142">Authorization</span></span> | <span data-ttu-id="97296-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97296-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="97296-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="97296-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="97296-146">CSV</span><span class="sxs-lookup"><span data-stu-id="97296-146">CSV</span></span>

<span data-ttu-id="97296-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="97296-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="97296-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="97296-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="97296-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="97296-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="97296-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="97296-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="97296-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="97296-151">Report Refresh Date</span></span>
- <span data-ttu-id="97296-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="97296-152">User Principal Name</span></span>
- <span data-ttu-id="97296-153">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="97296-153">Is Deleted</span></span>
- <span data-ttu-id="97296-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="97296-154">Deleted Date</span></span>
- <span data-ttu-id="97296-155">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="97296-155">Last Activity Date</span></span>
- <span data-ttu-id="97296-156">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="97296-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="97296-157">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="97296-157">Synced File Count</span></span>
- <span data-ttu-id="97296-158">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="97296-158">Shared Internally File Count</span></span>
- <span data-ttu-id="97296-159">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="97296-159">Shared Externally File Count</span></span>
- <span data-ttu-id="97296-160">"Assigned Products" (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="97296-160">Assigned Products</span></span>
- <span data-ttu-id="97296-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="97296-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="97296-162">JSON</span><span class="sxs-lookup"><span data-stu-id="97296-162">JSON</span></span>

<span data-ttu-id="97296-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="97296-163">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="97296-164">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="97296-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="97296-165">Пример</span><span class="sxs-lookup"><span data-stu-id="97296-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="97296-166">CSV</span><span class="sxs-lookup"><span data-stu-id="97296-166">CSV</span></span>

<span data-ttu-id="97296-167">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="97296-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="97296-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="97296-168">Request</span></span>

<span data-ttu-id="97296-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97296-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="97296-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="97296-170">Response</span></span>

<span data-ttu-id="97296-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="97296-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="97296-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="97296-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="97296-173">JSON</span><span class="sxs-lookup"><span data-stu-id="97296-173">JSON</span></span>

<span data-ttu-id="97296-174">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="97296-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="97296-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="97296-175">Request</span></span>

<span data-ttu-id="97296-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97296-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="97296-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="97296-177">Response</span></span>

<span data-ttu-id="97296-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97296-178">The following is an example of the response.</span></span>

> <span data-ttu-id="97296-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97296-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
