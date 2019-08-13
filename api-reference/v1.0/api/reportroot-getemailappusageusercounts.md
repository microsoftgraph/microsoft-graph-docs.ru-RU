---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e50835d96aacfbed50e0655e2c8f6435735a98ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327352"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="38165-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="38165-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="38165-104">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="38165-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="38165-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="38165-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="38165-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38165-106">Permissions</span></span>

<span data-ttu-id="38165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38165-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38165-109">Permission type</span></span>                        | <span data-ttu-id="38165-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38165-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38165-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38165-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38165-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38165-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38165-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38165-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38165-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38165-114">Not supported.</span></span>                           |
| <span data-ttu-id="38165-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38165-115">Application</span></span>                            | <span data-ttu-id="38165-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38165-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="38165-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38165-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="38165-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="38165-118">Function parameters</span></span>

<span data-ttu-id="38165-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="38165-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="38165-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="38165-120">Parameter</span></span> | <span data-ttu-id="38165-121">Тип</span><span class="sxs-lookup"><span data-stu-id="38165-121">Type</span></span>   | <span data-ttu-id="38165-122">Описание</span><span class="sxs-lookup"><span data-stu-id="38165-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38165-123">period</span><span class="sxs-lookup"><span data-stu-id="38165-123">period</span></span>    | <span data-ttu-id="38165-124">string</span><span class="sxs-lookup"><span data-stu-id="38165-124">string</span></span> | <span data-ttu-id="38165-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="38165-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38165-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="38165-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38165-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="38165-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="38165-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38165-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="38165-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38165-129">Request headers</span></span>

| <span data-ttu-id="38165-130">Имя</span><span class="sxs-lookup"><span data-stu-id="38165-130">Name</span></span>          | <span data-ttu-id="38165-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38165-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="38165-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38165-132">Authorization</span></span> | <span data-ttu-id="38165-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38165-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="38165-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="38165-135">If-None-Match</span></span> | <span data-ttu-id="38165-136">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="38165-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="38165-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="38165-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="38165-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="38165-138">Response</span></span>

<span data-ttu-id="38165-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="38165-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38165-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="38165-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38165-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="38165-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38165-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="38165-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38165-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="38165-143">Report Refresh Date</span></span>
- <span data-ttu-id="38165-144">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="38165-144">Mail For Mac</span></span>
- <span data-ttu-id="38165-145">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="38165-145">Outlook For Mac</span></span>
- <span data-ttu-id="38165-146">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="38165-146">Outlook For Windows</span></span>
- <span data-ttu-id="38165-147">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="38165-147">Outlook For Mobile</span></span>
- <span data-ttu-id="38165-148">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="38165-148">Other For Mobile</span></span>
- <span data-ttu-id="38165-149">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="38165-149">Outlook For Web</span></span>
- <span data-ttu-id="38165-150">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="38165-150">POP3 App</span></span>
- <span data-ttu-id="38165-151">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="38165-151">IMAP4 App</span></span>
- <span data-ttu-id="38165-152">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="38165-152">SMTP App</span></span>
- <span data-ttu-id="38165-153">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="38165-153">Report Date</span></span>
- <span data-ttu-id="38165-154">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="38165-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="38165-155">Пример</span><span class="sxs-lookup"><span data-stu-id="38165-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="38165-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="38165-156">Request</span></span>

<span data-ttu-id="38165-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38165-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="38165-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="38165-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38165-159">C#</span><span class="sxs-lookup"><span data-stu-id="38165-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38165-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38165-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38165-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="38165-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="38165-162">Java</span><span class="sxs-lookup"><span data-stu-id="38165-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38165-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="38165-163">Response</span></span>

<span data-ttu-id="38165-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38165-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="38165-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="38165-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
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
