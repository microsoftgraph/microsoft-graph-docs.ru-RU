---
title: 'reportRoot: getYammerActivityUserDetail'
description: Получите сведения об активности пользователей в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cb3f46ddaf52f306fc6452b96f1534e7e921fffb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898291"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="0988b-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0988b-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="0988b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0988b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0988b-105">Получение сведений о действиях в Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="0988b-105">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="0988b-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Activity Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="0988b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="0988b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0988b-107">Permissions</span></span>

<span data-ttu-id="0988b-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0988b-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0988b-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0988b-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0988b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0988b-110">Permission type</span></span>                        | <span data-ttu-id="0988b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0988b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0988b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0988b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0988b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0988b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0988b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0988b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0988b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0988b-115">Not supported.</span></span>                           |
| <span data-ttu-id="0988b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0988b-116">Application</span></span>                            | <span data-ttu-id="0988b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0988b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0988b-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0988b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0988b-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0988b-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0988b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0988b-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0988b-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0988b-121">Function parameters</span></span>

<span data-ttu-id="0988b-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0988b-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0988b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="0988b-123">Parameter</span></span> | <span data-ttu-id="0988b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0988b-124">Type</span></span>   | <span data-ttu-id="0988b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0988b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0988b-126">period</span><span class="sxs-lookup"><span data-stu-id="0988b-126">period</span></span>    | <span data-ttu-id="0988b-127">string</span><span class="sxs-lookup"><span data-stu-id="0988b-127">string</span></span> | <span data-ttu-id="0988b-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0988b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0988b-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0988b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0988b-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0988b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0988b-131">date</span><span class="sxs-lookup"><span data-stu-id="0988b-131">date</span></span>      | <span data-ttu-id="0988b-132">Date</span><span class="sxs-lookup"><span data-stu-id="0988b-132">Date</span></span>   | <span data-ttu-id="0988b-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="0988b-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0988b-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="0988b-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0988b-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="0988b-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0988b-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="0988b-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0988b-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0988b-137">Request headers</span></span>

| <span data-ttu-id="0988b-138">Имя</span><span class="sxs-lookup"><span data-stu-id="0988b-138">Name</span></span>          | <span data-ttu-id="0988b-139">Описание</span><span class="sxs-lookup"><span data-stu-id="0988b-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0988b-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0988b-140">Authorization</span></span> | <span data-ttu-id="0988b-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0988b-141">Bearer {token}.</span></span> <span data-ttu-id="0988b-142">Required.</span><span class="sxs-lookup"><span data-stu-id="0988b-142">Required.</span></span>                |
| <span data-ttu-id="0988b-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0988b-143">If-None-Match</span></span> | <span data-ttu-id="0988b-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="0988b-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0988b-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0988b-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0988b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0988b-146">Response</span></span>

<span data-ttu-id="0988b-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0988b-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0988b-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0988b-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0988b-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0988b-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0988b-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0988b-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0988b-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0988b-151">Report Refresh Date</span></span>
- <span data-ttu-id="0988b-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="0988b-152">User Principal Name</span></span>
- <span data-ttu-id="0988b-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="0988b-153">Display Name</span></span>
- <span data-ttu-id="0988b-154">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="0988b-154">User State</span></span>
- <span data-ttu-id="0988b-155">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="0988b-155">State Change Date</span></span>
- <span data-ttu-id="0988b-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="0988b-156">Last Activity Date</span></span>
- <span data-ttu-id="0988b-157">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="0988b-157">Posted Count</span></span>
- <span data-ttu-id="0988b-158">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="0988b-158">Read Count</span></span>
- <span data-ttu-id="0988b-159">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="0988b-159">Liked Count</span></span>
- <span data-ttu-id="0988b-160">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="0988b-160">Assigned Products</span></span>
- <span data-ttu-id="0988b-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="0988b-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0988b-162">Пример</span><span class="sxs-lookup"><span data-stu-id="0988b-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0988b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="0988b-163">Request</span></span>

<span data-ttu-id="0988b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0988b-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="0988b-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="0988b-165">Response</span></span>

<span data-ttu-id="0988b-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0988b-166">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="0988b-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="0988b-167">Request</span></span>

<span data-ttu-id="0988b-168">Если параметр указан, то в отчет выдаются `date` действия, выполняемые на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="0988b-168">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="0988b-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="0988b-169">Response</span></span>

<span data-ttu-id="0988b-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0988b-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```


<span data-ttu-id="0988b-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0988b-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
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
