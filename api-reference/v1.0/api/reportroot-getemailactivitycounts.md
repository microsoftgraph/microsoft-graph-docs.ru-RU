---
title: 'reportRoot: getEmailActivityCounts'
description: Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2dd98b73f3dbba6881bc7e68f4d0657d49e1b3c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022091"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="f26f9-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f26f9-103">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="f26f9-104">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="f26f9-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="f26f9-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="f26f9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="f26f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f26f9-106">Permissions</span></span>

<span data-ttu-id="f26f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f26f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f26f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f26f9-109">Permission type</span></span>                        | <span data-ttu-id="f26f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f26f9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f26f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f26f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f26f9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f26f9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f26f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f26f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f26f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f26f9-114">Not supported.</span></span>                           |
| <span data-ttu-id="f26f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f26f9-115">Application</span></span>                            | <span data-ttu-id="f26f9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f26f9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f26f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f26f9-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f26f9-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="f26f9-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f26f9-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f26f9-119">Function parameters</span></span>

<span data-ttu-id="f26f9-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f26f9-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f26f9-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="f26f9-121">Parameter</span></span> | <span data-ttu-id="f26f9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f26f9-122">Type</span></span>   | <span data-ttu-id="f26f9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f26f9-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f26f9-124">period</span><span class="sxs-lookup"><span data-stu-id="f26f9-124">period</span></span>    | <span data-ttu-id="f26f9-125">string</span><span class="sxs-lookup"><span data-stu-id="f26f9-125">string</span></span> | <span data-ttu-id="f26f9-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f26f9-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f26f9-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f26f9-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f26f9-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f26f9-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f26f9-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f26f9-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f26f9-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f26f9-130">Request headers</span></span>

| <span data-ttu-id="f26f9-131">Имя</span><span class="sxs-lookup"><span data-stu-id="f26f9-131">Name</span></span>          | <span data-ttu-id="f26f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f26f9-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f26f9-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f26f9-133">Authorization</span></span> | <span data-ttu-id="f26f9-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f26f9-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f26f9-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f26f9-136">If-None-Match</span></span> | <span data-ttu-id="f26f9-137">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f26f9-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f26f9-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f26f9-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f26f9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f26f9-139">Response</span></span>

<span data-ttu-id="f26f9-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f26f9-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f26f9-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f26f9-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f26f9-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f26f9-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f26f9-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f26f9-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f26f9-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f26f9-144">Report Refresh Date</span></span>
- <span data-ttu-id="f26f9-145">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="f26f9-145">Send</span></span>
- <span data-ttu-id="f26f9-146">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="f26f9-146">Receive</span></span>
- <span data-ttu-id="f26f9-147">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="f26f9-147">Read</span></span>
- <span data-ttu-id="f26f9-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="f26f9-148">Report Date</span></span>
- <span data-ttu-id="f26f9-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="f26f9-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f26f9-150">Пример</span><span class="sxs-lookup"><span data-stu-id="f26f9-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f26f9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="f26f9-151">Request</span></span>

<span data-ttu-id="f26f9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f26f9-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f26f9-153">C#</span><span class="sxs-lookup"><span data-stu-id="f26f9-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f26f9-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="f26f9-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f26f9-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f26f9-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f26f9-156">Java</span><span class="sxs-lookup"><span data-stu-id="f26f9-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f26f9-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="f26f9-157">Response</span></span>

<span data-ttu-id="f26f9-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f26f9-158">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f26f9-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f26f9-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
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
