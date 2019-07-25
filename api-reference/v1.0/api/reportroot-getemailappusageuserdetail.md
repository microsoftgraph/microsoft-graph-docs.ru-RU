---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e73eeb096bbb6cdf31ccff66a3cf546fa10f6b34
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886347"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="f9277-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f9277-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="f9277-104">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="f9277-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="f9277-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="f9277-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9277-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9277-106">Permissions</span></span>

<span data-ttu-id="f9277-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9277-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9277-109">Permission type</span></span>                        | <span data-ttu-id="f9277-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9277-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f9277-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9277-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9277-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9277-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f9277-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9277-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9277-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9277-114">Not supported.</span></span>                           |
| <span data-ttu-id="f9277-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9277-115">Application</span></span>                            | <span data-ttu-id="f9277-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9277-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f9277-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9277-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9277-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9277-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f9277-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f9277-119">Function parameters</span></span>

<span data-ttu-id="f9277-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f9277-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f9277-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="f9277-121">Parameter</span></span> | <span data-ttu-id="f9277-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f9277-122">Type</span></span>   | <span data-ttu-id="f9277-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f9277-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f9277-124">period</span><span class="sxs-lookup"><span data-stu-id="f9277-124">period</span></span>    | <span data-ttu-id="f9277-125">string</span><span class="sxs-lookup"><span data-stu-id="f9277-125">string</span></span> | <span data-ttu-id="f9277-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f9277-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f9277-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f9277-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f9277-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f9277-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f9277-129">date</span><span class="sxs-lookup"><span data-stu-id="f9277-129">date</span></span>      | <span data-ttu-id="f9277-130">Date</span><span class="sxs-lookup"><span data-stu-id="f9277-130">Date</span></span>   | <span data-ttu-id="f9277-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="f9277-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f9277-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="f9277-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f9277-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="f9277-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f9277-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="f9277-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9277-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9277-135">Request headers</span></span>

| <span data-ttu-id="f9277-136">Имя</span><span class="sxs-lookup"><span data-stu-id="f9277-136">Name</span></span>          | <span data-ttu-id="f9277-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f9277-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f9277-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9277-138">Authorization</span></span> | <span data-ttu-id="f9277-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9277-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f9277-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f9277-141">If-None-Match</span></span> | <span data-ttu-id="f9277-142">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f9277-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f9277-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f9277-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f9277-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9277-144">Response</span></span>

<span data-ttu-id="f9277-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f9277-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f9277-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f9277-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f9277-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f9277-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f9277-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f9277-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f9277-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f9277-149">Report Refresh Date</span></span>
- <span data-ttu-id="f9277-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="f9277-150">User Principal Name</span></span>
- <span data-ttu-id="f9277-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="f9277-151">Display Name</span></span>
- <span data-ttu-id="f9277-152">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="f9277-152">Is Deleted</span></span>
- <span data-ttu-id="f9277-153">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="f9277-153">Deleted Date</span></span>
- <span data-ttu-id="f9277-154">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="f9277-154">Last Activity Date</span></span>
- <span data-ttu-id="f9277-155">"Mail For Mac" (Почта для Mac);</span><span class="sxs-lookup"><span data-stu-id="f9277-155">Mail For Mac</span></span>
- <span data-ttu-id="f9277-156">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="f9277-156">Outlook For Mac</span></span>
- <span data-ttu-id="f9277-157">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="f9277-157">Outlook For Windows</span></span>
- <span data-ttu-id="f9277-158">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="f9277-158">Outlook For Mobile</span></span>
- <span data-ttu-id="f9277-159">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="f9277-159">Other For Mobile</span></span>
- <span data-ttu-id="f9277-160">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="f9277-160">Outlook For Web</span></span>
- <span data-ttu-id="f9277-161">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="f9277-161">POP3 App</span></span>
- <span data-ttu-id="f9277-162">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="f9277-162">IMAP4 App</span></span>
- <span data-ttu-id="f9277-163">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="f9277-163">SMTP App</span></span>
- <span data-ttu-id="f9277-164">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="f9277-164">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f9277-165">Пример</span><span class="sxs-lookup"><span data-stu-id="f9277-165">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f9277-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9277-166">Request</span></span>

<span data-ttu-id="f9277-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9277-167">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9277-168">C#</span><span class="sxs-lookup"><span data-stu-id="f9277-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9277-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9277-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9277-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f9277-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9277-171">Java</span><span class="sxs-lookup"><span data-stu-id="f9277-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9277-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9277-172">Response</span></span>

<span data-ttu-id="f9277-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9277-173">The following is an example of the response.</span></span>

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

<span data-ttu-id="f9277-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f9277-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
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
