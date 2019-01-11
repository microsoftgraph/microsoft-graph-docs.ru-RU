---
title: 'reportRoot: getYammerActivityUserDetail'
description: Получите сведения об активности пользователей в Yammer.
localization_priority: Normal
ms.openlocfilehash: da1337d6b925c7b729c950eeac35cc3a8981596e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839622"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="b2b5e-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b2b5e-103">reportRoot: getYammerActivityUserDetail</span></span>

> <span data-ttu-id="b2b5e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2b5e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2b5e-106">Получите сведения об активности пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-106">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="b2b5e-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="b2b5e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2b5e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b5e-108">Permissions</span></span>

<span data-ttu-id="b2b5e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2b5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b5e-111">Permission type</span></span>                        | <span data-ttu-id="b2b5e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b2b5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2b5e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b5e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b2b5e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2b5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-116">Not supported.</span></span>                           |
| <span data-ttu-id="b2b5e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2b5e-117">Application</span></span>                            | <span data-ttu-id="b2b5e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b5e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b2b5e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2b5e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b2b5e-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="b2b5e-120">Function parameters</span></span>

<span data-ttu-id="b2b5e-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b2b5e-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="b2b5e-122">Parameter</span></span> | <span data-ttu-id="b2b5e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b2b5e-123">Type</span></span>   | <span data-ttu-id="b2b5e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b5e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b2b5e-125">period</span><span class="sxs-lookup"><span data-stu-id="b2b5e-125">period</span></span>    | <span data-ttu-id="b2b5e-126">строка</span><span class="sxs-lookup"><span data-stu-id="b2b5e-126">string</span></span> | <span data-ttu-id="b2b5e-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b2b5e-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b2b5e-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b2b5e-130">date</span><span class="sxs-lookup"><span data-stu-id="b2b5e-130">date</span></span>      | <span data-ttu-id="b2b5e-131">Date</span><span class="sxs-lookup"><span data-stu-id="b2b5e-131">Date</span></span>   | <span data-ttu-id="b2b5e-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b2b5e-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b2b5e-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b2b5e-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b2b5e-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b2b5e-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-137">The default output type is text/csv.</span></span> <span data-ttu-id="b2b5e-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2b5e-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2b5e-139">Request headers</span></span>

| <span data-ttu-id="b2b5e-140">Имя</span><span class="sxs-lookup"><span data-stu-id="b2b5e-140">Name</span></span>          | <span data-ttu-id="b2b5e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="b2b5e-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b2b5e-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2b5e-142">Authorization</span></span> | <span data-ttu-id="b2b5e-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b2b5e-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2b5e-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b2b5e-146">CSV</span><span class="sxs-lookup"><span data-stu-id="b2b5e-146">CSV</span></span>

<span data-ttu-id="b2b5e-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b2b5e-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b2b5e-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b2b5e-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b2b5e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b2b5e-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b2b5e-151">Report Refresh Date</span></span>
- <span data-ttu-id="b2b5e-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="b2b5e-152">User Principal Name</span></span>
- <span data-ttu-id="b2b5e-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="b2b5e-153">Display Name</span></span>
- <span data-ttu-id="b2b5e-154">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="b2b5e-154">User State</span></span>
- <span data-ttu-id="b2b5e-155">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="b2b5e-155">State Change Date</span></span>
- <span data-ttu-id="b2b5e-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-156">Last Activity Date</span></span>
- <span data-ttu-id="b2b5e-157">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-157">Posted Count</span></span>
- <span data-ttu-id="b2b5e-158">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-158">Read Count</span></span>
- <span data-ttu-id="b2b5e-159">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-159">Liked Count</span></span>
- <span data-ttu-id="b2b5e-160">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="b2b5e-160">Assigned Products</span></span>
- <span data-ttu-id="b2b5e-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b2b5e-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b2b5e-162">JSON</span><span class="sxs-lookup"><span data-stu-id="b2b5e-162">JSON</span></span>

<span data-ttu-id="b2b5e-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-163">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b2b5e-164">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b2b5e-165">Пример</span><span class="sxs-lookup"><span data-stu-id="b2b5e-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b2b5e-166">CSV</span><span class="sxs-lookup"><span data-stu-id="b2b5e-166">CSV</span></span>

<span data-ttu-id="b2b5e-167">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b2b5e-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2b5e-168">Request</span></span>

<span data-ttu-id="b2b5e-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b2b5e-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2b5e-170">Response</span></span>

<span data-ttu-id="b2b5e-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b2b5e-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="b2b5e-173">JSON</span><span class="sxs-lookup"><span data-stu-id="b2b5e-173">JSON</span></span>

<span data-ttu-id="b2b5e-174">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b2b5e-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2b5e-175">Request</span></span>

<span data-ttu-id="b2b5e-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b2b5e-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2b5e-177">Response</span></span>

<span data-ttu-id="b2b5e-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-178">The following is an example of the response.</span></span>

> <span data-ttu-id="b2b5e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2b5e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
