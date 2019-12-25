---
title: 'reportRoot: getEmailActivityUserDetail'
description: Узнайте, какие действия пользователи выполняли с электронной почтой.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 89985d1349a1f10811ce8fca7dbd393bad82f68e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864511"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="0b632-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0b632-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="0b632-104">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="0b632-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="0b632-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="0b632-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b632-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b632-106">Permissions</span></span>

<span data-ttu-id="0b632-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b632-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b632-109">Permission type</span></span>                        | <span data-ttu-id="0b632-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b632-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b632-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b632-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b632-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b632-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b632-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b632-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b632-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b632-114">Not supported.</span></span>                           |
| <span data-ttu-id="0b632-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b632-115">Application</span></span>                            | <span data-ttu-id="0b632-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b632-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="0b632-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0b632-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0b632-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0b632-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0b632-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b632-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0b632-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0b632-120">Function parameters</span></span>

<span data-ttu-id="0b632-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0b632-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0b632-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="0b632-122">Parameter</span></span> | <span data-ttu-id="0b632-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0b632-123">Type</span></span>   | <span data-ttu-id="0b632-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0b632-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b632-125">period</span><span class="sxs-lookup"><span data-stu-id="0b632-125">period</span></span>    | <span data-ttu-id="0b632-126">string</span><span class="sxs-lookup"><span data-stu-id="0b632-126">string</span></span> | <span data-ttu-id="0b632-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0b632-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b632-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0b632-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b632-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0b632-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0b632-130">date</span><span class="sxs-lookup"><span data-stu-id="0b632-130">date</span></span>      | <span data-ttu-id="0b632-131">Date</span><span class="sxs-lookup"><span data-stu-id="0b632-131">Date</span></span>   | <span data-ttu-id="0b632-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="0b632-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0b632-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="0b632-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0b632-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="0b632-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0b632-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="0b632-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b632-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b632-136">Request headers</span></span>

| <span data-ttu-id="0b632-137">Имя</span><span class="sxs-lookup"><span data-stu-id="0b632-137">Name</span></span>          | <span data-ttu-id="0b632-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0b632-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0b632-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b632-139">Authorization</span></span> | <span data-ttu-id="0b632-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b632-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0b632-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0b632-142">If-None-Match</span></span> | <span data-ttu-id="0b632-143">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="0b632-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0b632-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0b632-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0b632-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b632-145">Response</span></span>

<span data-ttu-id="0b632-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0b632-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b632-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0b632-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b632-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0b632-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b632-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0b632-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b632-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0b632-150">Report Refresh Date</span></span>
- <span data-ttu-id="0b632-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="0b632-151">User Principal Name</span></span>
- <span data-ttu-id="0b632-152">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="0b632-152">Display Name</span></span>
- <span data-ttu-id="0b632-153">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="0b632-153">Is Deleted</span></span>
- <span data-ttu-id="0b632-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="0b632-154">Deleted Date</span></span>
- <span data-ttu-id="0b632-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="0b632-155">Last Activity Date</span></span>
- <span data-ttu-id="0b632-156">Send Count (количество отправленных писем)</span><span class="sxs-lookup"><span data-stu-id="0b632-156">Send Count</span></span>
- <span data-ttu-id="0b632-157">Receive Count (количество полученных писем)</span><span class="sxs-lookup"><span data-stu-id="0b632-157">Receive Count</span></span>
- <span data-ttu-id="0b632-158">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="0b632-158">Read Count</span></span>
- <span data-ttu-id="0b632-159">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="0b632-159">Assigned Products</span></span>
- <span data-ttu-id="0b632-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="0b632-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0b632-161">Пример</span><span class="sxs-lookup"><span data-stu-id="0b632-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0b632-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b632-162">Request</span></span>

<span data-ttu-id="0b632-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b632-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b632-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b632-164">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b632-165">C#</span><span class="sxs-lookup"><span data-stu-id="0b632-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b632-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b632-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b632-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b632-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b632-168">Java</span><span class="sxs-lookup"><span data-stu-id="0b632-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b632-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b632-169">Response</span></span>

<span data-ttu-id="0b632-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b632-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="0b632-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0b632-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
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
