---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d38cc8a5cd6cfad9d7b98c61a054f57e230208da
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865197"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="567c7-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="567c7-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="567c7-104">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="567c7-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="567c7-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="567c7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="567c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="567c7-106">Permissions</span></span>

<span data-ttu-id="567c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="567c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="567c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="567c7-109">Permission type</span></span>                        | <span data-ttu-id="567c7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="567c7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="567c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="567c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="567c7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="567c7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="567c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="567c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="567c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="567c7-114">Not supported.</span></span>                           |
| <span data-ttu-id="567c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="567c7-115">Application</span></span>                            | <span data-ttu-id="567c7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="567c7-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="567c7-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="567c7-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="567c7-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="567c7-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="567c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="567c7-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="567c7-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="567c7-120">Function parameters</span></span>

<span data-ttu-id="567c7-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="567c7-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="567c7-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="567c7-122">Parameter</span></span> | <span data-ttu-id="567c7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="567c7-123">Type</span></span>   | <span data-ttu-id="567c7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="567c7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="567c7-125">period</span><span class="sxs-lookup"><span data-stu-id="567c7-125">period</span></span>    | <span data-ttu-id="567c7-126">string</span><span class="sxs-lookup"><span data-stu-id="567c7-126">string</span></span> | <span data-ttu-id="567c7-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="567c7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="567c7-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="567c7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="567c7-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="567c7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="567c7-130">date</span><span class="sxs-lookup"><span data-stu-id="567c7-130">date</span></span>      | <span data-ttu-id="567c7-131">Date</span><span class="sxs-lookup"><span data-stu-id="567c7-131">Date</span></span>   | <span data-ttu-id="567c7-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="567c7-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="567c7-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="567c7-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="567c7-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="567c7-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="567c7-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="567c7-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="567c7-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="567c7-136">Request headers</span></span>

| <span data-ttu-id="567c7-137">Имя</span><span class="sxs-lookup"><span data-stu-id="567c7-137">Name</span></span>          | <span data-ttu-id="567c7-138">Описание</span><span class="sxs-lookup"><span data-stu-id="567c7-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="567c7-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="567c7-139">Authorization</span></span> | <span data-ttu-id="567c7-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="567c7-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="567c7-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="567c7-142">If-None-Match</span></span> | <span data-ttu-id="567c7-143">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="567c7-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="567c7-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="567c7-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="567c7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="567c7-145">Response</span></span>

<span data-ttu-id="567c7-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="567c7-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="567c7-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="567c7-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="567c7-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="567c7-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="567c7-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="567c7-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="567c7-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="567c7-150">Report Refresh Date</span></span>
- <span data-ttu-id="567c7-151">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="567c7-151">Group Display Name</span></span>
- <span data-ttu-id="567c7-152">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="567c7-152">Is Deleted</span></span>
- <span data-ttu-id="567c7-153">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="567c7-153">Owner Principal Name</span></span>
- <span data-ttu-id="567c7-154">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="567c7-154">Last Activity Date</span></span>
- <span data-ttu-id="567c7-155">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="567c7-155">Group Type</span></span>
- <span data-ttu-id="567c7-156">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="567c7-156">Office 365 Connected</span></span>
- <span data-ttu-id="567c7-157">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="567c7-157">Member Count</span></span>
- <span data-ttu-id="567c7-158">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="567c7-158">Posted Count</span></span>
- <span data-ttu-id="567c7-159">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="567c7-159">Read Count</span></span>
- <span data-ttu-id="567c7-160">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="567c7-160">Liked Count</span></span>
- <span data-ttu-id="567c7-161">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="567c7-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="567c7-162">Пример</span><span class="sxs-lookup"><span data-stu-id="567c7-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="567c7-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="567c7-163">Request</span></span>

<span data-ttu-id="567c7-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="567c7-164">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="567c7-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="567c7-165">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="567c7-166">C#</span><span class="sxs-lookup"><span data-stu-id="567c7-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="567c7-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="567c7-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="567c7-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="567c7-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="567c7-169">Java</span><span class="sxs-lookup"><span data-stu-id="567c7-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="567c7-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="567c7-170">Response</span></span>

<span data-ttu-id="567c7-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="567c7-171">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="567c7-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="567c7-172">Request</span></span>
<span data-ttu-id="567c7-173">При вызове с `date`параметром a для отчета предоставляется область действия на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="567c7-173">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="567c7-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="567c7-174">Response</span></span>

<span data-ttu-id="567c7-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="567c7-175">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="567c7-176">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="567c7-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
