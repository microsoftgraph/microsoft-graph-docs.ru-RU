---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4bdd20168d9f6e1fc9d365a165ee2597f8c6165e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268826"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="2581d-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="2581d-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="2581d-104">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="2581d-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="2581d-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="2581d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="2581d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2581d-106">Permissions</span></span>

<span data-ttu-id="2581d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2581d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2581d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2581d-109">Permission type</span></span>                        | <span data-ttu-id="2581d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2581d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2581d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2581d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2581d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2581d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2581d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2581d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2581d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2581d-114">Not supported.</span></span>                           |
| <span data-ttu-id="2581d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2581d-115">Application</span></span>                            | <span data-ttu-id="2581d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2581d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2581d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2581d-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2581d-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2581d-118">Function parameters</span></span>

<span data-ttu-id="2581d-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2581d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2581d-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="2581d-120">Parameter</span></span> | <span data-ttu-id="2581d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2581d-121">Type</span></span>   | <span data-ttu-id="2581d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2581d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2581d-123">period</span><span class="sxs-lookup"><span data-stu-id="2581d-123">period</span></span>    | <span data-ttu-id="2581d-124">string</span><span class="sxs-lookup"><span data-stu-id="2581d-124">string</span></span> | <span data-ttu-id="2581d-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2581d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2581d-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2581d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2581d-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2581d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2581d-128">date</span><span class="sxs-lookup"><span data-stu-id="2581d-128">date</span></span>      | <span data-ttu-id="2581d-129">Date</span><span class="sxs-lookup"><span data-stu-id="2581d-129">Date</span></span>   | <span data-ttu-id="2581d-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="2581d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2581d-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="2581d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2581d-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="2581d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2581d-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="2581d-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2581d-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2581d-134">Request headers</span></span>

| <span data-ttu-id="2581d-135">Имя</span><span class="sxs-lookup"><span data-stu-id="2581d-135">Name</span></span>          | <span data-ttu-id="2581d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="2581d-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2581d-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2581d-137">Authorization</span></span> | <span data-ttu-id="2581d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2581d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2581d-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2581d-140">If-None-Match</span></span> | <span data-ttu-id="2581d-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="2581d-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2581d-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2581d-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2581d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2581d-143">Response</span></span>

<span data-ttu-id="2581d-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2581d-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2581d-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2581d-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2581d-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2581d-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2581d-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2581d-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2581d-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2581d-148">Report Refresh Date</span></span>
- <span data-ttu-id="2581d-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="2581d-149">User Principal Name</span></span>
- <span data-ttu-id="2581d-150">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="2581d-150">Display Name</span></span>
- <span data-ttu-id="2581d-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="2581d-151">Is Deleted</span></span>
- <span data-ttu-id="2581d-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="2581d-152">Deleted Date</span></span>
- <span data-ttu-id="2581d-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="2581d-153">Last Activity Date</span></span>
- <span data-ttu-id="2581d-154">"Mail For Mac" (Почта для Mac);</span><span class="sxs-lookup"><span data-stu-id="2581d-154">Mail For Mac</span></span>
- <span data-ttu-id="2581d-155">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="2581d-155">Outlook For Mac</span></span>
- <span data-ttu-id="2581d-156">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="2581d-156">Outlook For Windows</span></span>
- <span data-ttu-id="2581d-157">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="2581d-157">Outlook For Mobile</span></span>
- <span data-ttu-id="2581d-158">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="2581d-158">Other For Mobile</span></span>
- <span data-ttu-id="2581d-159">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="2581d-159">Outlook For Web</span></span>
- <span data-ttu-id="2581d-160">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="2581d-160">POP3 App</span></span>
- <span data-ttu-id="2581d-161">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="2581d-161">IMAP4 App</span></span>
- <span data-ttu-id="2581d-162">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="2581d-162">SMTP App</span></span>
- <span data-ttu-id="2581d-163">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="2581d-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2581d-164">Пример</span><span class="sxs-lookup"><span data-stu-id="2581d-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2581d-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="2581d-165">Request</span></span>

<span data-ttu-id="2581d-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2581d-166">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2581d-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="2581d-167">Response</span></span>

<span data-ttu-id="2581d-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2581d-168">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2581d-169">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="2581d-169">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2581d-170">C#</span><span class="sxs-lookup"><span data-stu-id="2581d-170">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2581d-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="2581d-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2581d-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2581d-172">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="2581d-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2581d-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
