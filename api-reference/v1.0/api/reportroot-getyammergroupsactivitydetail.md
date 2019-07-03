---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5b213b0ab159587e82219a3314fbe120b359790b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461381"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="151d8-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="151d8-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="151d8-104">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="151d8-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="151d8-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="151d8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="151d8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="151d8-106">Permissions</span></span>

<span data-ttu-id="151d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="151d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="151d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="151d8-109">Permission type</span></span>                        | <span data-ttu-id="151d8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="151d8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="151d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="151d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="151d8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="151d8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="151d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="151d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="151d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="151d8-114">Not supported.</span></span>                           |
| <span data-ttu-id="151d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="151d8-115">Application</span></span>                            | <span data-ttu-id="151d8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="151d8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="151d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="151d8-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="151d8-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="151d8-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="151d8-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="151d8-119">Function parameters</span></span>

<span data-ttu-id="151d8-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="151d8-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="151d8-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="151d8-121">Parameter</span></span> | <span data-ttu-id="151d8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="151d8-122">Type</span></span>   | <span data-ttu-id="151d8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="151d8-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="151d8-124">period</span><span class="sxs-lookup"><span data-stu-id="151d8-124">period</span></span>    | <span data-ttu-id="151d8-125">string</span><span class="sxs-lookup"><span data-stu-id="151d8-125">string</span></span> | <span data-ttu-id="151d8-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="151d8-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="151d8-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="151d8-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="151d8-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="151d8-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="151d8-129">date</span><span class="sxs-lookup"><span data-stu-id="151d8-129">date</span></span>      | <span data-ttu-id="151d8-130">Date</span><span class="sxs-lookup"><span data-stu-id="151d8-130">Date</span></span>   | <span data-ttu-id="151d8-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="151d8-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="151d8-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="151d8-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="151d8-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="151d8-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="151d8-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="151d8-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="151d8-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="151d8-135">Request headers</span></span>

| <span data-ttu-id="151d8-136">Имя</span><span class="sxs-lookup"><span data-stu-id="151d8-136">Name</span></span>          | <span data-ttu-id="151d8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="151d8-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="151d8-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="151d8-138">Authorization</span></span> | <span data-ttu-id="151d8-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="151d8-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="151d8-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="151d8-141">If-None-Match</span></span> | <span data-ttu-id="151d8-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="151d8-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="151d8-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="151d8-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="151d8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="151d8-144">Response</span></span>

<span data-ttu-id="151d8-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="151d8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="151d8-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="151d8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="151d8-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="151d8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="151d8-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="151d8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="151d8-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="151d8-149">Report Refresh Date</span></span>
- <span data-ttu-id="151d8-150">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="151d8-150">Group Display Name</span></span>
- <span data-ttu-id="151d8-151">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="151d8-151">Is Deleted</span></span>
- <span data-ttu-id="151d8-152">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="151d8-152">Owner Principal Name</span></span>
- <span data-ttu-id="151d8-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="151d8-153">Last Activity Date</span></span>
- <span data-ttu-id="151d8-154">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="151d8-154">Group Type</span></span>
- <span data-ttu-id="151d8-155">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="151d8-155">Office 365 Connected</span></span>
- <span data-ttu-id="151d8-156">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="151d8-156">Member Count</span></span>
- <span data-ttu-id="151d8-157">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="151d8-157">Posted Count</span></span>
- <span data-ttu-id="151d8-158">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="151d8-158">Read Count</span></span>
- <span data-ttu-id="151d8-159">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="151d8-159">Liked Count</span></span>
- <span data-ttu-id="151d8-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="151d8-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="151d8-161">Пример</span><span class="sxs-lookup"><span data-stu-id="151d8-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="151d8-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="151d8-162">Request</span></span>

<span data-ttu-id="151d8-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="151d8-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="151d8-164">C#</span><span class="sxs-lookup"><span data-stu-id="151d8-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="151d8-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="151d8-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="151d8-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="151d8-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="151d8-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="151d8-167">Response</span></span>

<span data-ttu-id="151d8-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="151d8-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="151d8-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="151d8-169">Request</span></span>
<span data-ttu-id="151d8-170">При вызове с `date`параметром a для отчета предоставляется область действия на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="151d8-170">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="151d8-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="151d8-171">Response</span></span>

<span data-ttu-id="151d8-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="151d8-172">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="151d8-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="151d8-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
