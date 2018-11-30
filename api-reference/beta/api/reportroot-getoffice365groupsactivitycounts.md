---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Узнайте, сколько различных действий было в группах.
ms.openlocfilehash: 0dfcf2a20344c3f0336f9042b22295c7a9b0e2b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074611"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="67058-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="67058-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

> <span data-ttu-id="67058-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67058-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67058-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67058-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67058-106">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="67058-106">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="67058-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="67058-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="67058-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67058-108">Permissions</span></span>

<span data-ttu-id="67058-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67058-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67058-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67058-111">Permission type</span></span>                        | <span data-ttu-id="67058-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67058-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="67058-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67058-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="67058-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67058-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="67058-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67058-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67058-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67058-116">Not supported.</span></span>                           |
| <span data-ttu-id="67058-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67058-117">Application</span></span>                            | <span data-ttu-id="67058-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67058-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="67058-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67058-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="67058-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="67058-120">Function parameters</span></span>

<span data-ttu-id="67058-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="67058-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="67058-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="67058-122">Parameter</span></span> | <span data-ttu-id="67058-123">Тип</span><span class="sxs-lookup"><span data-stu-id="67058-123">Type</span></span>   | <span data-ttu-id="67058-124">Описание</span><span class="sxs-lookup"><span data-stu-id="67058-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="67058-125">period</span><span class="sxs-lookup"><span data-stu-id="67058-125">period</span></span>    | <span data-ttu-id="67058-126">строка</span><span class="sxs-lookup"><span data-stu-id="67058-126">string</span></span> | <span data-ttu-id="67058-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="67058-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="67058-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="67058-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="67058-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="67058-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="67058-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67058-130">Required.</span></span> |

<span data-ttu-id="67058-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67058-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="67058-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="67058-132">The default output type is text/csv.</span></span> <span data-ttu-id="67058-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="67058-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67058-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67058-134">Request headers</span></span>

| <span data-ttu-id="67058-135">Имя</span><span class="sxs-lookup"><span data-stu-id="67058-135">Name</span></span>          | <span data-ttu-id="67058-136">Описание</span><span class="sxs-lookup"><span data-stu-id="67058-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="67058-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67058-137">Authorization</span></span> | <span data-ttu-id="67058-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67058-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="67058-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="67058-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="67058-141">CSV</span><span class="sxs-lookup"><span data-stu-id="67058-141">CSV</span></span>

<span data-ttu-id="67058-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="67058-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="67058-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="67058-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="67058-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="67058-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="67058-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="67058-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="67058-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="67058-146">Report Refresh Date</span></span>
- <span data-ttu-id="67058-147">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="67058-147">Exchange Emails Received</span></span>
- <span data-ttu-id="67058-148">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="67058-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="67058-149">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="67058-149">Yammer Messages Read</span></span>
- <span data-ttu-id="67058-150">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="67058-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="67058-151">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="67058-151">Report Date</span></span>
- <span data-ttu-id="67058-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="67058-152">Report Period</span></span>

<span data-ttu-id="67058-153">В Китае Microsoft Graph обслуживается 21Vianet не поддерживаются следующие столбцы:</span><span class="sxs-lookup"><span data-stu-id="67058-153">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="67058-154">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="67058-154">Yammer Messages Posted</span></span>
- <span data-ttu-id="67058-155">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="67058-155">Yammer Messages Read</span></span>
- <span data-ttu-id="67058-156">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="67058-156">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="67058-157">JSON</span><span class="sxs-lookup"><span data-stu-id="67058-157">JSON</span></span>

<span data-ttu-id="67058-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="67058-158">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="67058-159">Следующие свойства объекта **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** не поддерживаются в Китае Microsoft Graph обслуживается 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="67058-159">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="67058-160">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="67058-160">yammerMessagesPosted</span></span>
- <span data-ttu-id="67058-161">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="67058-161">yammerMessagesRead</span></span>
- <span data-ttu-id="67058-162">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="67058-162">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="67058-163">Пример</span><span class="sxs-lookup"><span data-stu-id="67058-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="67058-164">CSV</span><span class="sxs-lookup"><span data-stu-id="67058-164">CSV</span></span>

<span data-ttu-id="67058-165">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="67058-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="67058-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="67058-166">Request</span></span>

<span data-ttu-id="67058-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67058-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="67058-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="67058-168">Response</span></span>

<span data-ttu-id="67058-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="67058-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="67058-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="67058-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="67058-171">JSON</span><span class="sxs-lookup"><span data-stu-id="67058-171">JSON</span></span>

<span data-ttu-id="67058-172">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="67058-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="67058-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="67058-173">Request</span></span>

<span data-ttu-id="67058-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67058-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="67058-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="67058-175">Response</span></span>

<span data-ttu-id="67058-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67058-176">The following is an example of the response.</span></span>

> <span data-ttu-id="67058-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67058-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
