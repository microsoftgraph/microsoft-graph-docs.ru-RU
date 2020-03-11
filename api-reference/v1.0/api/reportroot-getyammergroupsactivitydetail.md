---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7bf0bf8ce8950e823fce9d6d8a4a3c5c42aa93a1
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591154"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="b3a6e-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="b3a6e-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="b3a6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3a6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3a6e-105">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-105">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="b3a6e-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="b3a6e-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3a6e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a6e-107">Permissions</span></span>

<span data-ttu-id="b3a6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3a6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3a6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a6e-110">Permission type</span></span>                        | <span data-ttu-id="b3a6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b3a6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3a6e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3a6e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b3a6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3a6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-115">Not supported.</span></span>                           |
| <span data-ttu-id="b3a6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3a6e-116">Application</span></span>                            | <span data-ttu-id="b3a6e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3a6e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="b3a6e-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b3a6e-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b3a6e-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b3a6e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3a6e-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b3a6e-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b3a6e-121">Function parameters</span></span>

<span data-ttu-id="b3a6e-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b3a6e-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3a6e-123">Parameter</span></span> | <span data-ttu-id="b3a6e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b3a6e-124">Type</span></span>   | <span data-ttu-id="b3a6e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b3a6e-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b3a6e-126">period</span><span class="sxs-lookup"><span data-stu-id="b3a6e-126">period</span></span>    | <span data-ttu-id="b3a6e-127">string</span><span class="sxs-lookup"><span data-stu-id="b3a6e-127">string</span></span> | <span data-ttu-id="b3a6e-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b3a6e-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b3a6e-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b3a6e-131">date</span><span class="sxs-lookup"><span data-stu-id="b3a6e-131">date</span></span>      | <span data-ttu-id="b3a6e-132">Date</span><span class="sxs-lookup"><span data-stu-id="b3a6e-132">Date</span></span>   | <span data-ttu-id="b3a6e-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b3a6e-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b3a6e-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b3a6e-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3a6e-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3a6e-137">Request headers</span></span>

| <span data-ttu-id="b3a6e-138">Имя</span><span class="sxs-lookup"><span data-stu-id="b3a6e-138">Name</span></span>          | <span data-ttu-id="b3a6e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b3a6e-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b3a6e-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3a6e-140">Authorization</span></span> | <span data-ttu-id="b3a6e-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b3a6e-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b3a6e-143">If-None-Match</span></span> | <span data-ttu-id="b3a6e-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b3a6e-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b3a6e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3a6e-146">Response</span></span>

<span data-ttu-id="b3a6e-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b3a6e-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b3a6e-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b3a6e-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b3a6e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b3a6e-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b3a6e-151">Report Refresh Date</span></span>
- <span data-ttu-id="b3a6e-152">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-152">Group Display Name</span></span>
- <span data-ttu-id="b3a6e-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-153">Is Deleted</span></span>
- <span data-ttu-id="b3a6e-154">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-154">Owner Principal Name</span></span>
- <span data-ttu-id="b3a6e-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-155">Last Activity Date</span></span>
- <span data-ttu-id="b3a6e-156">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-156">Group Type</span></span>
- <span data-ttu-id="b3a6e-157">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-157">Office 365 Connected</span></span>
- <span data-ttu-id="b3a6e-158">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-158">Member Count</span></span>
- <span data-ttu-id="b3a6e-159">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-159">Posted Count</span></span>
- <span data-ttu-id="b3a6e-160">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-160">Read Count</span></span>
- <span data-ttu-id="b3a6e-161">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="b3a6e-161">Liked Count</span></span>
- <span data-ttu-id="b3a6e-162">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b3a6e-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b3a6e-163">Пример</span><span class="sxs-lookup"><span data-stu-id="b3a6e-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b3a6e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3a6e-164">Request</span></span>

<span data-ttu-id="b3a6e-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-165">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="b3a6e-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3a6e-166">Response</span></span>

<span data-ttu-id="b3a6e-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-167">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="b3a6e-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3a6e-168">Request</span></span>
<span data-ttu-id="b3a6e-169">При вызове с `date`параметром a для отчета предоставляется область действия на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-169">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="b3a6e-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3a6e-170">Response</span></span>

<span data-ttu-id="b3a6e-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-171">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b3a6e-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b3a6e-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
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
