---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 29363dde998fa641bddbaee6e436ed70458f4975
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022063"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="1a9b1-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="1a9b1-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="1a9b1-105">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="1a9b1-106">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="1a9b1-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="1a9b1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a9b1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a9b1-108">Permissions</span></span>

<span data-ttu-id="1a9b1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a9b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a9b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a9b1-111">Permission type</span></span>                        | <span data-ttu-id="1a9b1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a9b1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1a9b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a9b1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a9b1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a9b1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1a9b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a9b1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a9b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-116">Not supported.</span></span>                           |
| <span data-ttu-id="1a9b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a9b1-117">Application</span></span>                            | <span data-ttu-id="1a9b1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a9b1-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1a9b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a9b1-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1a9b1-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a9b1-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1a9b1-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1a9b1-121">Function parameters</span></span>

<span data-ttu-id="1a9b1-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1a9b1-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a9b1-123">Parameter</span></span> | <span data-ttu-id="1a9b1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1a9b1-124">Type</span></span>   | <span data-ttu-id="1a9b1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1a9b1-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1a9b1-126">period</span><span class="sxs-lookup"><span data-stu-id="1a9b1-126">period</span></span>    | <span data-ttu-id="1a9b1-127">string</span><span class="sxs-lookup"><span data-stu-id="1a9b1-127">string</span></span> | <span data-ttu-id="1a9b1-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1a9b1-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1a9b1-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1a9b1-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1a9b1-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a9b1-132">Request headers</span></span>

| <span data-ttu-id="1a9b1-133">Имя</span><span class="sxs-lookup"><span data-stu-id="1a9b1-133">Name</span></span>          | <span data-ttu-id="1a9b1-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1a9b1-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1a9b1-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a9b1-135">Authorization</span></span> | <span data-ttu-id="1a9b1-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1a9b1-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1a9b1-138">If-None-Match</span></span> | <span data-ttu-id="1a9b1-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1a9b1-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1a9b1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a9b1-141">Response</span></span>

<span data-ttu-id="1a9b1-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1a9b1-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1a9b1-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1a9b1-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1a9b1-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1a9b1-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1a9b1-146">Report Refresh Date</span></span>
- <span data-ttu-id="1a9b1-147">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="1a9b1-147">Total</span></span>
- <span data-ttu-id="1a9b1-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="1a9b1-148">Active</span></span>
- <span data-ttu-id="1a9b1-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="1a9b1-149">Report Date</span></span>
- <span data-ttu-id="1a9b1-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="1a9b1-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1a9b1-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1a9b1-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1a9b1-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a9b1-152">Request</span></span>

<span data-ttu-id="1a9b1-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a9b1-154">C#</span><span class="sxs-lookup"><span data-stu-id="1a9b1-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a9b1-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a9b1-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a9b1-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1a9b1-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a9b1-157">Java</span><span class="sxs-lookup"><span data-stu-id="1a9b1-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a9b1-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a9b1-158">Response</span></span>

<span data-ttu-id="1a9b1-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="1a9b1-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1a9b1-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
